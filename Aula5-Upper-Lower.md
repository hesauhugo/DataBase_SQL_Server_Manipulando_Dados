# Usando Upper e Lower
```sql
    -- Maiúsculo
    SELECT
        UPPER(Nome + ' - ' + Cor) NomeProduto
    FROM
        Produtos

    -- Minúsculo
    SELECT
        LOWER(Nome + ' - ' + Cor) NomeProduto
    FROM
        Produtos
        
```