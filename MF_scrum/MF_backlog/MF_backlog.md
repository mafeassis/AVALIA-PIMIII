# MF_Gerenciamento de Backlogs – Projeto Avalia+

## Descrição

Esta pasta reúne toda a documentação relacionada ao gerenciamento de Backlogs do projeto **Avalia+**, utilizando a metodologia ágil Scrum para organização, priorização e acompanhamento das atividades do sistema e da documentação acadêmica do PIM III.

O gerenciamento de Backlogs permite estruturar tanto o desenvolvimento técnico da plataforma quanto as entregas acadêmicas exigidas no projeto.

---

# Estrutura do Documento

## 1. Introdução

Apresenta a proposta do gerenciamento de Backlogs no projeto Avalia+, incluindo a organização das atividades relacionadas ao desenvolvimento do sistema, modelagem, diagramas e documentação técnica.

---

## 2. Backlogs no Scrum

O projeto utiliza os principais Backlogs do framework Scrum:

### Product Backlog
Lista contendo todas as funcionalidades, melhorias e atividades previstas para o desenvolvimento da plataforma.

### Sprint Backlog
Conjunto de atividades selecionadas para execução durante cada Sprint.

---

# Product Backlog do Projeto Avalia+

O Product Backlog foi dividido em três categorias principais:

- Funcionalidades do sistema
- Modelagem e diagramas
- Documentação do projeto

Essa divisão permite melhor organização e controle das atividades desenvolvidas ao longo das sprints.

---

# 1. Funcionalidades do Sistema

Esses itens representam as funcionalidades principais da plataforma Avalia+.

| ID | Funcionalidade | Descrição | Prioridade |
|---|---|---|---|
| PB01 | Autenticação de usuários | Permitir login utilizando e-mail e senha | Alta |
| PB02 | Cadastro de usuários | Gerenciamento de usuários (Aluno, Professor e Administrador) | Alta |
| PB03 | Gerenciamento de questões | Cadastro, edição e exclusão de questões por disciplina | Alta |
| PB04 | Gerenciamento de disciplinas | Cadastro, edição e exclusão de disciplinas | Alta |
| PB05 | Gerenciamento de turmas | Criação, edição, exclusão e vinculação de professores e alunos | Alta |
| PB06 | Geração automática de simulados | Gerar simulados automáticos com quantidade configurável de questões | Alta |
| PB07 | Realização de simulados | Permitir realização de simulados online | Alta |
| PB08 | Correção automática | Correção automática após finalização | Alta |
| PB09 | Histórico de simulados | Armazenamento de simulados realizados | Média |
| PB10 | Dashboard de desempenho por turma | Indicadores de desempenho para professores | Média |
| PB11 | Painel de indicadores administrativos | Indicadores gerais da plataforma | Média |
| PB12 | Controle de permissões | Restrição de acesso conforme perfil do usuário | Alta |

---

# 2. Modelagem e Diagramas do Sistema

Essas atividades representam a modelagem estrutural e funcional da plataforma.

| ID | Atividade | Descrição | Prioridade |
|---|---|---|---|
| MD01 | Diagrama de Casos de Uso | Representação das interações do sistema | Alta |
| MD02 | Diagrama de Classes | Modelagem das entidades e relacionamentos do sistema (backend C#) | Alta |
| MD03 | Diagrama de Sequência | Fluxo de execução das funcionalidades | Média |
| MD04 | Fluxo de Usuário | Navegação dos usuários na plataforma | Alta |
| MD05 | Modelo Conceitual (MER) | Estrutura conceitual do banco de dados | Alta |
| MD06 | Modelo Lógico | Estrutura lógica das tabelas | Alta |
| MD07 | Diagrama Entidade-Relacionamento (DER) | Representação gráfica do banco de dados | Alta |
| MD08 | Dicionário de Dados | Documentação das tabelas e atributos | Média |

Essas atividades garantem organização e padronização da estrutura do sistema.

---

# 3. Documentação do Projeto

Essas atividades correspondem à elaboração da documentação acadêmica do PIM III.

| ID | Atividade | Descrição | Prioridade |
|---|---|---|---|
| DOC01 | Introdução do projeto | Apresentação geral da proposta | Alta |
| DOC02 | Descrição do problema | Problema que o sistema pretende solucionar | Alta |
| DOC03 | Objetivos do sistema | Objetivos gerais e específicos | Alta |
| DOC04 | Público-alvo | Identificação dos usuários da plataforma | Média |
| DOC05 | Requisitos do sistema | Requisitos funcionais e não funcionais | Alta |
| DOC06 | Arquitetura do sistema | Tecnologias e estrutura da solução | Média |
| DOC07 | Modelagem do sistema | Diagramas e modelagem UML | Alta |
| DOC08 | Metodologia de desenvolvimento | Aplicação do Scrum | Alta |
| DOC09 | Planejamento de Sprints | Organização das atividades por sprint | Alta |
| DOC10 | Conclusão do projeto | Resultados e considerações finais | Média |

---

# Planejamento das Sprints

## Sprint 1 – Estrutura Inicial do Projeto

### Objetivo
Definir a base do sistema e iniciar a documentação do projeto.

### Atividades
- Configuração do ambiente de desenvolvimento
- Criação do repositório do projeto
- Levantamento de requisitos
- Definição dos tipos de usuários
- Criação do Product Backlog
- Início da modelagem do banco de dados

---

## Sprint 2 – Modelagem do Sistema

### Objetivo
Desenvolver a modelagem estrutural e conceitual da plataforma.

### Atividades
- Diagrama de Casos de Uso
- Diagrama de Classes
- Fluxo de Usuário
- MER e DER
- Dicionário de Dados
- Revisão dos requisitos
- Documentação da arquitetura

---

## Sprint 3 – Desenvolvimento Inicial da Plataforma

### Objetivo
Desenvolver a estrutura inicial da plataforma e das funcionalidades principais do sistema.

### Atividades
- Implementação do sistema de login
- Cadastro e gerenciamento de usuários
- Gerenciamento de disciplinas e turmas
- Estruturação inicial do banco de questões
- Desenvolvimento das primeiras interfaces da plataforma
- Integração inicial entre frontend e banco de dados

---

## Sprint 4 – Ajustes e Finalização da Documentação

### Objetivo
Realizar ajustes finais na plataforma e concluir a documentação do projeto.

### Atividades
- Ajustes no frontend da aplicação
- Refinamento das interfaces do sistema
- Continuação da integração das funcionalidades
- Validação da modelagem do sistema
- Revisão da documentação do projeto
- Organização final das entregas do PIM III

---

# Estrutura de Organização no Trello

O quadro do Trello foi organizado com as seguintes listas:

| Lista | Descrição |
|---|---|
| Product Backlog | Funcionalidades e atividades gerais |
| Sprint 1 | Estrutura inicial do projeto |
| Sprint 2 | Modelagem e diagramas |
| Sprint 3 | Desenvolvimento inicial da plataforma |
| Sprint 4 | Ajustes finais e documentação |
| Em Desenvolvimento | Atividades em execução |
| Em Revisão | Atividades em validação |
| Concluído | Atividades finalizadas |

---

# Benefícios da Utilização de Backlogs

A utilização de Backlogs no projeto Avalia+ proporciona:

- organização das atividades;
- definição clara de prioridades;
- acompanhamento do progresso;
- transparência no desenvolvimento;
- melhor planejamento das entregas.

Além disso, o uso do Trello auxilia no controle visual das tarefas e no acompanhamento das atividades realizadas pela equipe.
