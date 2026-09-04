# Comandos CRUD para o banco de dados Fly By Night

## INSERT de fornecedores

```sql
INSERT INTO fornecedores (nome) VALUES('Eletrônicos Tabajara');

INSERT INTO fornecedores (nome) VALUES
    ('Games ABCD'),
    ('Supermercado Tem de Tudo'),
    ('Livraria Demais da Conta');
```

## INSERT na tabela de Produtos 
```sql 
INSERT INTO produtos (nome, descricao, preco, quantidade, fornecedor_id)
VALUES(
    'Smartphone Galaxy S23',
    'Equipamento com sistema Android e câmera Full HD e etc e tal',
    1599.45,
    20,
    1 -- id do fornecedor Eletrônicos Tabajara
);
```