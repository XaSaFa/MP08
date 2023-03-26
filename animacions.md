# HTML

Icona a la pestanya de la pàgina web.

Normalment les pàgines que visitem tenen una petita imatge o logotip a la pestanya del navegador per identificar-les millor, això ho podem fer amb HTML:

![image](https://user-images.githubusercontent.com/110727546/227779104-6af466b7-a354-4072-82f4-91177bc1a1ba.png)

Exemple, tenim un web dedicat a la música i volem utilitzar una imatge d'una nota musical:

![image](https://user-images.githubusercontent.com/110727546/227778933-54710e15-9edd-49d3-ba35-cd1458b89d26.png)

El millor es que descarreguem la imatge i la tinguem al servidor per evitar problemes com que desaparegui el recurs o canvii de nom.

La línia que hem d'escriure dins de l'etiqueta HEAD del nostre web és:

```
<link rel="icon" href="https://cdn-icons-png.flaticon.com/512/727/727248.png" />
```

Resultat:

![image](https://user-images.githubusercontent.com/110727546/227779399-c03778a2-0d76-4044-abec-fbe642335d90.png)

# CSS

De vegades ens interessa que alguns elements del nostre web tinguin una petita animació, això ho podem aconseguir amb CSS.

Per a fer-ho utilitzem la propietat animation i keyframes.

## animation-name:

És el nom del keyframe d'animacions que farem servir.

## animation-duration:

La durada que tindrà l'animació.

## animation-delay:

El retràs entre que carrega el web i comença l'animació (pot ser negatiu).

## animation-iteration-count:

Quantes vegades es repetirà l'animació, si volem que es repeteixi per sempre li direm que és infinite.

## animation-direction:

Per defecte l'animació es comportarà com li indiquem, però podem fer que vagi al revés amb el valor **reverse**, que alterni amb el valor **alternate** o que alterni i vagi al revés amb **alternate-reverse**.

![image](https://user-images.githubusercontent.com/110727546/227781595-1ed9fa86-b5bd-4bbe-b332-b6ab1055fcbd.png)

## animation-timing-function:

Especifica la corva d'acceleració de l'animació.

![image](https://user-images.githubusercontent.com/110727546/227781632-7c45ac5d-0c6b-4e17-97fa-ca3c0aa57a3a.png)

## animation-fill-mode:

Amb aquesta propietat indiquem com volem que quedi un element quan està fora de l'animació (abans o després).

![image](https://user-images.githubusercontent.com/110727546/227781771-da195537-e9de-4891-8821-b1b13a776f2c.png)

Exemples:

```
/* The animation code */
@keyframes example {
  from {background-color: red;}
  to {background-color: yellow;}
}

/* The element to apply the animation to */
div {
  width: 100px;
  height: 100px;
  background-color: red;
  animation-name: example;
  animation-duration: 4s;
}
```

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss3_animation1)

Com veieu el nostre element haurà de tenir una propietat **animation-name** que coincideixi amb el nom del **@keyframes**.

En l'exemple anterior hem indicat un estat inicial i un final, però podem indicar més estats intermitjos:

```
/* The animation code */
@keyframes example {
  0%   {background-color: red;}
  25%  {background-color: yellow;}
  50%  {background-color: blue;}
  100% {background-color: green;}
}

/* The element to apply the animation to */
div {
  width: 100px;
  height: 100px;
  background-color: red;
  animation-name: example;
  animation-duration: 4s;
}
```

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss3_animation2)

Podem alterar més d'una propietat a cada estat:

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss3_animation3)

Apliquem un retard a l'animació amb **animation-delay**:

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss3_animation_delay)

Indiquem quantes vegades volem que es faci l'animació amb **animation-iteration-count**:

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss3_animation_count)

Fem que una animació vagi al revés amb **animation-direction**:

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss3_animation_direction)

Podem alterar la corva de velocitat de l'animació amb **animation-timing-function**:

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss3_animation_speed)

Podem fer que l'objecte canviï el seu estat final amb **animation-fill-mode**:

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss3_animation_fill-mode)

# Practicar:

[Pràctica](https://www.w3schools.com/css/exercise.asp?filename=exercise_css3_animations1)






