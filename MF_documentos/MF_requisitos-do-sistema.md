# ⚙️ MF_Requisitos do Sistema – Avalia+

--- 

## 1. Requisitos Funcionais

Os requisitos funcionais descrevem os serviços e comportamentos que o sistema deve fornecer aos usuários, conforme as necessidades do negócio e as interações previstas na plataforma.

---

### RF01 – Autenticação de Usuários

O sistema deve permitir que usuários realizem autenticação por meio de **e-mail e senha**, concedendo acesso às funcionalidades conforme o perfil de usuário (Aluno, Professor ou Administrador).

---

### RF02 – Gerenciamento de Usuários

O sistema deve permitir que o Administrador realize o gerenciamento de usuários, incluindo **cadastro, edição e exclusão** de contas no sistema.

---

### RF03 – Gerenciamento de Questões

O sistema deve permitir que o Administrador **cadastre, edite e exclua** questões no banco de dados, organizadas por disciplina.

---

### RF04 – Gerenciamento de Disciplinas

O sistema deve permitir que o Administrador **cadastre, edite e exclua disciplinas**, às quais as questões do banco de dados estarão vinculadas.

---

### RF05 – Gerenciamento de Turmas

O sistema deve permitir que o Administrador **cadastre, edite e exclua turmas**, realizando a vinculação de professores e alunos a cada turma.

---

### RF06 – Geração de Simulados

Permite ao aluno gerar automaticamente um simulado com **10, 15 ou 20 questões**, selecionadas aleatoriamente a partir do banco de questões do sistema. As questões podem ser de diferentes disciplinas e níveis de dificuldade variados, sem restrição de categoria.

---

### RF07 – Realização de Simulados

Permite ao aluno responder um simulado online, visualizando as questões e selecionando as alternativas de resposta, com **registro das respostas** ao longo da realização da atividade.

---

### RF08 – Correção Automática

O sistema deve **corrigir automaticamente** os simulados após sua finalização pelo aluno, apresentando o resultado imediato.

---

### RF09 – Visualização de Desempenho do Aluno

O sistema deve permitir que o aluno visualize seu **desempenho individual** nos simulados realizados, incluindo histórico de resultados e indicadores de acertos.

---

### RF10 – Dashboard de Desempenho por Turma

O sistema deve permitir que **professores** visualizem indicadores de desempenho dos alunos de suas turmas por meio de dashboards, incluindo resultados individuais e gerais dos simulados realizados.

---

### RF11 – Painel de Indicadores Administrativos

O sistema deve disponibilizar ao **Administrador** um painel com indicadores gerais da plataforma, incluindo:

- Média de acertos por turma
- Quantidade de questões cadastradas no banco
- Quantidade de usuários cadastrados por perfil
- Quantidade de simulados realizados

---

### RF12 – Visualização de Perfil do Usuário

O sistema deve permitir que o usuário visualize suas **informações de perfil**, incluindo dados básicos da conta como nome e e-mail. O acesso deve respeitar o controle baseado em perfis, garantindo que cada usuário visualize apenas seus próprios dados.

---

## 2. Requisitos Não Funcionais

Os requisitos não funcionais descrevem as características de qualidade do sistema, incluindo aspectos de segurança, desempenho e usabilidade. 

---

### RNF01 – Segurança de Acesso

O sistema deve garantir autenticação segura por meio de **controle de acesso baseado em perfis de usuário**, assegurando que cada usuário acesse apenas as funcionalidades autorizadas.
*(Alinhado às práticas de controle de acesso da ISO/IEC 27001.)*

---

### RNF02 – Proteção das Informações

O sistema deve garantir a **proteção das informações** armazenadas no banco de dados, assegurando confidencialidade e integridade dos dados dos usuários.
*(Conforme princípios de segurança da informação da ISO/IEC 27001.)*

---

### RNF03 – Responsividade

O sistema deve possuir **interface responsiva**, permitindo acesso adequado em diferentes resoluções de tela, como desktop e notebook.

---

### RNF04 – Usabilidade

A interface do sistema deve ser projetada de forma **intuitiva**, permitindo que os usuários realizem suas tarefas com eficácia, eficiência e satisfação.
*(Alinhado aos princípios de usabilidade definidos pela ISO 9241-11.)*

---

### RNF05 – Integridade dos Dados

O banco de dados deve garantir **consistência e integridade** das informações armazenadas, evitando perda ou alteração indevida de dados.

---

### RNF06 – Manutenibilidade

O sistema deve possuir **organização modular de código** e documentação adequada, facilitando manutenção, evolução e correção de erros.
*(Alinhado às práticas de desenvolvimento previstas na ISO/IEC 12207.)*
