## Lápices de colores

¡Vamos a añadir lápices de colores diferentes a tu proyecto, y vamos a hacer que el usuario pueda elegir entre ellos!

+ Haz clic en el objeto lápiz, haz clic en “Disfraces” y duplica el disfraz “lápiz-azul”.

	![screenshot](images/paint-blue-duplicate.png)

+ Renombra el nuevo disfraz “lápiz-verde”, y pinta el lápiz de color verde.

	![screenshot](images/paint-pencil-green.png)

+ Crea dos objetos nuevos, que usarás para seleccionar el lápiz azul o el verde.

	![screenshot](images/paint-selectors.png)

+ Al hacer clic en el selector verde, necesitas `enviar` {.blockevents} un mensaje al objeto lápiz, diciéndole que tiene que cambiar su disfraz y color de lápiz.

	Para hacer esto, primero añade este código al objeto selector verde:

	```blocks
		al hacer clic en este objeto
		enviar [Verde v]
	```

	Para crear el bloque `enviar` {.blockevents}, haz clic en la flecha hacia abajo y selecciona “nuevo mensaje…”.

	![screenshot](images/paint-broadcast.png)

	Luego puedes escribir “Verde” para crear tu nuevo mensaje.

	![screenshot](images/paint-green-message.png)

+ Ahora necesitas decirle a tu objeto lápiz qué tiene que hacer cuando recibe el mensaje. Añade este código al objeto lápiz:

	```blocks
		al recibir [Verde v]
		cambiar disfraz a [lápiz-verde v]
		fijar color de lápiz a [#00ff00]
	```

	Para hacer que el lápiz pinte de color verde, haz clic en el recuadro de color del bloque `fijar color` {.blockpen}, y haz clic en el icono selector verde para escoger el verde como el color para tu lápiz.

+ Ahora puedes hacer lo mismo para el lápiz azul, añadiendo este código al objeto selector azul:

	```blocks
		al hacer clic en este objeto
		enviar [Azul v]
	```

	...y añade este código al objeto lápiz:

	```blocks
		al recibir [Azul v]
		cambiar disfraz a [lápiz-azul v]
		fijar color de lápiz a [#0000ff]
	```

+ Por último, necesitas decirle al objeto lápiz qué disfraz y color de lápiz elegir, y limpiar la pantalla cuando empieza tu proyecto. Añade este código al objeto lápiz, al principio del código {.blockevents} `al presionar bandera verde`  (antes del bucle `por siempre` {.blockcontrol}):

	```blocks
		borrar
		cambiar disfraz a [lápiz-azul v]
		fijar color de lápiz a [#0000ff]
	```

	Si lo prefieres, ¡puedes empezar con un color de lápiz diferente!

+ Prueba tu proyecto. ¿Puedes cambiar entre los lápices azul y verde?

	![screenshot](images/paint-pens-test.png)



