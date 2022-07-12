# docs.dawntech.dev


## Como criar uma nova página na documentação

Documentação utilizando o GitHub Pages, que usa o Jekyll pra processar Markdown em HTML.

Para criar uma nova página:

- Crie um arquivo .md com o nome do link desejado. Ex: O arquivo [zoho.md](zoho.md) gera [https://docs.dawntech.dev/zoho](https://docs.dawntech.dev/zoho).
- Inserir imagens usando a mesma lógica do nome dentro do diretórios `images`.
- Dentro do arquivo .md criado, inserir um header de metadados:
```
---
title: Título do Header
description: 
title-override: Título da Aba | Dawntech Inc.
---
```
- Após o push para main, o GitHub Actions (https://github.com/dawntech/docs.dawntech.dev/actions) vai transformar os arquivos em um site estático, disponível em https://docs.dawntech.dev
