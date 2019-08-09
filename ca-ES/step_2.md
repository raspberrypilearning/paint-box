## Feu un llapis

Comenceu fent un llapis que podeu fer servir per dibuixar a l’escenari.

\--- task \--- Obriu el projecte d’inici Scratch 'Paint box'.

**En línia**: obriu el projecte inicial al [rpf.io/paint-box-on](http://rpf.io/paint-box-on){: target = "_ blank"}

Si tens un compte a Scratch fes una còpia fent clic a **Reinventa**.

**Desconnectat**: obriu el projecte [arrencada](http://rpf.io/p/en/paint-box-go){: target = "_ blank"} a l'editor fora de línia.

Si necessiteu descarregar i instal·lar l’editor fora de línia Scratch, el podeu trobar a [rpf.io/scratchoff](http://rpf.io/scratchoff){: target = "_ blank"}

Al projecte d’arrencada, hauríeu de veure sprites de llapis i d’esborranys:

![captura de pantalla](images/paint-starter.png) \--- /task \---

\--- task \---

Afegiu l’extensió del llapis al vostre projecte.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Afegiu algun codi al sprite de llapis per fer que el sprite seguiu el punter del ratolí `per sempre`{: class = "block3control"} perquè pugueu dibuixar:

![llapis](images/pencil.png)

```blocks3
quan es fa clic a la bandera
per sempre
  aneu a (punter del ratolí v)
final
```

\--- /task \---

\--- task \--- Feu clic al senyalador i, a continuació, moveu el punter del ratolí al voltant de l’etapa per provar si el vostre codi funciona. \--- /task \---

A continuació, feu que el llapis només dibuixi `si es fa clic amb el botó del ratolí`{: class = "block3control"}.

\--- task \--- Afegiu aquest codi al vostre sprite de llapis:

![llapis](images/pencil.png)

```blocks3
quan es fa clic a la bandera
per sempre
  aneu a (punter del ratolí v)

+ si <mouse down?> llavors
  llapis cap avall
  llapis
  fins al final

```

\--- /task \---

\--- task \--- Torneu a provar el vostre codi. Aquesta vegada, moveu el llapis al voltant de l’etapa i manteniu premut el botó del ratolí. Es pot dibuixar amb el teu llapis?

![captura de pantalla](images/paint-draw.png) \--- /task \---

## \--- collapse \---

## title: El seu llapis no es dibuixa de la seva punta?

Si la línia del dibuix de llapis sembla que prové del centre del llapis, haureu de canviar el sprite del llapis de manera que la punta sigui el centre del sprite.

Feu clic al sprite del llapis i feu clic a la pestanya **Disfresses**.

Moure el vestit de manera que la punta del llapis és **just per sobre de** el centre.

![Centre de rotació](images/costume-center-annotated.png)

Ara moveu el llapis al voltant de l’escenari i dibuixeu-lo. El llapis hauria de dibuixar una línia des de la seva punta.

\--- / collapse \---