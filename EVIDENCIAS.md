# Evidências de execução — testes de API

A coleção foi validada contra JSONPlaceholder em 13/10/2026 antes da entrega.

| Métrica | Resultado |
|---|---:|
| Requisições executadas | 4 |
| Requisições com falha | 0 |
| Assertions aprovadas | 8 |
| Assertions com falha | 0 |

Os resultados esperados foram observados: listagem HTTP 200, detalhe HTTP 200, recurso inexistente HTTP 404 e POST simulado HTTP 201 com dados ecoados na resposta.

A entrega não inclui Newman nem dependências Node: basta importar a coleção e o ambiente no Postman. Newman foi usado apenas na validação preparatória; durante a inspeção de dependências apareceram alertas de segurança no conjunto do Newman, então a dependência foi removida do pacote. Isso não afeta a coleção Postman nem o uso pelo Postman Runner.
