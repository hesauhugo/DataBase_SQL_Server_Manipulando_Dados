# contar mediante uma determinada condição
```sql
    -- CONTANDO SEM NOMEAR
    SELECT COUNT(*) FROM Produtos
    -- CONTANDO NOMEANDO
    SELECT COUNT(*) AS QuantidadeProdutos FROM Produtos
    -- CONTANDO COM WHERE
    SELECT COUNT(*) AS QuantidadeProdutosTamanhoM FROM Produtos WHERE Tamanho = 'M'
´´´
