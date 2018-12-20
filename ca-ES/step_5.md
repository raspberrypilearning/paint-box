## Cometre errors

De vegades es produeixen errors, així que afegirem un botó "esborrar tot" i una goma d'esborrar.

+ Afegeix l'sprite 'X-block': el trobaràs a la biblioteca, a la secció de lletres. Pinta el vestit de vermell. Això es convertirà en el botó "esborrar tot".

![captura de pantalla](images/paint-x.png)

+ Afegeix codi a aquest sprite per esborrar l'etapa quan es fa clic.

![Esborra pantalla](images/clear-stage.png)

Tingues en compte que no necessites enviar un missatge per esborrar l'escenari, simplement pots utilitzar el botó "esborrar tot" d'aquest sprite.

Probablement hagis notat que el teu sprite de llapis inclou un vestit de goma d'esborrar:

![captura de pantalla](images/paint-eraser-costume.png)

+ El teu projecte també inclou un sprite de goma d'esborrar. Fes clic amb el botó dret sobre aquest sprite i selecciona "mostrar". Així és com s'hauria de veure el teu escenari:

![captura de pantalla](images/paint-eraser-stage.png)

+ Afegeix codi a l'sprite d'esborrar per indicar-li al llapis que canviï a una goma d'esborrar quan es faci clic a l'sprite.

![Goma d'emissió de difusió](images/broadcast-eraser.png)

Quan el llapis rep el missatge "goma d'esborrar", podeu canviar el llapis a la goma d'esborrar i canviar el color del llapis a blanc, el mateix color que l'escenari!

+ Afegeix codi per crear la goma d'esborrar

\--- hints \--- \--- hint \--- Afegeix codi l'sprite de llapis: **Quan rebo** el missatge de**goma d'esborrar** **Canviar al vestit** goma d'esborrar **Configura el color del llapis** a blanc \--- /hint \--- \--- hint \--- Així és com s'hauria de veure el codi dins l'sprite de llapis:

```blocks
quan rebo [goma d'esborrar v]
canvia el vestit a [goma d'esborrar v]
estableix el color del llapis a [#FFFFFF]
```

\--- /hint \--- \--- /hints \---

+ Proveu el vostre projecte per veure si podeu esborrar i esborrar a l'escenari.

![captura de pantalla](images/paint-erase-test.png)

Hi ha un problema més amb el llapis: podeu dibuixar en qualsevol lloc de l'escenari, incloent-hi prop de les icones del selector.

![captura de pantalla](images/paint-draw-problem.png)

Per solucionar-ho, digueu-li només al llapis si es fa clic al ratolí *i* si la posició del mouse és superior a -120:

![captura de pantalla](images/pencil-gt-code.png)

+ Prova el teu projecte; ara no hauríeu de poder acostar-vos als blocs del selector.

![captura de pantalla](images/paint-fixed.png)