# Adicionando uma nova coluna
```sql
    ALTER TABLE Produtos ADD DataCadastro DATETIME2;
    UPDATE Produtos SET DataCadastro = GETDATE();
```
