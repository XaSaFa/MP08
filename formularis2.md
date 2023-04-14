# HTML

## Label

Quan utilitzem elements input per un formulari els podem acompanyar d'elements label "etiqueta".

Un element label:
- Ha de tenir un atribut "for" amb un valor idèntic al atribut "id" de l'element type.
- Fer clic a un label associat a un input és equivalent a clicar al mateix input.

```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="checkbox" id="fname" name="fname" value="John"><br>  
</form>
```
## Atributs de input

### ⋆ value ⋆

L'atribut value és el valor inicial que té un element.

```
<input type="text" id="fname" name="fname" value="John">
```

### ⋆ readonly ⋆

Si un input té l'atribut readonly vol dir que no es podrà modificar el valor d'aquest element. 

```
<input type="text" id="fname" name="fname" value="John" readonly><br>
```

[Exemple web.](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_attributes_readonly)

### ⋆ disable ⋆

Un element amb l'atribut disabled no es pot utilitzar i a més el seu valor no s'enviarà amb la resta de valors.

```
<input type="text" id="fname" name="fname" value="John" disabled><br>
```

[Exemple web.](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_attributes_disabled)

### ⋆ size ⋆

Indica el tamany (en nombre de caràcters) que caben dins de l'element, per defecte és de 20.

```
 <input type="text" id="fname" name="fname" size="50"><br>
```

![image](https://user-images.githubusercontent.com/110727546/232070269-ed189149-58e8-4d70-aa4f-3896f879d2eb.png)

[Exemple web.](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_attributes_size)

### ⋆ maxlength ⋆

Indica el número màxim de caràcters que es podran introduir a un input.

```
<input type="text" id="fname" name="fname" size="50"><br>
```

[Exemple web.](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_input_attributes_maxlength)

### ⋆ min i max ⋆

Aquests atributs indiquen els valors mínim i màxim que es permeten als elements.

```
<input type="number" id="quantity" name="quantity" min="1" max="5">
<input type="date" id="datemax" name="datemax" max="1979-12-31">
<input type="date" id="datemin" name="datemin" min="2000-01-02">
```

### ⋆ multiple ⋆

L'atribut multiple serveix per indicar que un element permet més d'un valor entrat per l'usuari.

Només serveix per als elements de tipus email i file.

```
<input type="file" id="files" name="files" multiple>
```

[Exemple web.](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_multiple)

### ⋆ pattern ⋆

Pattern serveix per indicar un patró que ha de seguir l'entrada de l'usuari.

```
<input type="text" id="country_code" name="country_code" pattern="[A-Za-z]{3}" title="Three letter country code">
```

[Exemple web.](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_pattern)

### ⋆ placeholder ⋆

L'atribut placeholder és un text que està dins de l'element input per indicar a l'usuari un exemple del que s'espera que introdueixi.

```
<input type="tel" id="phone" name="phone"
  placeholder="123-45-678"
  pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}">
```

[Exemple web](https://www.w3schools.com/html/tryit.asp?filename=tryhtml5_input_placeholder)
