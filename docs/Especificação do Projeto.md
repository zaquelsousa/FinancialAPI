## Objetivo do projeto
Essa API permite o controle financeiro pessoal de forma simples e organizada, oferecendo cadastro de movimentaçoes, relatorio, metas e controle recorrente de despesas.

## Personas
Desenvolvedor front-end (Maria, 22 anos, estagiária): precisa de endpoints claros e dados bem estruturados pra fazer um app mobile.<br>
Desenvolvedor front-end (Pedro, 19 anos, Dev junior): precisa de endpoints seguros para usar em seu web app.

## Histórias de Usuário

Como desenvolvedor front-end, quero acessar um endpoint que retorne as metas por categoria para exibir no dashboard.

## Requisitos Funcionais

| Código  | Descrição |
|---------|-----------|
| **RF01** | O sistema deve permitir o cadastro e gerenciamento de usuários, informando nome, email e senha (armazenada de forma segura com hash). |
| **RF02** | O sistema deve permitir que o usuário se autentifique utilizando email e senha. |
| **RF03** | O sistema deve garantir que cada usuário tenha acesso apenas aos seus próprios dados financeiros, metas e categorias. |
| **RF04** | O sistema deve permitir que o usuário cadastre, edite e remova categorias financeiras. |
| **RF05** | O sistema deve permitir que o usuário cadastre movimentações financeiras com os seguintes campos: descrição, valor, data, tipo (entrada ou saída), categoria e repetição (opcional). |
| **RF06** | O sistema deve permitir que o usuário visualize a lista de movimentações financeiras cadastradas, com filtros por data, tipo e categoria. |
| **RF07** | O sistema deve permitir o cadastro de movimentações recorrentes com frequência, próxima execução, status, tipo, valor, descrição, categoria e data padrão de execução. |
| **RF08** | O sistema deve gerar automaticamente novas movimentações com base nas configurações de repetição ativas, na data definida. |
| **RF09** | O sistema deve permitir o cadastro de metas financeiras com descrição, categoria vinculada, valor objetivo, data limite, status de atingido e usuário vinculado. |
| **RF10** | O sistema deve monitorar o progresso das metas financeiras e atualizar o campo de status (atingido) automaticamente quando o valor objetivo for atingido. |
| **RF11** | O sistema deve permitir a criação de objetivos financeiros contendo nome, valor meta, valor atual, prazo, status de atingido e usuário vinculado. |
| **RF12** | O sistema deve notificar o usuário quando uma meta ou objetivo financeiro estiver próxima de ser atingida ou quando for atingida. |
| **RF13** | O sistema deve apresentar relatórios sobre saldo total, saldo mensal, gastos por categoria e entradas/saídas agrupadas por período. |

## Requisitos Não Funcionais

| Código   | Descrição |
|----------|-----------|
| **RNF01** | O sistema deve utilizar um banco de dados na nuvem (ex: Azure SQL ou MySQL na Azure) para persistência dos dados. |
| **RNF02** | A API deve exigir autenticação via token JWT. As senhas dos usuários devem ser armazenadas com hash seguro (bcrypt). Todas as rotas devem ser protegidas por autenticação, exceto login e cadastro. |
| **RNF03** | Todas as requisições entre o frontend e a API devem ser feitas via HTTPS. |

## Diagrama de caso de uso
![Diagrama de caso de uso](<imagens/caso de uso fanancas pessoais.drawio.png>)
## Restrições

| Código   | Descrição |
|----------|-----------|
| **RT01** | A API será desenvolvida utilizando .NET 8. |
| **RT02** | O banco de dados será SQL Server. |
| **RT03** | O deploy será feito exclusivamente na Azure. |
| **RT04** | A API não terá frontend, apenas endpoints documentados via Swagger. |