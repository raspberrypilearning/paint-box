## Desfés els errors

De vegades es produeixen errors, de manera que afegiu un botó "netejar" i un botó d'esborrany.

\--- task \--- Afegiu el "sprite X-block" a la secció de lletres de la biblioteca. Acoloreu el vestit de l'esperit en vermell i fes-lo una mica més petit. Aquest sprite és el botó "netejar".

[[[generic-scratch3-sprite-from-library]]]

![captura de pantalla](images/paint-x.png) \--- /task \---

\--- task \--- Afegiu codi al sprite del "X-block" per esborrar la fase quan el sprite hagi fet clic.

![creu](images/cross.png)

```blocks3
quan aquest sprite va fer clic a
esborrar-ho tot
```

\--- /task \---

No heu d’utilitzar un `broadcast`{: class = "block3events"} per esborrar l’etapa, ja que els `esborren tots els`{: class = "block3extensions"} bloc que fan aquesta feina.

Veus que el llapis sprite inclou un vestit de goma?

![captura de pantalla](images/paint-eraser-costume.png)

El teu projecte també inclou un sprite de goma d'esborrar.

\--- task \--- Feu clic amb el botó dret del ratolí sobre aquest sprite de l'esborrany i feu clic a **show**. A continuació, s’explica com hauria de mirar ara el vostre escenari:

![captura de pantalla](images/paint-eraser-stage.png) \--- /task \---

\--- task \--- Afegiu un codi al sprite del esborrany per enviar una emissió `'eraser'`{: class = "block3events"} quan es fa clic a l'esborrador de l'esborrador.

![goma d'esborrar](images/eraser.png)

```blocks3
quan aquest sprite va fer clic en
difusió (esborrany v)
```

\--- /task \---

Quan el sprite de llapis rep el missatge d’un "esborrany", hauria de canviar el seu vestit a l’esbós i canviar el color del llapis al blanc, que és del mateix color que l’escenari.

\--- task \--- Afegiu alguns codis per crear el borrador.

\--- consells \--- \--- pista \--- Afegiu algun codi al sprite del llapis: `Quan rebo`{: class = "block3events"} el `eraser`{: class = "block3events"} missatge `Canvia a esborrar de disfresses`{: class = "block3looks"} `Estableix el color de la ploma`{: class = "block3extensions"} al blanc \--- / pista \--- \--- pista \--- Aquí teniu tots els blocs que necessiteu:

```blocks3
estableix el color del llapis a [#FFFFFF]
quan rebi [eraser v]

canvia el vestit (eraser v)
```

\--- / hint \--- \--- pista \--- Això és el que hauria de tenir el codi: ![llapis](images/pencil.png)

```blocks3
quan rebo [eraser v]
canvi de vestit a (borrador v)
establir color de llapis a [#FFFFFF]
```

\--- / pista \--- \--- / consells \--- \--- / tasca \---

\--- task \--- Poseu a prova el vostre projecte per veure si podeu esborrar les etapes i esborrar les línies de llapis.

![captura de pantalla](images/paint-erase-test.png) \--- /task \---

Hi ha un altre problema amb el llapis: podeu dibuixar en qualsevol lloc de l’Escenari, inclosos els botons "netejar" i "d'esborrar".

![captura de pantalla](images/paint-draw-problem.png)

\--- task \--- Per solucionar-ho, canvieu el codi de manera que el llapis només estigui cap avall si es fa clic al ratolí **i** la posició `y` del punter del ratolí és superior a `-120`:

![llapis](images/pencil.png)

```blocks3
quan es fa clic a la bandera
esborrar tots els
vestit de canvi a (llapis blau v)
establir el color del llapis a [# 0035FF]
per sempre
  aneu a (punter del ratolí v)
+ si <<mouse down?> i <(i el ratolí) > [-120]>> a continuació, 
  la ploma cap avall
  més
  de la ploma fins
final
```

\--- /task \---

\--- task \--- Posa a prova el teu projecte. Ara no hauríeu de poder apropar-vos als botons.

![captura de pantalla](images/paint-fixed.png) \--- /task \---