# Máximos e mínimos
* valores máximos e minimos de alguma coluna da tabela
```sql
    --Produto mais caro
    SELECT 
        MAX(Preco) AS PrecoMaximo
    FROM Produtos
    
    --Produto mais caro tamanho M
    SELECT 
        MAX(Preco) AS PrecoMaximoM
    FROM Produtos 
    WHERE Tamanho = 'M'

    --Produto mais barato tamanho M
    SELECT 
        MIN(Preco) AS PrecoMinimo
    FROM Produtos 

    --Produto mais barato tamanho M
    SELECT 
        MIN(Preco) AS PrecoMinimoM
    FROM Produtos 
    WHERE Tamanho = 'M'

    --média
        --Produto mais barato tamanho M
    SELECT 
        AVG(Preco) AS MediaPreco
    FROM Produtos 

```