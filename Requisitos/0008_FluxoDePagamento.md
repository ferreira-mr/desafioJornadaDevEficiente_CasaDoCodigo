# Começo do fluxo de pagamento

## Necessidades - Fluxo 01
Uma coisa importante. Na cdc, você não faz um cadastro e tem suas compras associadas. Toda vez você coloca seu email, cpf/cnpj etc. Como isso vai ser implementado depende da aplicação.

Os seguintes campos precisam ser preenchidos:
- Email
- Nome
- Aobrenome
- Documento(cpf/cnpj)
- Endereco
- Complemento
- Cidade
- Pais
- Estado(caso aquele pais tenha estado)
- Telefone
- Cep
- Receber também o parâmetro relativo ao carrinho de compras no formulário final. O json montado pelo cliente relativo ao carrinho tem o seguinte formato:
```json
{
  "total": decimal,
  "itens":[
     {
      "idLivro":number,
      "quantidade": "number"
    },
     {
      "idLivro":number,
      "quantidade": number
    }
  ]
}

```

## Restrições
- Email obrigatório e com formato adequado
- Nome obrigatório
- Sobrenome obrigatório
- Documento(cpf/cnpj) obrigatório e só precisa ser um cpf ou cnpj
- Endereco obrigatório
- Complemento obrigatório
- Cidade obrigatório
- País obrigatório
- Se o país tiver estados, um estado precisa ser selecionado
- Estado(caso aquele pais tenha estado) - apenas se o país tiver cadastro de estados
- Telefone obrigatório
- Cep é obrigatório
- O total é não nulo
- O total é maior que zero
- Tem pelo menos um item no carrinho
- IdLivro é obrigatório e precisa existir
- Quantidade é obrigatória
- Quantidade é maior que zero
- O total calculado no servidor precisa ser igual ao total enviado

## Resultado esperado
- Compra gerada com um status de iniciada
- Status 201 gerado com o endereço de detalhe da compra