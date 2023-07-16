# Cadastro de país e estados do país

## Necessidades
Precisamos de um cadastro simples de países e seus respectivos estados.
Cada país tem um nome e cada estado tem um nome e pertence a um país.

## Restrições
- O nome é obrigatório
- O nome é único

### Restrição para estados
- O nome é obrigatório
- O nome é único
- O país é obrigatório

## Resultado esperado
- Dois endpoints para que seja possível cadastrar países e estados. Pode existir país sem estados associados.
- Caso alguma restrição não seja atendida, retornar 400 e json com os problemas de validação.