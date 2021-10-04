# Orquestrador
Este é o coração do nosso sistema. Ele é o responsável por orquestrar cada transação. Isso é, ele quem é o responsável por debitar e creditar no serviço de conta. Enviar os dados para pagar o boleto, enviar mensagens no kafka e tudo mais. 

Toda requisição que ele recebe passa pelo BFF (camada que se comunica com a internet e realiza a autenticação e autorização). 

O **Orquestrador** então delega as operações para cada serviço. Ou seja, basta que ele conheça um serviço financeiro para que possamos fazer uso dele. 


As tarefas do Orquestrador são baseadas nas tarefas do serviço. Ou seja, para realizar um depósito a operação deve passar pelo orquestrator que registra a operação e envia o envento da transação para o Kafka.
