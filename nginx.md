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

![image](https://user-images.githubusercontent.com/110727546/236473370-784ec917-d46d-49e8-8155-8709cd92264e.png)

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

