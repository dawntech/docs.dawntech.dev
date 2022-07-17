---
title: Blip Bucket Manager
description: 
title-override: Blip Bucket Manager | Dawntech Inc.
---

## How to install the plugin on Blip

1. Go to your chatbot configurations.

    ![image](../images/en/blip-bucket-viewer/home.png)

2. Go to advanced settings.

    ![image](../images/en/blip-bucket-viewer/settings.png)

3. Click on 'Continue'.

    ![image](../images/en/blip-bucket-viewer/continue_advanced_settings.png)

4. Add the plugin to the chatbot:

    - If a configuration with domain `postmaster@portal.blip.ai` and key `Plugins` doesn't exists:
       
        1. Create a new configuration, clicking in 'Add'
            
            ![image](../images/en/blip-bucket-viewer/add_advanced_settings.png)
        
        2. Put the following JSON in the "Value" field:
            ```
            {
                "bucket-manager": 
                {
                    "name": "Bucket Manager",
                    "url": "https://bucket.dawntech.dev/"
                }
            }
            ``` 

        3. Now click on the check icon.

            ![image](../images/en/blip-bucket-viewer/add_advanced_settings_2.png)
    
    - If a configuration with domain `postmaster@portal.blip.ai` and key `Plugins` already exists: 
      
        1. Click on the edit icon.

            ![image](../images/en/blip-bucket-viewer/edit_advanced_settings.png)

        2. If before the value of this configuration was:
            ```
            {
                "some-random-id": {
                    "name": "Some Random Plugin",
                    "url": "https://some-random-plugin-url.com"
                }
            }
            ``` 

            Add the JSON values so it stays like this:
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

            And click on the check icon.

            ![image](../images/en/blip-bucket-viewer/edit_advanced_settings_2.png)

5. Refresh the page and find the plugin when clicking on the 3 horizontal points.

    ![image](../images/en/blip-bucket-viewer/3_dots.png)

You can find more instructions in <https://github.com/takenet/cra-template-blip-plugin/blob/main/template/README.md> at section `Now just add the plugin to your chatbot and enjoy`


## Terms of Privacy

When installing this extensions, you automatically agree with the using terms described on [https://dawntech.dev/privacy](https://dawntech.dev/privacy), which is also the policy valid for the data collected by the plugin (when and if needed).

## SLA

The SLA provided by this one and the other plugins by Dawntech Inc. can be accessed on <https://status.dawntech.dev>.


