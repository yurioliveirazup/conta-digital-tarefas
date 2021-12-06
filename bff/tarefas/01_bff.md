# BFF - Comunicação

## Necessidades

Precisamos fazer com que, para cada operação do orquestrador, o BFF se comunique repassando os dados da request
   
## Resultado Esperado
- Em caso de sucesso:
   - Devolver um status de sucesso (2xx) retornado pelo Orquestrador


- Em caso de falha:
  - Retornar o status de falha com as mensagem, caso essa esteja nas faixas **4xx**
  - Retornar um status **500** com uma mensagem mais genérica caso outro erro de servidor acontecer

