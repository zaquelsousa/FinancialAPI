## Metodologia

O projeto será desenvolvido utilizando **C#** para o backend e **SQL** como banco de dados relacional. A comunicação entre cliente e servidor será baseada em **requisições HTTPS**, e o **Visual Studio** será a IDE principal utilizada no desenvolvimento. O versionamento será feito com **Git**, com repositório hospedado no **GitHub**.

---

## Processo de Desenvolvimento

Apesar de ser um projeto individual, foi adotada uma abordagem inspirada na **metodologia ágil Scrum**, com foco em **ciclos curtos de entrega** e **validação constante do progresso**.  
Em vez de seguir todas as cerimônias e papéis formais do Scrum (como Scrum Master ou Product Owner), foi feita uma **adaptação simplificada**, priorizando a entrega contínua e a organização das tarefas.

As tarefas foram organizadas em um **quadro kanban no GitHub Projects**, seguindo as etapas:

- **Backlog**: ideias e funcionalidades pendentes  
- **To Do**: tarefas planejadas para a sprint atual  
- **Em andamento**: funcionalidades em desenvolvimento  
- **Revisão/Testes**: validações antes da entrega  
- **Finalizado**: funcionalidades completas  

Essa abordagem permitiu manter o foco, evitar acúmulo de tarefas e facilitar o controle de progresso mesmo sem uma equipe.

---

## Controle de Versão

O versionamento do projeto é feito com **Git**, utilizando **GitHub** como repositório remoto. Foram definidas **convenções para nomeação de branches** e **organização de issues**, com o objetivo de manter o repositório limpo e organizado:

### Branches

- `main`: versão estável e pronta para entrega  
- `testing`: versão em testes  
- `dev`: versão em desenvolvimento ativo 
- `feature/nome-da-feature`: branch específica para desenvolvimento de uma nova funcionalidade  
  - Exemplo: `feature/cadastro-usuario` 

### Issues

As **issues** do projeto seguem **etiquetas padronizadas** para facilitar a triagem e acompanhamento:

- `documentation`: melhorias ou ajustes na documentação  
- `bug`: erro encontrado em alguma funcionalidade  
- `enhancement`: necessidade de melhorar algo já existente  
- `feature`: implementação de novas funcionalidades  
