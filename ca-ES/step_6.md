## Canviar l'amplada del llapis

Fem que l'usuari pugui dibuixar amb diferents mides de llapis.

+ Primer, afegeix una nova variable anomenada `amplada`{:class = "blockvariable"}.

[[[generic-scratch-add-variable]]]

+ Afegiu aquesta línia *dins * del loop `per sempre`{:class = "blockcontrol"} del codi del llapis:

```blocks
    estableix la mida del llapis a (amplada)
```

L'amplada del llapis s'establirà repetidament al valor de la variable "amplada".

+ Fes clic amb el botó dret a la visualització de la variable a l'escenari i fes clic a "control lliscant".

![captura de pantalla](images/paint-slider.png)

Ara podeu arrossegar el control lliscant per sota de la variable per canviar el seu valor.

![captura de pantalla](images/paint-slider-change.png)

+ Proveu el vostre projecte i vegeu si podeu modificar l'amplada del llapis.

![captura de pantalla](images/paint-width-test.png)

Si ho preferiu, podeu establir el valor mínim i màxim de "amplada" que està permès. Per fer-ho, feu clic amb el botó dret a la variable de nou i feu clic a "Configura el control lliscant mínim i màxim". Establiu els valors mínims i màxims de la variable a una cosa més sensible, com ara l'1 i la 20.

![captura de pantalla](images/paint-slider-max.png)

Continueu provant la vostra variable "ample" fins que estigueu contents.