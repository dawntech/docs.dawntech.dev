---
title: Blip Bucket Manager
description: 
title-override: Blip Bucket Manager | Dawntech Inc.
---
# Como instalar o plugin no Blip

1. Vá nas configurações do bot.

    ![image](../images/pt/blip-bucket-viewer/home.png)

2. Vá nas configurações avançadas.

    ![image](../images/pt/blip-bucket-viewer/settings.png)

3. Clique em 'Continuar'.

    ![image](../images/pt/blip-bucket-viewer/continue_advanced_settings.png)

4. Adicione o plugin no bot:

    - Se não existir uma configuração com domínio `postmaster@portal.blip.ai` e chave `Plugins`:
       
        1. Crie uma configuração nova, clicando em 'Adicionar'
            
            ![image](../images/pt/blip-bucket-viewer/add_advanced_settings.png)
        
        2. Coloque no campo 'Valor' o seguinte JSON:
            ```
            {
                "bucket-manager": 
                {
                    "name": "Bucket Manager",
                    "url": "https://bucket.dawntech.dev/"
                }
            }
            ``` 

        3. Agora clique no ícone de check.

            ![image](../images/pt/blip-bucket-viewer/add_advanced_settings_2.png)
    
    - Se já existir uma configuração com domínio `postmaster@portal.blip.ai` e chave `Plugins`: 
      
        1. Clique no ícone de edição

            ![image](../images/pt/blip-bucket-viewer/edit_advanced_settings.png)

        2. Se o valor dessa configuração antes era:
            ```
            {
                "some-random-id": {
                    "name": "Some Random Plugin",
                    "url": "https://some-random-plugin-url.com"
                }
            }
            ``` 

            Adicione os valores do JSON para que fique assim:
            ```
            {
                "some-random-id": {
                    "name": "Some Random Plugin",
                    "url": "https://some-random-plugin-url.com"
                },
                "bucket-manager": 
                {
                    "name": "Bucket Manager",
                    "url": "https://bucket.dawntech.dev/"
                }
            }
            ```

            E clique no ícone de check.

            ![image](../images/pt/blip-bucket-viewer/edit_advanced_settings_2.png)

5. Atualize a página e clique nos 3 pontos horizontais para achar o plugin

    ![image](../images/pt/blip-bucket-viewer/3_dots.png)


Você pode achar mais instruções em <https://github.com/takenet/cra-template-blip-plugin/blob/main/template/README.md> na seção `Now just add the plugin to your chatbot and enjoy`
