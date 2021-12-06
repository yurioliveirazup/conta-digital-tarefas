# Pagando um boleto

## Necessidades

Para pagar um boleto é necessário receber o valor a ser pago e o código de barras do boleto. 

## Restrições

- Só pode ser efetuado o pagamento quando o saldo for maior ou igual ao valor
- O valor mínimo de cada pagamento deve ser maior que zero
- Caso o sistema do banco esteja fora do ar, o boleto deve ter um status "**AGUARDANDO_PAGAMENTO**" e deve tentar ser pago novamente em até 5 minutos. Caso não consiga pagar, a operação deve ser anulada e um email deve ser enviado ao cliente
   
## Resultado Esperado
- Em caso de sucesso:
   - Devolver um status de sucesso (2xx) 
   - Debitar o valor da conta
   - A pessoa deve receber um email com a transação feita
   - O Extrato deve ser atualizado com a nova transação

- Em caso de falha:
   - Retornar um status **422** com a mensagem de erro caso o saldo não seja suficiente
   - Retornar um status **5xx** caso o serviço da operadora esteja indisponível

## Pontos de atenção
- É importante notar quantos serviços estão envolvidos nessa operação
- Qual o melhor lugar para deixar a lógica de verificação de saldo?
