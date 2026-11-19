# Testes de API com Postman: Kits de Produtos

Testes do endpoint `/api/v1/kits/:id/products` de um aplicativo de pedidos.

## Objetivo
Verificar se a API aceita entradas válidas e rejeita entradas inválidas com o código HTTP correto.

## Resultado
- 20 casos de teste, desenhados com classes de equivalência e valores limite.
- 11 bugs registrados no Jira.
- Padrão encontrado: a API retorna 500 (erro do servidor) ou 200 quando deveria retornar 400 (requisição inválida), em casos como letras ou símbolos no `id` e na `quantity`, campos vazios ou ausentes, lista de produtos vazia e corpo da requisição vazio.

## Ferramentas utilizadas
Postman, JSON, Jira.

## O que aprendi
- Escolher dados de teste com classes de equivalência e valores limite.
- Conferir não só o status HTTP, mas também se o erro corresponde ao tipo de problema.
- Documentar cada falha com requisição, resultado esperado e resultado real.

## Melhorias possíveis
- Automatizar a coleção com scripts de teste do Postman.
- Cobrir também os endpoints de criação e exclusão de kits.

## Documentação
[Planilha com os casos de teste](https://docs.google.com/spreadsheets/d/1gcO2OzskBA80sH3rPQleONSNsfzfBnP5/edit?usp=sharing)
