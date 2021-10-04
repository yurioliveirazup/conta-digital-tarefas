# Email

O serviço de email é, basicamente, um serviço de notificação. A sua função é ficar escutando um tópico no _Kafka_ para saber quais as transações que aconteceram e enviar um email para as pessoas que são donas das contas.

A tarefa para esse serviço é basicamente a seguinte:
- 1. [Enviando um email com a transação](./tarefas/01_enviar_email.md)