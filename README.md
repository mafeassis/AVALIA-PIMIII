<h1 align="center">
  <img src="./docs/assets/AVALIA +.svg" alt="Avalia+" width="300"/>
</h1>

<p align="center">
  <b>Plataforma web de avaliação acadêmica para estudantes do ensino superior</b><br/>
  PIM III – Projeto Integrado Multidisciplinar | ADS – UNIP 2026-1
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow?style=flat-square"/>
  <img src="https://img.shields.io/badge/Linguagem-C%23-239120?style=flat-square&logo=csharp"/>
  <img src="https://img.shields.io/badge/Metodologia-Scrum-0052CC?style=flat-square"/>
</p>

---

## 📌 Descrição do Desafio

Estudantes do ensino superior enfrentam dificuldades na preparação para avaliações acadêmicas por falta de ferramentas acessíveis e direcionadas. O **Avalia+** surge para resolver esse problema, oferecendo uma plataforma web onde alunos podem realizar simulados gerados automaticamente a partir de um banco de questões, acompanhar seu desempenho e identificar pontos de melhoria — tudo de forma gratuita e intuitiva.

---

## 📋 Backlog de Produto

| ID | Funcionalidade | Prioridade | Status |
|----|---------------|------------|--------|
| PB01 | Autenticação de usuários (login por e-mail e senha) | 🔴 Alta | 🔲 A fazer |
| PB02 | Cadastro e gerenciamento de usuários (Aluno, Professor, Admin) | 🔴 Alta | 🔲 A fazer |
| PB03 | Gerenciamento de questões (cadastro, edição, exclusão) | 🔴 Alta | 🔲 A fazer |
| PB04 | Geração automática de simulados | 🔴 Alta | ✅ Concluído |
| PB05 | Realização de simulados | 🔴 Alta | ✅ Concluído |
| PB06 | Correção automática de simulados | 🔴 Alta | ✅ Concluído |
| PB07 | Histórico de simulados realizados | 🟡 Média | 🔲 A fazer |
| PB08 | Relatórios de desempenho individual e por turma | 🟡 Média | 🔲 A fazer |
| PB09 | Dashboards de desempenho | 🟡 Média | ✅ Concluído |
| PB10 | Controle de permissões por perfil de usuário | 🔴 Alta | 🔲 A fazer |

---

## 🗓️ Cronograma de Sprints

```
Sprint 1 ──────────────────────────────── ✅ Concluída
  Estrutura inicial, documentação e requisitos

Sprint 2 ──────────────────────────────── ✅ Concluída
  Modelagem do sistema (diagramas UML, MER, DER)

Sprint 3 ──────────────────────────────── ✅ Concluída
  Desenvolvimento das funcionalidades principais

Sprint 4 ──────────────────────────────── 🔄 Em andamento
  Análise, resultados e finalização da documentação
```

---

## 📅 Tabela de Sprints

| Sprint | Período | Documentação | Vídeo de Entrega |
|--------|---------|-------------|-----------------|
| Sprint 1 | Mar/2026 | [📄 Ver docs](./scrum/sprint-planning/sprint-1-planning.md) | 🔗 Em breve |
| Sprint 2 | Abr/2026 | [📄 Ver docs](./scrum/sprint-planning/sprint-2-planning.md) | 🔗 Em breve |
| Sprint 3 | Abr/2026 | [📄 Ver docs](./scrum/sprint-planning/sprint-3-planning.md) | 🔗 Em breve |
| Sprint 4 | Mai/2026 | [📄 Ver docs](./scrum/sprint-planning/sprint-4-planning.md) | 🔗 Em breve |

---

## 🛠️ Tecnologias Utilizadas

| Camada | Tecnologia |
|--------|-----------|
| Backend | C# |
| Banco de Dados | SQL Server |
| Frontend | HTML, CSS, JavaScript |
| Metodologia | Scrum |
| Versionamento | Git + GitHub |
| Gerenciamento | Trello |

---

## 📁 Estrutura do Projeto

```
avalia-plus/
│
├── 📁 diagramas/
│   ├── 📁 banco-de-dados/       # MER, DER, Dicionário de Dados
│   ├── 📁 fluxo-de-usuario/     # Fluxos por perfil (Aluno, Prof, Admin)
│   └── 📁 uml/                  # Casos de Uso, Classes, Sequência
│
├── 📁 docs/                     # Documentação técnica do PIM
│
├── 📁 scrum/
│   ├── 📁 backlog/              # Backlog consolidado
│   ├── 📁 product-backlog/      # Product Backlog detalhado
│   ├── 📁 sprint-backlog/       # Backlogs por sprint
│   ├── 📁 sprint-planning/      # Planejamentos de sprint
│   ├── 📁 sprint-retrospective/ # Retrospectivas
│   ├── 📁 sprint-review/        # Reviews de entrega
│   └── 📁 dailys/               # Registros das dailys por sprint
│
└── 📄 README.md
```

---

## ▶️ Como Executar o Projeto

> ⚠️ O sistema está em desenvolvimento. As instruções de execução serão atualizadas conforme o progresso do projeto.

```bash
# Clone o repositório
git clone https://github.com/SEU_USUARIO/avalia-plus.git

# Acesse a pasta do projeto
cd avalia-plus

# Em breve: instruções de build e execução do backend em C#
```

---

## 📂 Documentação Completa

Acesse a pasta [`/docs`](./docs/) para consultar toda a documentação técnica do projeto, incluindo:

- Requisitos do sistema
- Regras de negócio
- Escopo do projeto
- Tipos de usuários
- Metodologia de desenvolvimento (Scrum)
- Documento de gerenciamento de backlogs

---

## 👥 Equipe

<table align="center">
  <tr>
    <td align="center">
      <img src="./docs/assets/Gabriel.jpeg" width="120px" style="border-radius: 50%;" alt="Gabriel"/><br/>
      <b>Gabriel Vinicius Rosa Pereira</b><br/>
      Desenvolvedor Frontend<br/>
      <sub>HTML · CSS · JavaScript</sub><br/><br/>
      <a href="https://github.com/GabrielVRosa">GitHub</a> · <a href="https://www.linkedin.com/in/gabriel-vinicius-6a6059352/">LinkedIn</a>
    </td>
    <td align="center">
      <img src="./docs/assets/Isabella.jpeg" width="120px" style="border-radius: 50%;" alt="Isabella"/><br/>
      <b>Isabella Santos Leal</b><br/>
      Scrum Master · Banco de Dados · Protótipo<br/>
      <sub>SQL Server · Figma</sub><br/><br/>
      <a href="https://github.com/IsabellaLeal06">GitHub</a> · <a href="https://www.linkedin.com/in/isabella-santos-1148b02b9/">LinkedIn</a>
    </td>
    <td align="center">
      <img src="./docs/assets/Leticia.jpeg" width="120px" style="border-radius: 50%;" alt="Letícia"/><br/>
      <b>Letícia Aparecida Santos Mota</b><br/>
      Desenvolvedora Backend<br/>
      <sub>C# · Diagrama de Classes</sub><br/><br/>
      <a href="https://github.com/Jmclemota">GitHub</a> · <a href="https://www.linkedin.com/in/let%C3%ADcia-aparecida-a465b7313/">LinkedIn</a>
    </td>
    <td align="center">
      <img src="./docs/assets/Maria.jpeg" width="120px" style="border-radius: 50%;" alt="Maria Fernanda"/><br/>
      <b>Maria Fernanda de Assis</b><br/>
      Product Owner · Documentação · Diagramas UML<br/>
      <sub>UML · Casos de Uso · Sequência</sub><br/><br/>
      <a href="https://github.com/mafeassis">GitHub</a> · <a href="https://www.linkedin.com/in/maria-fernanda-de-assis-1a1414252/">LinkedIn</a>
    </td>
  </tr>
</table>

---


<p align="center">
  Desenvolvido com 💙 pela equipe Avalia+ · PIM III · UNIP 2026-1
</p>
