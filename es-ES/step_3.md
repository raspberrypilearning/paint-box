## Lápices de colores

Ahora vas a añadir diferentes lápices de colores a tu proyecto y permitir que el usuario elija entre los mismos.

\--- task \---

Cambia el nombre del objeto `lápiz` a ` lápiz-azul `

![renombrar-lápiz](images/rename-pencil.png)

\--- /task \---

\--- task \---

Haz clic en el botón derecho del objeto lápiz-azul y duplica su disfraz.

![captura de pantalla](images/paint-blue-duplicate.png)

\--- /task \---

\--- task \---

Cambia el nombre de tu nuevo disfraz a 'lápiz-verde' y cambia su color a verde.

![captura de pantalla](images/paint-pencil-green.png)

\--- /task \---

\--- task \---

Dibuja dos objetos más - un cuadrado azul y un cuadrado verde. Estos sirven para elegir entre el lápiz azul y el verde.

![captura de pantalla](images/paint-selectors.png)

\--- /task \---

\--- task \---

Renombra los nuevos objetos para que se llamen 'azul' y 'verde'

[[[generic-scratch3-rename-sprite]]]

\--- /task \---

\--- task \---

Añade algún código al objeto ‘verde’, de modo que cuando se haga clic en este objeto, se `envie`{:class="block3events"} el mensaje “verde”.

![cuadrado verde](images/green_square.png)

```blocks3
al hacer clic en este objeto
enviar (verde v)
```

[[[generic-scratch3-broadcast-message]]]

\--- /task \---

El objeto lápiz debería 'escuchar' el mensaje "verde" y cambiar su disfraz y color de lápiz como respuesta.

\--- task \---

Cambia al objeto lápiz. Añade algún código de modo que cuando este objeto reciba el envio `verde`{:class="block3events"}, cambie al disfraz de lápiz verde y cambie el color de lápiz a verde.

![lápiz](images/pencil.png)

```blocks3
al recibir [verde v]
cambiar disfraz a (lápiz-verde v)
fijar color de lápiz a [#00C44]
```

Para poner el color de lápiz en verde, haz clic en el pequeño ovalo que está a la derecha, dentro, en el bloque `fijar color de lápiz a`{:class="block3extensions"}, luego haz clic en el cuentagotas y selecciona el objeto cuadrado verde.

\--- /task \---

Luego del mismo modo puedes cambiar el color de lápiz a azul.

\--- task \---

Haz clic sobre el objeto cuadrado azul y añade este código:

![cuadrado azul](images/blue_square.png)

```blocks3
al hacer clic en este objeto
enviar (azul v)
```

Luego, haz clic sobre el objeto lápiz y añade este código:

![lápiz](images/pencil.png)

```blocks3
al recibir [azul v]
cambiar disfraz a (lápiz-azul v)
fijar color de lápiz a [#0000ff]
```

\--- /task \---

\--- task \---

Finalmente, añade este código para indicarle al objeto lápiz con qué color comenzar, y asegurarte de que la pantalla esté limpia cuando comiences.

![lápiz](images/pencil.png)

```blocks3
al hacer clic en la bandera
+borrar todo
+cambiar disfraz a (lápiz-azul v)
+fijar color de lápiz a [#0035FF]
por siempre
  ir a (puntero del ratón v)
si<mouse down?>entonces
  bajar lápiz
  si no 
  subir lápiz
fin
```

\--- /task \---

Si prefieres, puedes comenzar con un lápiz de color diferente.

\--- task \---

Prueba tu código. ¿Puedes cambiar entre el color de lápiz verde y el azul al cliquear en los objetos cuadrado azul o verde?

![captura de pantalla](images/paint-pens-test.png)

\--- /task \---