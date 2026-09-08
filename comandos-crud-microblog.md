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
    'sim',
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
    'sim',
    3,
    2
);

INSERT INTO noticias (titulo, resumo, texto, imagem, destaque, usuario_id, categoria_id)
VALUES
(
    'Corinthias está mal para caramba',
    'O time caiu muito após a copa do mundo',
    'Não sei mais o que escrever sobre isso tudo e etc e tal e bla bla',
    'corinthians.jpg'
    'sim'
    1,
    1
);

INSERT INTO noticias (titulo, resumo, texto, imagem, destaque, usuario_id, categoria_id)
VALUES
(
    'Visual Studio Code com IA aprimorada',
    'As atualizações recentes do VSCode trouxeram melhorias para o Copilot',
    'Usar o VSCode ficou mais fácil pois etc e tal bla bla bla e etc e sei la etc',
    'vscode.jpg'
);
```