# BFF - Segurança

## Necessidades

Precisamos implementar a parte de segurança no BFF para que toda requisição esteja autenticada e, se possível, autorizada

## Resultado Esperado
- Em caso de sucesso:
   - Na hora da autenticação:
      - Devolver um token (ou outra forma de validar uma pessoa autenticada)
   - Nas requisições:
      - Liberar requisições para o orquestrador.

- Em caso de falha:
   - Na hora da autenticação:
      - Devolver uma mensagem falando que ou o usuário ou a senha estão incorretas
   - Nas requisições:
      - Devolver status de **403** com a menagem de erro



