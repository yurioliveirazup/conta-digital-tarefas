# Registrando uma transação

## Necessidades

Toda transação deve ser registrada para fins de auditoria. Essas informações chegam na nossa API através do Kafka em um tópico chamado `transacoes`. Basicamente, é enviado um JSON com as seguintes informações:

- Operação
- Valor dessa operação
- Data da transação
- Cliente que efetuou a transação
- Conta participante
   
## Resultado Esperado

- Todos os dados devem estar disponíveis no banco de dados para serem consultados em um futuro.

