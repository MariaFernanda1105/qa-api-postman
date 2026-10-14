# Testes de API — Postman + JSONPlaceholder

Coleção demonstrativa de validação de integrações usando a API pública [JSONPlaceholder](https://jsonplaceholder.typicode.com/). Não há tokens, credenciais ou dependências de Node no pacote.

## Cenários incluídos

| Requisição | Validações principais |
|---|---|
| `GET /posts` | HTTP 200, lista não vazia e campos esperados |
| `GET /posts/1` | HTTP 200 e ID retornado igual a 1 |
| `GET /posts/999` | HTTP 404 para recurso inexistente |
| `POST /posts` | HTTP 201 e dados enviados na resposta |

## Importar e executar no Postman

1. No Postman, escolha **Import**.
2. Importe `postman/qa-api.postman_collection.json` e `postman/jsonplaceholder.postman_environment.json`.
3. Selecione o ambiente **JSONPlaceholder - Público**.
4. Abra a coleção e execute **Run collection**.
5. Confira os testes de cada requisição no resultado da execução.

Os scripts de teste já estão embutidos em cada requisição. Newman é opcional e não é necessário para importar ou usar a coleção.

## Evidência de validação

A coleção foi validada antes da entrega: 4 requisições e 8 assertions aprovadas. Resumo em `EVIDENCIAS.md`.

## Limitação importante

JSONPlaceholder é uma API de demonstração. O `POST /posts` simula a criação e devolve uma resposta `201`, mas **não persiste o novo post**. Os resultados dependem da disponibilidade da API pública e do acesso à internet.
