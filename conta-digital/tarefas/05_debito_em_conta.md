# Debitando em uma conta

## Necessidades

Sempre que um usuário realiza um pagamento é necessário debitar esse valor de sua conta. 
   
## Restrições

- Só pode ser debitado um valor menor ou igual ao valor do saldo atual da conta.
- O valor a ser debitado precisa ser positivo


## Resultado Esperado

- Em caso de sucesso:
   - Devolver um status de sucesso (2xx)

- Em caso de falha:
   - Retornar um status **422** com a mensagem de erro

## Pontos de atenção
- O que acontece quando duas operações de débito acontecerem ao mesmo tempo?
