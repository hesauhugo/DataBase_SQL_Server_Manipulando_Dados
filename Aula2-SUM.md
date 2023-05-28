# Usando sum
* coluna preço
```sql
    --Somando todos produtos
    SELECT 
        SUM(Preco) AS PrecoTotal
    FROM Produtos
    --Somando  produtos tamanho M
    SELECT 
        SUM(Preco) AS PrecoTotalM
    FROM Produtos
    WHERE Tamanho = 'M'
```