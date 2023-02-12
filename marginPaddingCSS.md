# CSS

![image](https://user-images.githubusercontent.com/110727546/218313563-f4f80669-f821-4111-ada8-e8e69882f67f.png)

## Margin

L'element margin serveix per crear un marge que envolta un element i que està per fora d'ell, de la seva vora (border).

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss_margin_sides)

Els marges es poden definir indivialment per cada costat:

![image](https://user-images.githubusercontent.com/110727546/218313149-1d7c446b-f582-41dd-9ec0-48a016b4e74a.png)

O directament en una línia:

![image](https://user-images.githubusercontent.com/110727546/218313172-ccad21d1-dc5f-4208-8162-a0ed5719b05a.png)

- Si margin té 4 valors s'està indicant el valor individual de top, right, bottom left.
- Si margin té tres valors s'especifica el valor de top, (right i left), bottom.
- Si margn té dos valors s'especifica el valor de (top i bottom), (right i left).
- Si només té un valor serà el mateix valor pels quatre costats.

### Valor auto:

El valor auto serveix per centrar horitzontalment l'element dins del seu contenidor.

![image](https://user-images.githubusercontent.com/110727546/218313625-4453da7b-5d47-4ba8-91b5-fddf4977eb30.png)

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss_margin_auto)

### Valor inherit:

Podem fer que els elements heretin el marge (tinguin el mateix) que els elements dins els quals estan, ho fem amb la paraula inherit

![image](https://user-images.githubusercontent.com/110727546/218313800-a2dda78c-80a0-4b34-8ace-c2985d8606db.png)

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss_margin-left_inherit)

### Margin collapse:

Els marges de dalt i baix tenen la propietat collapse, la qual no afecta als marges d'esquerra i dreta.

Aquesta propietat fa que els marges top i bottom de dos elements que es toquen no es sumin si no que s'emplei el valor més alt dels dos.

[Exemple web](https://www.w3schools.com/css/tryit.asp?filename=trycss_margin_collapse)

![image](https://user-images.githubusercontent.com/110727546/218313997-e0ee33eb-650d-4311-ab8d-6052e65e9f93.png)

A l'exemple en lloc de tenir dos marges sumats de 10px, per un vaor de 20px només hi haurà un marge de 10px (el valor més alt).

### Practicar:

[Pràctica](https://www.w3schools.com/css/exercise.asp?filename=exercise_margin1).

## Padding:



