# Cadastro de cupom de desconto

## Necessidades
A cdc pode liberar cupons de desconto com valores e validade variados. Precisamos ter suporte a isso.
Todo cupom tem:
- Código para ser entendido por pessoas
- Percentual de desconto
- Validade para ser associado a uma compra

## Restrições
- Código é obrigatório
- Código é único
- Percentual é obrigatório e positivo
- Validade é no futuro

## Resultado esperado
- Status 400 e json de erros em caso de falha de validação
- Status 200 e cupom gerado