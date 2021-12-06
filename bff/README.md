# BFF

BFF ([back-end for front-end](https://samnewman.io/patterns/architectural/bff/)) é um padrão de projetos que podemos dizer é uma especialização de um [API Gateway](https://microservices.io/patterns/apigateway.html).

A ideia é que para cada tipo de aplicação Front-end (mobile, web, desktop) exista um serviço específico para realizar essa comunicação.

Na nossa arquitetura, esse aplicação fica na camada da internet recebendo as requisições do mundo mobile e repassando para o orquestrador. 

É nessa camada que toda a autenticação será feita. Dessa forma, quando as chamadas chegarem ao orquestrador elas já vão estar autenticadas e, se possível, autorizadas.

Sabendo disso, vamos as tarefas:

Sabendo disso, vamos as tarefas:

1. [Se comunicando com orquestrador](./tarefas/01_bff.md)
1. [Criando estrutura de autenticação](./tarefas/02_bff.md)