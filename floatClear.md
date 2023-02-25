# CSS

## Float

La propietat float especifica com un element "flota", d'aquesta manera es pot posicionar un contingut, com una imatge o un bloc de text.

Els valors de float són:

![image](https://user-images.githubusercontent.com/110727546/221346696-030e3e39-706c-4f14-9612-aae85cdb5598.png)

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_float)

![image](https://user-images.githubusercontent.com/110727546/221346787-a181171d-4e47-4e8e-bccb-716971fbaed5.png)

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_float3)

![image](https://user-images.githubusercontent.com/110727546/221346824-1a683618-0b7f-4589-b90d-42e2a1af5bd7.png)

## Clear

Quan fem servir la propietat Float i volem que el següent element a sota (no al costat), hem d'utiitzar la propietat clear.

Clear diu que passarà amb els elements que segueixen a un element amb la propietat float.

Pot tenir els següents valors:

![image](https://user-images.githubusercontent.com/110727546/221346919-3f207f6e-c11e-4246-a67b-d1260276cfaf.png)

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_clear)

![image](https://user-images.githubusercontent.com/110727546/221346969-60f016bd-abd2-47f8-8b92-9e7f083024a6.png)

### Clearfix

Quan tenim un element flotant que és més alt que l'element que el conté aquest element sortirà per fora de l'element contenidor.

Exemple:

![image](https://user-images.githubusercontent.com/110727546/221347101-6b3dd75c-1a5b-48a2-91e0-b15278caf324.png)

Si volem que estigui dins de l'element contenidor haurem d'utilitzar algun truc:

![image](https://user-images.githubusercontent.com/110727546/221347345-4a67765a-0897-4d11-8dfe-5f8423e5e00d.png)

#### Overflow

```
.clearfix {
  overflow: auto;
}
```

#### Clearfix hack

```
.clearfix::after {
  content: "";
  clear: both;
  display: table;
}
```

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss_layout_clearfix2)

## Exemples 

### Caixes de text

![image](https://user-images.githubusercontent.com/110727546/221347448-73bc5fb0-ea3f-4da4-9f05-a87bff1d54f3.png)

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss_float_boxes)

### Imatges

![image](https://user-images.githubusercontent.com/110727546/221347485-aa49adaf-a2da-473d-9807-fcedbd8d226a.png)

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss_float_images_side)

### Barra de navegació

![image](https://user-images.githubusercontent.com/110727546/221347902-8fcb28a2-c957-49f4-ae29-8615ccb0271f.png)

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss_float5)
