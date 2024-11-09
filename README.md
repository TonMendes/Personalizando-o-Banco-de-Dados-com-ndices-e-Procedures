# Projeto de Otimização de Consultas com Índices

Este projeto foi desenvolvido para otimizar as consultas em um banco de dados fictício de uma empresa, utilizando índices adequados para melhorar a performance nas operações de busca e agrupamento.

## Índices Criados

1. **Índice `idx_department` na tabela `employees`**:
   - **Motivo**: Melhorar a performance da consulta que retorna o departamento com o maior número de pessoas.
   - **Tipo de Índice**: Índice simples na coluna `department`.
   
2. **Índice `idx_city_department` na tabela `employees`**:
   - **Motivo**: Melhorar a performance da consulta que retorna departamentos por cidade, realizando um agrupamento por `city` e `department`.
   - **Tipo de Índice**: Índice composto nas colunas `city` e `department`.
   
3. **Índice `idx_department_name` na tabela `employees`**:
   - **Motivo**: A consulta que retorna a relação de empregados por departamento se beneficia de um índice composto, melhorando a ordenação e recuperação de dados.
   - **Tipo de Índice**: Índice composto nas colunas `department` e `employee_name`.

## Considerações

- Os índices foram criados levando em consideração os campos mais utilizados nas consultas SQL.
- A escolha dos índices visa reduzir o tempo de execução das consultas e garantir a eficiência na busca e agrupamento de dados.
