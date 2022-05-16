# Documentação (page.title)
## Como utilizar

1. Crie um novo repositório **público** utilizando o template
![image](https://user-images.githubusercontent.com/10299622/168600729-abc433cf-601c-475a-994e-b22c48a39333.png)
2. Defina as variáveis em `_config.yml`, sem alterar a chave `theme`.
3. No novo repositório, ative o GitHub Pages nas configurações, alterando o domínio customizado para o desejado.
![image](https://user-images.githubusercontent.com/10299622/168601276-f4932705-00b9-4250-834f-bcfc596e7ec0.png)
4. Confirme o valor do domínio customizado no arquivo [CNAME](CNAME).
5. Adicione o CNAME para a documentação no DNS do domínio:
    - Domain name é o nome customizado presente em [CNAME](CNAME);
    - Canonical name é fixo para todas documentações, deve ser `dawntech.github.io`.
![image](https://user-images.githubusercontent.com/10299622/168602011-ca92088a-4310-4657-a688-c3ec32f1fa60.png)
6. Após propagado, a documentação deverá estar acessível na URL definida, com o conteúdo definido neste arquivo.

# Documentação de rotas (exemplo)

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
