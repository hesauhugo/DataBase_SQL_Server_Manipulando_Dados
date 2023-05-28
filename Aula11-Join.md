# Realiando um JOIN
* fazendo join inicial
```sql
    SELECT 
        * 
    FROM 
        Clientes
    INNER JOIN 
        Enderecos 
        ON 
            Clientes.Id = Enderecos.IdCliente

    WHERE Clientes.Id = 4
```

* Ao selecionar o `Id`  tem nomes iguais e pode dar erro de ambiguos
* Fazendo join e apresentando colunas de cada tabela em conjunto

```sql
    SELECT 
        Clientes.Nome,
        Clientes.Sobrenome,
        Clientes.Email,
        Enderecos.Bairro,
        Enderecos.Cidade

    FROM 
        Clientes
    INNER JOIN Enderecos ON Clientes.Id = Enderecos.IdCliente
    WHERE Clientes.Id = 4
```
* dando nome para as tabelas

```sql

    SELECT 
        C.Nome,
        C.Sobrenome,
        C.Email,
        E.Bairro,
        E.Cidade

    FROM 
        Clientes C
    INNER JOIN Enderecos E ON C.Id = E.IdCliente
    WHERE C.Id = 4

```