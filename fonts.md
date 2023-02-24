# CSS

## Fonts de lletra.

Les fonts de lletres ens permeten mostrar text de diferents tipus. Una font de lletres és un conjunt de dibuixos que representen cada caràcter que es vol escriure.

Hem de tenir en compte que no totes les fonts estaran instal·lades a tots els dispositius on es veurà el nostre web, per això és important conèixer les famílies genèriques de fonts.

A CSS hi ha 5 famílies de fonts genèriques:

- **Serif**: Fonts en que les lletres tenen una petita decoració.
- **Sans-serif**: Fonts sense decoració, més austeres.
- **Monospace**: Fonts en les que totes les lletres tenen el mateix ample.
- **Cursive**: Fonts que imiten l'escriptura humana.
- **Fantasy**: Fonts amb més decoració.

![image](https://user-images.githubusercontent.com/110727546/219415999-024ef02e-39ab-4f93-9d7e-2487def0d969.png)

![image](https://user-images.githubusercontent.com/110727546/219416059-c248b5bd-fa12-4438-a4fc-659e449d48bc.png)

![image](https://user-images.githubusercontent.com/110727546/219416327-c6cf99b9-8977-42f0-a1db-b3de07d32d85.png)

### font-family

Serveix per indicar la font del text, normalment fiquem fonts específiques i afegim una font genèrica per si no es pot mostrar la font que volem especificar:

Exemple:

```
.p1 {
  font-family: "Times New Roman", Times, serif;
}

.p2 {
  font-family: Arial, Helvetica, sans-serif;
}

.p3 {
  font-family: "Lucida Console", "Courier New", monospace;
}
```

![image](https://user-images.githubusercontent.com/110727546/219417189-2b64a285-190e-4f1e-ae3e-b0f76fecd9d5.png)

### font-style:

Podem definir l'estil del text entre:
- normal.
- italic (cursiva).
- oblique (similar a italic).

Exemple:

```
p.normal {
  font-style: normal;
}

p.italic {
  font-style: italic;
}

p.oblique {
  font-style: oblique;
}
```

![image](https://user-images.githubusercontent.com/110727546/219418661-95f0ca6a-99bf-4665-a2a5-1a4f09d72c6c.png)



