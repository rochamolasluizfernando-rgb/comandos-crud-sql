## Atualizando e excluindo dados

## Alterando o nome de um dos usuários cadastrados
```sql
UPDATE usuarios SET nome = 'Carlos Eduardo' WHERE id = 1;
```

## Alterando o tipo de um usuário de editor para admin
```sql 
UPDATE usuarios SET tipo = 'admin' WHERE id = 1;
```

## Alterando o nome de uma categoria
```sql 
UPDATE categorias SET nome = 'Tecnologia e Inovação' WHERE id = 1;
```

## Alterando o título de uma notícia
```sql 
UPDATE noticias SET titulo = 'Inteligência Artificial transforma o mercado de trabalho' WHERE id = 4;
```

## Alterando uma notícia que esteja com destaque = 'nao' para destaque = 'sim'
```sql
UPDATE noticias SET destaque = 'nao' WHERE id = 5;
```

## Alterando a categoria de uma notícia
```sql
UPDATE noticias SET categoria_id = 3 WHERE id = 1;
```

## Excluindo uma das notícias cadastradas
```sql
DELETE FROM noticias = 26 WHERE id = 3;
```

## Excluindo uma categoria que não esteja sendo utilizada por nenhuma notícia
```sql
DELETE FROM categorias = 29 WHERE id = 5; 
```

## Excluindo um usuário que não esteja associado a nenhuma notícia
```sql 
DELETE FROM usuarios = 32 WHERE id = 4;
```