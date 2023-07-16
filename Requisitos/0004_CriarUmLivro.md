# Criar um novo livro

## Necessidades
- título
- Resumo do que vai ser encontrado no livro
- Sumário de tamanho livre. O texto deve entrar no formato markdown, que é uma string. Dessa forma ele pode ser formatado depois da maneira apropriada.
- Preço do livro
- Número de páginas
- Isbn(identificador do livro)
- Data que ele deve entrar no ar(de publicação)
- Livro pertence a uma categoria
- Livro é de um autor

## Restrições
- Título é obrigatório
- Título é único
- Resumo é obrigatório e tem no máximo 500 caracteres
- Sumário é de tamanho livre.
- Preço é obrigatório e o mínimo é de 20
- Número de páginas é obrigatória e o mínimo é de 100
- Isbn é obrigatório, formato livre
- Isbn é único
- Data que vai entrar no ar precisa ser no futuro
- A categoria não pode ser nula
- O autor não pode ser nulo

## Resultado esperado
- Um novo livro precisa ser criado e status 200 retornado
- Caso alguma restrição não seja atendida, retorne 400 e um json informando os problemas de validação