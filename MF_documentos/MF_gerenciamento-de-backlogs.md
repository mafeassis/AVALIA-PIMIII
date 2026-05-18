# 📋 MF_Documento de Gerenciamento de Backlogs – Avalia+

---

## 1. Introdução

Este documento apresenta a estrutura de gerenciamento de Backlogs do projeto **Avalia+**, desenvolvido utilizando a metodologia ágil **Scrum**.

O gerenciamento de Backlogs permite organizar, priorizar e acompanhar todas as atividades necessárias para o desenvolvimento da plataforma e para a elaboração da documentação exigida no **Projeto Integrado Multidisciplinar (PIM)**.

Além das funcionalidades da plataforma, também foram incluídas no planejamento atividades relacionadas à:

- Modelagem do sistema
- Produção de diagramas UML
- Modelagem de banco de dados
- Elaboração da documentação técnica do projeto

Dessa forma, o gerenciamento do projeto contempla tanto o desenvolvimento da solução tecnológica quanto a organização das entregas exigidas no trabalho acadêmico.

---

## 2. Backlogs no Scrum

No framework Scrum, o gerenciamento das atividades do projeto é realizado por meio de **Backlogs**, que representam listas organizadas de tarefas e funcionalidades.

**Product Backlog**
Contém todas as funcionalidades, melhorias e atividades necessárias para o desenvolvimento do produto, organizadas por prioridade.

**Sprint Backlog**
Representa o conjunto de tarefas selecionadas do Product Backlog para serem executadas durante uma Sprint. Ao final de cada Sprint deve existir uma entrega funcional do sistema ou avanço significativo na documentação.

---

## 3. Product Backlog do Projeto Avalia+

O Product Backlog foi dividido em três categorias principais: **funcionalidades do sistema**, **modelagem e diagramas** e **documentação do PIM**.

---

### 3.1 Funcionalidades do Sistema

| ID | Funcionalidade | Descrição | Prioridade |
|----|---------------|-----------|------------|
| PB01 | Autenticação de usuários | Permitir login no sistema utilizando e-mail e senha | 🔴 Alta |
| PB02 | Cadastro de usuários | Cadastro e gerenciamento de usuários (Aluno, Professor e Administrador) | 🔴 Alta |
| PB03 | Gerenciamento de questões | Cadastro, edição e exclusão de questões por disciplina | 🔴 Alta |
| PB04 | Gerenciamento de disciplinas | Cadastro, edição e exclusão de disciplinas | 🔴 Alta |
| PB05 | Gerenciamento de turmas | Criação, edição, exclusão e vinculação de professores e alunos | 🔴 Alta |
| PB06 | Geração automática de simulados | Criar simulados com 10, 15 ou 20 questões aleatórias do banco | 🔴 Alta |
| PB07 | Realização de simulados | Permitir que alunos respondam simulados pela plataforma | 🔴 Alta |
| PB08 | Correção automática | Corrigir automaticamente os simulados após finalização | 🔴 Alta |
| PB09 | Histórico de simulados | Armazenar os simulados realizados pelos alunos | 🟡 Média |
| PB10 | Dashboard de desempenho por turma | Indicadores de desempenho para professores | 🟡 Média |
| PB11 | Painel de indicadores administrativos | Visão geral com médias de acertos, questões cadastradas e usuários | 🟡 Média |
| PB12 | Controle de permissões | Restringir funcionalidades de acordo com o perfil do usuário | 🔴 Alta |

---

### 3.2 Backlog de Modelagem do Sistema

| ID | Atividade | Descrição | Prioridade |
|----|-----------|-----------|------------|
| MD01 | Diagrama de Casos de Uso | Representar as interações entre usuários e sistema | 🔴 Alta |
| MD02 | Diagrama de Classes | Modelar entidades, atributos e relacionamentos do sistema (backend C#) | 🔴 Alta |
| MD03 | Diagrama de Sequência | Representar o fluxo de execução das funcionalidades | 🟡 Média |
| MD04 | Fluxo de Usuário (User Flow) | Mapear a navegação dos usuários dentro da plataforma | 🔴 Alta |
| MD05 | Modelo Conceitual do Banco de Dados (MER) | Representar entidades e relacionamentos do banco | 🔴 Alta |
| MD06 | Modelo Lógico do Banco de Dados | Estrutura detalhada das tabelas do sistema | 🔴 Alta |
| MD07 | Diagrama Entidade-Relacionamento (DER) | Representação gráfica do banco de dados | 🔴 Alta |
| MD08 | Dicionário de Dados | Documentação detalhada de tabelas e atributos | 🟡 Média |

---

### 3.3 Backlog de Documentação do PIM

| ID | Atividade | Descrição | Prioridade |
|----|-----------|-----------|------------|
| DOC01 | Introdução do projeto | Apresentação geral da proposta do sistema | 🔴 Alta |
| DOC02 | Descrição do problema | Explicação do problema que o sistema pretende resolver | 🔴 Alta |
| DOC03 | Objetivos do sistema | Definição dos objetivos gerais e específicos | 🔴 Alta |
| DOC04 | Público-alvo | Identificação dos usuários e instituições que utilizarão a plataforma | 🟡 Média |
| DOC05 | Requisitos do sistema | Levantamento de requisitos funcionais e não funcionais | 🔴 Alta |
| DOC06 | Arquitetura do sistema | Descrição das tecnologias utilizadas e arquitetura da solução | 🟡 Média |
| DOC07 | Modelagem do sistema | Inclusão e explicação dos diagramas UML | 🔴 Alta |
| DOC08 | Metodologia de desenvolvimento | Descrição da aplicação da metodologia Scrum | 🔴 Alta |
| DOC09 | Planejamento de Sprints | Organização das atividades do projeto em Sprints | 🔴 Alta |
| DOC10 | Conclusão do projeto | Apresentação dos resultados esperados e considerações finais | 🟡 Média |

---

## 4. Planejamento das Sprints

### Sprint 1 – Estrutura Inicial do Projeto ✅

**Objetivo:** Definir a base do sistema e iniciar a documentação do projeto.

- Configuração do ambiente de desenvolvimento
- Criação do repositório do projeto
- Levantamento de requisitos do sistema
- Elaboração da introdução do projeto
- Definição dos tipos de usuários
- Criação do Product Backlog
- Início da modelagem do banco de dados

---

### Sprint 2 – Modelagem do Sistema ✅

**Objetivo:** Desenvolver a modelagem conceitual e estrutural do sistema.

- Criação do Diagrama de Casos de Uso
- Criação do Diagrama de Classes (representação do backend C#)
- Criação do Fluxo de Usuário
- Criação do MER e DER
- Elaboração do Dicionário de Dados
- Revisão dos requisitos do sistema
- Documentação da arquitetura do sistema

---

### Sprint 3 – Desenvolvimento das Funcionalidades ✅

**Objetivo:** Implementar as funcionalidades principais da plataforma.

- Implementação do sistema de login
- Cadastro e gerenciamento de usuários
- Gerenciamento de disciplinas e turmas
- Implementação do banco de questões
- Geração automática de simulados (10, 15 ou 20 questões)
- Interface para realização de simulados

---

### Sprint 4 – Análise e Resultados 🔄

**Objetivo:** Implementar funcionalidades de análise de desempenho e finalizar a documentação.

- Implementação da correção automática
- Registro do histórico de simulados
- Desenvolvimento do dashboard de desempenho por turma (Professor)
- Implementação do painel de indicadores administrativos (Administrador)
- Finalização da documentação do projeto

---

## 5. Organização no Trello

Para o gerenciamento do projeto Avalia+, o quadro do Trello está organizado com as seguintes listas:

| Lista | Descrição |
|-------|-----------|
| **Product Backlog** | Todas as funcionalidades, modelagem e tarefas de documentação |
| **Sprint 1** | Estrutura inicial do projeto |
| **Sprint 2** | Modelagem e criação de diagramas |
| **Sprint 3** | Implementação das funcionalidades |
| **Sprint 4** | Finalização e documentação |
| **Em Desenvolvimento** | Tarefas sendo executadas pela equipe |
| **Em Revisão** | Tarefas em testes ou revisão |
| **Concluído** | Atividades finalizadas |

---

## 6. Benefícios da Utilização de Backlogs

A utilização de Backlogs no projeto Avalia+ proporciona:

- Organização clara das funcionalidades e tarefas do projeto
- Definição de prioridades de forma transparente
- Acompanhamento contínuo do progresso das atividades
- Melhor planejamento e previsibilidade das entregas
- Maior colaboração e alinhamento entre os membros da equipe
