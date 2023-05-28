# Criando a tabela de endereços com foreign key
* Visualizar design
* setar como primary key

```sql
    --CRIANDO TABELA
    CREATE TABLE Enderecos (
        Id int PRIMARY KEY IDENTITY(1,1) NOT NULL,
        IdCliente int NULL,
        Rua varchar(255) NULL,
        Bairro varchar(255) NULL,
        Cidade varchar(255) NULL,
        Estado char(2) NULL,

        CONSTRAINT FK_Enderecos_Clientes FOREIGN KEY (IdCliente) REFERENCES Clientes(Id)
    )
    --INSTRUÇÕES SELECT
    SELECT * FROM Clientes
    SELECT * FROM Enderecos

    --INSERINDO DADOS NA TABELA
    INSERT INTO Enderecos VALUES (4,'Rua Teste', 'Bairro teste', 'Cidade teste', 'SP')

```