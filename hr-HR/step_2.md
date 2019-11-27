## Napravite olovku

Započnite izradom olovke koju možete koristiti za crtanje na pozornici.

\--- zadatak \--- Otvorite početni projekt Scratch "Paint box".

**Online**: otvorite početni projekt na [rpf.io/paint-box-on](http://rpf.io/paint-box-on){:target="_blank"}

Ako imaš Scratch korisnički račun, možeš napraviti kopiju klikom na **Remix**.

**Offline**: otvorite [starter project](http://rpf.io/p/en/paint-box-go){:target="_blank"} u offline editoru.

Ako trebaš preuzeti i instalirati offline Scratch uređivač, to možeš napraviti na [rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}

U projektu pokretanja trebali biste vidjeti olovke i gumice za likove:

![screenshot](images/paint-starter.png) \--- /task \---

\--- task \---

Dodajte proširenje olovke svom projektu.

[[[generic-scratch3-add-pen-extension]]]

\--- /task \---

\--- task \---

Dodajte kod liku olovke ako da lik slijedi strelicu miša `forever`{:class="block3control"} te da možete crtati:

![pencil](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)
end
```

\--- /task \---

\--- task \--- Click the flag and then move the mouse pointer around the Stage to test whether your code works. \--- /task \---

Zatim, napravite da olovku samo crta `if` {: class = "block3control"} klikne se na tipku miša.

\--- task \--- Dodajte ovaj kôd liku okovke:

![pencil](images/pencil.png)

```blocks3
when flag clicked
forever
  go to (mouse pointer v)

+ if <mouse down?> then
  pen down
  else
  pen up
end
```

\--- /task \---

\--- task \--- Ponovno testiraj svoj kôd. Ovaj put, pomičite olovku oko pozornice i držite gumb miša. Možete li crtati olovkom?

![screenshot](images/paint-draw.png) \--- /task \---

## \--- collapse \---

## naslov: Crta li vaša olovka sa svog vrha?

Ako linija na kojoj crtate olovkom izgleda kao da dolazi iz sredine olovke, morate promijeniti lik olovke tako da je vrh središta lika.

Kliknite lik olovke, a zatim kliknite **Costumes** karticu.

Pomaknite kostim tako da vrh olovke bude **just above** središta.

![Costume center](images/costume-center-annotated.png)

Sada pomičite olovku na pozornici i crtajte. Olovka bi sada trebala povući crtu od svog vrha.

\--- /collapse \---