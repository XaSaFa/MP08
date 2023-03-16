# Bootstrap

Quan fem servir bootstrap us doneu compte de que es fan servir un munt de classe pròpies.

Anem a veure algunes d'elles.


## Headings

Podem fer que el text d'altres elements que no siguin heading es comportin com heading utilitzant les classes: h1 a h6.

Aquestes dues línies es comporten igual:

```
<p class="h1">h1 Bootstrap heading</p>
<h1>h1 Bootstrap heading</h1>
```

[Exemple web](https://www.w3schools.com/bootstrap5/tryit.asp?filename=trybs_txt_hn&stacked=h)

## Displays

Bootstrap disposa també de 6 capçaleres anomenades displays, que tenen un tamany de lletra més gran que els headings però són més lleugeres.

[Exemple web](https://www.w3schools.com/bootstrap5/tryit.asp?filename=trybs_txt_display&stacked=h)

## Small

Dins d'un mateix heading podem tenir dos tamanys diferents de lletres utilitzant l'element small.

```
<h1>h1 heading <small>secondary text</small></h1>
```
![image](https://user-images.githubusercontent.com/110727546/225693112-6cedc756-a432-44ea-a300-469aba8b7309.png)

## Color de lletra

A Bootstrap tenim classes per definir colors contextuals

- .text-muted
- .text-primary
- .text-success
- .text-info
- .text-warning
- .text-danger
- .text-secondary
- .text-white
- .text-dark
- .text-body
- .text-light

![image](https://user-images.githubusercontent.com/110727546/225694010-574aa7b7-98c9-4c97-b5c2-ad18cc62ca75.png)

[Exemple web](https://www.w3schools.com/bootstrap5/tryit.asp?filename=trybs_txt_colors&stacked=h)

## Color de fons d'elements

També tenim  classes per els colors de fons dels elements.

- .bg-primary
- .bg-success
- .bg-info
- .bg-warning
- .bg-danger
- .bg-secondary
- .bg-dark
- .bg-light.

![image](https://user-images.githubusercontent.com/110727546/225694676-c057fa26-2d4b-44c0-9159-7ea08b51543b.png)

[Exemple web](https://www.w3schools.com/bootstrap5/tryit.asp?filename=trybs_txt_bgcolors&stacked=h)

Podeu utilitzar la classe especifica text-bg-nomDeColor per al color de fons del text:

![image](https://user-images.githubusercontent.com/110727546/225695383-6bb4eaf2-cf77-4fa8-a94c-78263fd9993d.png)

[Exemple web](https://www.w3schools.com/bootstrap5/tryit.asp?filename=trybs_txt_bgcolors2&stacked=h)

## Contenidors

Els elements de Bootstrap han d'estar dins un contenidor, Bootstrap 5 té 2 tipus de contenidors:

- .container
- .container-fluid

![image](https://user-images.githubusercontent.com/110727546/225710329-49fe0637-4b9f-4f1e-860d-915baef4deaa.png)

[Exemple web](https://www.w3schools.com/bootstrap5/tryit.asp?filename=trybs_gs_container&stacked=v)

Aprofitem per aplicar el que hem aprés a l'exemple i practicar.

## Espaiat dels elements

Bootstrap disposa de classes per crear margin i padding, les classes **p** i **m**.

- m - for classes that set margin
- p - for classes that set padding

Costats als que aplica:

- t - for classes that set margin-top or padding-top
- b - for classes that set margin-bottom or padding-bottom
- s - (start) for classes that set margin-left or padding-left in LTR, margin-right or padding-right in RTL
- e - (end) for classes that set margin-right or padding-right in LTR, margin-left or padding-left in RTL
- x - for classes that set both *-left and *-right
- y - for classes that set both *-top and *-bottom
- blank - for classes that set a margin or padding on all 4 sides of the element

Quantitat de separació:

- 0 - for classes that eliminate the margin or padding by setting it to 0
- 1 - (by default) for classes that set the margin or padding to $spacer * .25
- 2 - (by default) for classes that set the margin or padding to $spacer * .5
- 3 - (by default) for classes that set the margin or padding to $spacer
- 4 - (by default) for classes that set the margin or padding to $spacer * 1.5
- 5 - (by default) for classes that set the margin or padding to $spacer * 3
- auto - for classes that set the margin to auto

## Grid

El sistema de grid ens deixa ordenar elements div per fil·les i columnes:

![image](https://user-images.githubusercontent.com/110727546/225721721-337b09c0-e796-4306-bf69-bc4c8600cba6.png)

```
<div class="container">
  <div class="row">
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
  </div>
</div>
```

[Exemples](https://getbootstrap.com/docs/5.0/layout/grid/)








