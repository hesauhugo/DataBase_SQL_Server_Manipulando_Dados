# Entendendo Group by
* quantos tamanhos agrupando por produto
* agrupar dados iguais e contar
```sql 

    SELECT 
        Tamanho,
        COUNT(*) Quantidade

    FROM Produtos
    WHERE Tamanho <> ''
    GROUP BY Tamanho
    order BY Quantidade

```
* a ordem importa
* select, from, where, group by , order by