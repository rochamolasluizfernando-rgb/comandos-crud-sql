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

9. Excluir usuários administradores 

```sql 
SELECT * 
FROM usuarios 
WHERE tipo <> 'admin';
```

## Combiando condições 

10. Utilizando AND 

```sql 
SELECT * 
FROM noticias 
WHERE destaque = 'sim'
AND categoria_id = 1;
```

11. Utilizando OR 

```sql 
SELECT * 
FROM usuarios 
WHERE tipo 'admin'
OR tipo = 'editor';
```

## Pesquisas com LIKE

12. Procurar notícias que contenham "smartphone"

```sql 
SELECT * 
FROM noticias 
WHERE titulo LIKE '%smartphone%';
``` 

13. Procurar usuários cujo nome começa com "A"

```sql 
SELECT * 
FROM usuarios 
WHERE nome LIKE 'A%';
```

## Ordenação 

14. Notícias da mais recente para a mais antiga

```sql 
SELECT * 
FROM noticias 
ORDER BY data DESC; 
```

15. Usuários em ordem alfabética

```sql 
SELECT * 
FROM usuarios 
ORDER BY nome ASC;
```

## Funções de agregação 

16. Quantidade de usuários cadastrados 

```sql 
SELECT COUNT(*) AS total_usuarios  
FROM usuarios; 
```

17. Quantidade de notícias cadastradas 

```sql 
SELECT COUNT(*) AS total_noticias 
FROM usuarios;
```

18. Notícia mais antiga e mais recente 

```sql 
SELECT 
    MIN(data) AS noticia_mais_antiga,
    MAX(data) AS noticia_mais_recente
FROM noticias;
```

## Desafio 

19. Consulta combinando AS, WHERE, LIKE e ORDER BY

```sql 
SELECT
    titulo AS "Título",
    data AS "Data de Publicação",
    destaque AS "Em Destaque"
FROM noticias
WHERE destaque = 'sim'
AND titulo LIKE '%smart%'
ORDER BY data DESC;
```