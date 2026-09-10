## Consultas Básicas

1. Dados dos usuários

```sql
SELECT * FROM usuarios;
```

2. Nome e e-mail dos usuários

```sql 
SELECT nome, email
FROM usuarios;
```

3. Todas as categorias

```sql
SELECT *
FROM categorias;
```

4. Título e data das notícias

```sql 
SELECT titulo, data
FROM noticias;
```

5. Utilizando AS para renomear colunas

```sql 
SELECT
    nome AS "Nome do Usuário",
    email AS "E-mail",
    tipo AS "Perfil"
FROM usuarios;
```

## Filtros com WHERE

6. Usuários do tipo editor

```sql 
SELECT * 
FROM usuarios 
WHERE tipo = 'editor';
```

7. Notícias em destaque 

```sql 
SELECT *
FROM noticias
WHERE destaque = 'sim';
```

8. Notícias da categoria Tecnologia e Inovação (ID = 1)

```sql 
SELECT * 
FROM noticias 
WHERE categoria_id = 1;
```