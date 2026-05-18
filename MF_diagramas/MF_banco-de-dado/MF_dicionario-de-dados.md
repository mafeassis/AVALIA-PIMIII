# MF_Dicionário de Dados

O Dicionário de Dados complementa o MER com a descrição detalhada de cada tabela do banco de dados relacional, incluindo restrições, valores padrão e observações relevantes para a implementação e manutenção do sistema.

---

# Tabela: Perfil

Representa os tipos de usuário do sistema (Aluno, Professor, Administrador). Define as permissões e o nível de acesso de cada conta cadastrada.

| Coluna | Tipo | Restrições | PK | FK | Nulo | Observações |
|---|---|---|---|---|---|---|
| Id | INT | — | ✓ | — | NÃO | Identificador único do perfil |
| Nome | VARCHAR(50) | — | — | — | NÃO | Nome do perfil (ex: Aluno, Professor) |

---

# Tabela: Turma

Representa um grupo de alunos da instituição. Uma turma pode ter várias disciplinas associadas e vários alunos vinculados.

| Coluna | Tipo | Restrições | PK | FK | Nulo | Observações |
|---|---|---|---|---|---|---|
| Id | INT | — | ✓ | — | NÃO | Identificador único da turma |
| Nome | VARCHAR(100) | — | — | — | NÃO | Nome ou código da turma |

---

# Tabela: Usuario

Representa qualquer usuário autenticado da plataforma (Aluno, Professor ou Administrador). O campo PerfilId determina o tipo e as permissões do usuário. TurmaId é preenchido apenas para alunos.

| Coluna | Tipo | Restrições | PK | FK | Nulo | Observações |
|---|---|---|---|---|---|---|
| Id | INT | — | ✓ | — | NÃO | Identificador único do usuário |
| Nome | VARCHAR(100) | — | — | — | NÃO | Nome completo do usuário |
| Email | VARCHAR(150) | — | — | — | NÃO | E-mail para autenticação (único) |
| Senha | VARCHAR(200) | — | — | — | NÃO | Senha criptografada do usuário |
| PerfilId | INT | → Perfil | — | ✓ | NÃO | Tipo de usuário (perfil) |
| TurmaId | INT | → Turma | — | ✓ | SIM | Turma do aluno (NULL para professor/admin) |
| FotoUrl | VARCHAR(500) | — | — | — | SIM | URL da foto de perfil do usuário |
| DataIngresso | DATETIME | — | — | — | NÃO | Data de cadastro na plataforma |
| Ativo | BIT | — | — | — | NÃO | Indica se a conta está ativa (1) ou inativa (0) |

---

# Tabela: Disciplina

Representa uma disciplina acadêmica da plataforma. Cada disciplina possui um professor responsável e é vinculada a uma ou mais turmas via Turma_Disciplina.

| Coluna | Tipo | Restrições | PK | FK | Nulo | Observações |
|---|---|---|---|---|---|---|
| Id | INT | — | ✓ | — | NÃO | Identificador único da disciplina |
| Nome | VARCHAR(150) | — | — | — | NÃO | Nome da disciplina |
| Descricao | VARCHAR(300) | — | — | — | SIM | Descrição opcional da disciplina |
| ProfessorId | INT | → Usuario | — | ✓ | NÃO | Professor responsável pela disciplina |

---

# Tabela: Turma_Disciplina

Entidade associativa que resolve o relacionamento N:N entre Turma e Disciplina. Representa as disciplinas que compõem a grade de cada turma.

| Coluna | Tipo | Restrições | PK | FK | Nulo | Observações |
|---|---|---|---|---|---|---|
| TurmaId | INT | → Turma | ✓ | ✓ | NÃO | Identificador da turma |
| DisciplinaId | INT | → Disciplina | ✓ | ✓ | NÃO | Identificador da disciplina |

---

# Tabela: Questao

Representa uma questão do banco de questões da plataforma, organizada por disciplina e nível de dificuldade. Cada questão possui alternativas de resposta associadas.

| Coluna | Tipo | Restrições | PK | FK | Nulo | Observações |
|---|---|---|---|---|---|---|
| Id | INT | — | ✓ | — | NÃO | Identificador único da questão |
| Enunciado | TEXT | — | — | — | NÃO | Texto do enunciado da questão |
| ImagemUrl | VARCHAR(500) | — | — | — | SIM | URL de imagem complementar (opcional) |
| ExplicacaoResposta | TEXT | — | — | — | SIM | Explicação exibida após correção |
| DisciplinaId | INT | → Disciplina | — | ✓ | NÃO | Disciplina à qual a questão pertence |
| Dificuldade | VARCHAR(20) | — | — | — | NÃO | Nível de dificuldade (Fácil, Médio, Difícil) |

---

# Tabela: Alternativa

Representa as alternativas de resposta de uma questão. Cada questão possui de 4 a 5 alternativas, sendo exatamente uma marcada como correta.

| Coluna | Tipo | Restrições | PK | FK | Nulo | Observações |
|---|---|---|---|---|---|---|
| Id | INT | — | ✓ | — | NÃO | Identificador único da alternativa |
| QuestaoId | INT | → Questao | — | ✓ | NÃO | Questão à qual a alternativa pertence |
| Letra | CHAR(1) | — | — | — | NÃO | Letra da alternativa (A, B, C, D ou E) |
| Texto | TEXT | — | — | — | NÃO | Texto da alternativa |
| Correta | BIT | — | — | — | NÃO | Indica se é a alternativa correta (1 = Sim) |

---

# Tabela: Simulado

Representa um simulado gerado pelo sistema. Pode ou não estar vinculado a uma disciplina específica — quando gerado de forma geral, DisciplinaId é NULL.

| Coluna | Tipo | Restrições | PK | FK | Nulo | Observações |
|---|---|---|---|---|---|---|
| Id | INT | — | ✓ | — | NÃO | Identificador único do simulado |
| Titulo | VARCHAR(200) | — | — | — | NÃO | Título descritivo do simulado |
| DisciplinaId | INT | → Disciplina | — | ✓ | SIM | Disciplina do simulado (NULL = geral) |
| QuantidadeQuestoes | INT | — | — | — | NÃO | Número de questões do simulado |
| DataCriacao | DATETIME | — | — | — | SIM | Data e hora de criação do simulado |

---

# Tabela: Simulado_Questao

Entidade associativa que resolve o relacionamento N:N entre Simulado e Questao. Armazena também a ordem de cada questão dentro do simulado.

| Coluna | Tipo | Restrições | PK | FK | Nulo | Observações |
|---|---|---|---|---|---|---|
| SimuladoId | INT | → Simulado | ✓ | ✓ | NÃO | Identificador do simulado |
| QuestaoId | INT | → Questao | ✓ | ✓ | NÃO | Identificador da questão |
| Ordem | INT | — | — | — | SIM | Posição da questão no simulado |

---

# Tabela: RespostaAluno

Registra cada resposta dada por um aluno durante a realização de um simulado. Armazena a alternativa marcada e se o aluno acertou a questão.

| Coluna | Tipo | Restrições | PK | FK | Nulo | Observações |
|---|---|---|---|---|---|---|
| Id | INT | — | ✓ | — | NÃO | Identificador único da resposta |
| UsuarioId | INT | → Usuario | — | ✓ | NÃO | Aluno que respondeu |
| QuestaoId | INT | → Questao | — | ✓ | NÃO | Questão respondida |
| SimuladoId | INT | → Simulado | — | ✓ | NÃO | Simulado ao qual a resposta pertence |
| AlternativaMarcada | CHAR(1) | — | — | — | SIM | Letra da alternativa selecionada pelo aluno |
| Acertou | BIT | — | — | — | SIM | Indica se o aluno acertou a questão |
| DataResposta | DATETIME | — | — | — | SIM | Data e hora em que a resposta foi registrada |

---

# Tabela: ResultadoSimulado

Registra o resultado consolidado de um aluno ao finalizar um simulado: total de questões, acertos e percentual de aproveitamento.

| Coluna | Tipo | Restrições | PK | FK | Nulo | Observações |
|---|---|---|---|---|---|---|
| Id | INT | — | ✓ | — | NÃO | Identificador único do resultado |
| UsuarioId | INT | → Usuario | — | ✓ | NÃO | Aluno que realizou o simulado |
| SimuladoId | INT | → Simulado | — | ✓ | NÃO | Simulado realizado |
| TotalQuestoes | INT | — | — | — | NÃO | Total de questões do simulado |
| TotalAcertos | INT | — | — | — | NÃO | Número de questões corretas |
| Percentual | DECIMAL(5,2) | — | — | — | SIM | Percentual de acertos (calculado) |
| DataRealizacao | DATETIME | — | — | — | SIM | Data e hora de conclusão do simulado |

---

# Tabela: Desempenho

Armazena o desempenho acumulado de cada aluno por disciplina. Atualizado automaticamente após a correção de cada simulado.

| Coluna | Tipo | Restrições | PK | FK | Nulo | Observações |
|---|---|---|---|---|---|---|
| Id | INT | — | ✓ | — | NÃO | Identificador único do registro |
| UsuarioId | INT | → Usuario | — | ✓ | NÃO | Aluno ao qual o desempenho pertence |
| DisciplinaId | INT | → Disciplina | — | ✓ | NÃO | Disciplina medida |
| TotalRespostas | INT | — | — | — | NÃO | Total de questões respondidas |
| TotalAcertos | INT | — | — | — | NÃO | Total de acertos na disciplina |
| Percentual | DECIMAL(5,2) | — | — | — | SIM | Percentual de acertos |
| UltimaAtualizacao | DATETIME | — | — | — | SIM | Data da última atualização do registro |

---

# Legenda

| Símbolo / Tipo | Descrição |
|---|---|
| PK | Primary Key — Chave primária que identifica unicamente cada registro da tabela |
| FK | Foreign Key — Chave estrangeira que referencia a chave primária de outra tabela |
| PK + FK | Coluna que atua simultaneamente como chave primária e estrangeira |
| NOT NULL | O campo é obrigatório e não pode conter valor nulo |
| NULL | O campo é opcional e pode conter valor nulo |
| BIT | Tipo booleano: 1 = verdadeiro / 0 = falso |
| DECIMAL(5,2) | Número decimal com até 5 dígitos e 2 casas decimais |
| TEXT | Texto de comprimento variável sem limite fixo |
