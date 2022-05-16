---
title: Documentação
description: Descrição
title-override: Título
---

# Documentação
## Como utilizar

1. Exemplo exemplo
![image](https://user-images.githubusercontent.com/10299622/168600729-abc433cf-601c-475a-994e-b22c48a39333.png)
2. Exemplo

# Documentação de rotas

## Inserção

- Método: `POST`
- URL: `https://api.dawntech.dev/endpoint`
- Headers: `dawntech-user-id: <user_id>`
- Body:
```
[
    {
        "Last_Name": string | Last name of the lead,
        "First_Name": string | First name of the lead,
        "Email": string | Email of the lead,
        "Company": string | Company where the lead works
    },
    ...
]
```

## Busca
- Método: `GET`
- URL: `https://api.zoho.dawntech.dev/endpoint`
- Headers: `dawntech-user-id: <user_id>`
