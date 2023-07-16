# Detalhes de uma compra

## Necessidades
Agora é preciso retornar todos os dados necessários para que a pessoa visualize os dados da compra dela. Para confirmar que tudo está certinho.
Caso tenha cupom aplicado, além do valor original da compra é necessário mostrar o valor final com o cupom aplicado.
O endpoint recebe apenas o id gerado pela compra.

## Resultado esperado
- Status 200 e json de detalhes de uma compra
 - Sempre teremos dois campos no json de saída: Um campo informando se existe o cupom e outro informando o valor da compra com o possível cupom aplicado. Caso não tenha cupom, os valores dos campos devem ser false e null respectivamente. 