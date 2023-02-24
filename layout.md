# HTML

## Layout

El Layout indica la disposició dels elements d'una pàgina web.

Normalment les pàgines web tenen seccions, a continuació podem veure un layout amb els noms dels elements que pot tenir:

![image](https://user-images.githubusercontent.com/110727546/221202977-46eed07b-ec1d-496a-aca1-66a5149de251.png)

### Header

Normalment és la part superior d'una web o està a sota de la barra de navegació.

Exemples de header:

```
.header {
  background-color: #f1f1f1;
  padding: 20px;
  text-align: center;
}

.header-imatge{
  font-size:30px;
  color:pink;
  background-color: red;
  background-image:url("https://stores.warhammer.com/wp-content/uploads/2020/11/4jtAGbPWOxDXUHN2.png");
  background-size: 100px 100px;
  padding: 25px;
  text-align: center;
}
```

![image](https://user-images.githubusercontent.com/110727546/221206143-88488fe2-6876-463c-993c-ba9314c98b79.png)

### NavBar

Normalment serveix per tenir una barra de navegació amb un menú d'opcions.

Exemple:

```
<!DOCTYPE html>
<html lang="en">
<head>
<title>CSS Website Layout</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

header{
  font-size:30px;
  color:pink;
  background-color: red;
  background-image:url("https://stores.warhammer.com/wp-content/uploads/2020/11/4jtAGbPWOxDXUHN2.png");
  background-size: 100px 100px;
  padding: 25px;
  text-align: center;
}

body {
  margin: 0;
}

/* Style the top navigation bar */
nav {
  overflow: hidden;
  background-color: #333;
}

/* Style the topnav links */
nav a {
  float: left;
  display: block;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

/* Change color on hover */
nav a:hover {
  background-color: #ddd;
  color: black;
}
</style>
</head>
<body>

<header>
  <h1>Header</h1>
</header>

<nav class="topnav">
  <a href="#">Warhammer</a>
  <a href="#">Warhammer 40K</a>
  <a href="#">Necromunda</a>
</nav>

</body>
</html>
```

![image](https://user-images.githubusercontent.com/110727546/221221652-9b91580c-bd09-40c2-b43f-673601621463.png)






