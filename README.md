I have visualised api about products using infinity datasource in grafana.
For deploying, find the custom.ini in /conf folder. If you don't find custom.ini in conf, then copy the sample.ini and rename it as custom.ini. Then change the custom.ini based on the requirements.
Here for embedding the grafana dashboard in index.html, I have changed the following in custom.ini:
1. allow_embedding = true
2. In auth.anonymous:
        enable = true
        org_name = Main Org.
        org_role = Viewer
If you move to the "Server Admin" , then choose "settings". Check the enabling of the above points.
Then, In the share option in created dashboard , contains "Embeded" option.
