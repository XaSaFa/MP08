# Instal·lar Nginx i PHP

1. Actualitzem paquets.

```
sudo apt update
```

2. Instal·lem el servidor Nginx:

```
sudo apt install nginx
```

3. Comprovem que funciona el servidor:

![image](https://user-images.githubusercontent.com/110727546/236466748-ed359bf9-4a2b-42c5-96eb-f5c1e6e0022d.png)

4. Comprovem la versió de PHP que necessita Owncloud:

![image](https://user-images.githubusercontent.com/110727546/236467047-f899b034-e802-4ec3-b213-d84d8bb1bf4c.png)

5. Afegim al nostre equip el repositori per a instal·lar PHP 7.4

```
sudo add-apt-repository ppa:ondrej/php
```

6. Actualitzem paquets.

```
sudo apt update
```

7. Instal·lem PHP 7.4

```
sudo apt install php7.4-fpm
```

8. Comprovem que està instal·lat

```
sudo service php7.4-fpm status
```

![image](https://user-images.githubusercontent.com/110727546/236472017-ff2b2f34-8cbc-40ee-aee7-23e532bea7f6.png)

9. Editem el fitxer de configuració de nginx per habilitar PHP

```
sudo nano /etc/nginx/sites-available/default
```

Fent els següents canvis:

![image](https://user-images.githubusercontent.com/110727546/236473019-8fb69a14-fd6c-4b83-baa8-139b20f8fdb1.png)

![image](https://user-images.githubusercontent.com/110727546/236475405-8f236183-a3d1-441d-98b1-f232bc0a85f1.png)

Comprovem que la sintaxis del fitxer de configuració és correcta.

```
sudo nginx -t
``` 

![image](https://user-images.githubusercontent.com/110727546/236475934-00ab0bbd-28b0-4405-8c5a-14f6821b1491.png)

10. Reiniciem servidor

```
sudo service nginx restart
```

11. Comprovem que PHP funciona a Nginx

Fem un fitxer anomenat index.php a /var/www/html

El codi del fitxer serà:

![image](https://user-images.githubusercontent.com/110727546/236474069-558a0ce8-7016-42b8-b36e-a05f592f8f52.png)

Comprovem al navegador que funciona:

![image](https://user-images.githubusercontent.com/110727546/236473828-bddc2ce9-36fa-4168-8b2a-efe49c9fc5d2.png)

12. Instal·lem MariaDB

[seguiu els passos necessaris](https://dungeonofbits.com/instalacion-de-owncloud-en-linux.html)

13. Instal·lem Owncloud

[seguiu els passos necessaris](https://dungeonofbits.com/instalacion-de-owncloud-en-linux.html)

14. Instal·lem els paquets que falten:

![Captura de pantalla de 2023-05-11 15-23-19](https://github.com/XaSaFa/MP08/assets/110727546/0f275434-bd34-43a0-b06d-9b9849a3385f)

15. Canvieu el fitxer de configuració de nginx a /etc/nginx/sites-available

![image](https://github.com/XaSaFa/MP08/assets/110727546/1e9bd52e-c80a-447d-9810-a99858bad6b2)

```
server {
    server_name owncloud.your_domain.com;
    root /var/www/html/owncloud;

    access_log /var/log/nginx/owncloud.your_domain-access.log;
    error_log /var/log/nginx/owncloud.your_domain-error.log;

    location / {
        index index.php;
        try_files $uri $uri/ /index.php$is_args$args;
    }

    location ~ \.php$ {
        include snippets/fastcgi-php.conf;
        fastcgi_pass unix:/run/php/php7.4-fpm.sock;
        fastcgi_param SCRIPT_FILENAME $document_root$fastcgi_script_name;
    }
}
```

Ja hauria de funcionar

![image](https://github.com/XaSaFa/MP08/assets/110727546/394de47e-9a62-4dfd-936e-16134a5463f8)

## Habilitar directoris locals a Owncloud

[Mireu a la documentació de Owncloud](https://doc.owncloud.com/server/next/admin_manual/configuration/files/external_storage/local.html)

Heu d'habilitar emmagatzematge extern dins de Owncloud:

![image](https://github.com/XaSaFa/MP08/assets/110727546/b9cbef3e-377b-424d-96b4-20c95e52ae3f)

I editar el fitxer de configuració com diu la configuració de Owncloud:

![image](https://github.com/XaSaFa/MP08/assets/110727546/3597713f-69d0-4554-8278-1078acbe925d)

Llavors ja podreu escollir emmagatzematge **Local**

![image](https://github.com/XaSaFa/MP08/assets/110727546/7c91bfba-4268-4a1e-b1d6-bd10d3594597)

