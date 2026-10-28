# Testes de API com Postman

Testes da API pública [JSONPlaceholder](https://jsonplaceholder.typicode.com),
criados para praticar validação de APIs com Postman.

## Arquivos
- `Testes reqres.postman_collection.json`: requisições e testes
- `reqres.postman_environment.json`: variável `base_url`

## Como executar
1. No Postman, clique em **Import** e importe os dois arquivos.
2. Selecione o environment no canto superior direito.
3. Clique na collection → **Run** → **Run**.

## O que foi testado

| Funcionalidade | Método | Endpoint | Status esperado |
|----------------|--------|----------|-----------------|
| Cadastro | POST | /users | 201 |
| Busca | GET | /users | 200 |
| Busca | GET | /users/2 | 200 |
| Busca (inexistente) | GET | /users/23 | 404 |
| Atualização | PUT | /users/2 | 200 |
| Exclusão | DELETE | /users/2 | 200 |

## Validações incluídas
- Código de status
- Tempo de resposta menor que 1000 ms
- Campos retornados no corpo da resposta

## Aprendizados
- Organização de collections em pastas
- Uso de variáveis de ambiente
- Cenários positivos e negativos
