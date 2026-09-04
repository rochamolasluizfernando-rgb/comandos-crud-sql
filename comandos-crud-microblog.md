-- USUÀRIOS
```sql 
INSERT INTO usuarios(nome, email, senha, tipo)
VALUES ('Ana Silva', 'ana@email.com', '123abc', 'editor');

INSERT INTO usuarios(nome, email, senha, tipo)
VALUES ('Bruno Souza', 'bruno@email.com', 'abc456', 'admin');

INSERT INTO usuarios(nome, email, senha, tipo)
VALUES ('Carla Mendes', 'carla@email.com', '789xyz', 'editor');
```

-- CATEGORIAS 
```sql 
INSERT INTO categorias(nome)
VALUES('Tecnologia');

INSERT INTO categorias(nome)
VALUES('Educação');

INSERT INTO categorias(nome)
VALUES('Entretenimento');
```

-- NOTÍCIAS
```sql
INSERT INTO noticias
(titulo, resumo, texto, imagem, destaque, usuario_id, categoria_id)
VALUES
(
    'Nova geração de smartphones chega ao mercado',
    'Lançamento promete mais desempenho e bateria.',
    'As fabricantes apresentaram novos modelos com recursos avançados e maior autonomia.',
    'smartphone.jpg',
    1,
    1,
    1
);

INSERT INTO noticias
(titulo, resumo, texto, imagem, destaque, usuario_id, categoria_id)
VALUES
(
    'Plataformas digitais transformam o ensino',
    'Ferramentas online ganham espaço nas escolas.',
    'O uso de ambientes virtuais de aprendizagem cresce em todo o país.',
    'educacao.jpg',
    0,
    3,
    2
);

INSERT INTO noticias
(titulo, resumo, texto, imagem, destaque, usuario_id, categoria_id)
VALUES
(
    'Novo filme bate recordes de bilheteria',
    'Produção lidera arrecadação nas primeiras semanas.',
    'O longa conquistou milhões de espectadores em diversos países.',
    'filme.jpg',
    1,
    2,
    3
);

INSERT INTO noticias
(titulo, resumo, texto, imagem, destaque, usuario_id, categoria_id)
VALUES
(
    'Inteligência Artificial avança no setor tecnológico',
    'Empresas investem cada vez mais em IA.',
    'Novas aplicações estão sendo desenvolvidas para diferentes áreas do mercado.',
    'ia.jpg',
    0,
    1,
    1
);
```