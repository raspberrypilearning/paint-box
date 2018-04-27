## Värikynät

Lisätään projektin eri värikynät ja annamme käyttäjän valita niiden välillä.

+ Napsauta kynän sprite, napsauta "Puvut" ja kopioi kynänsininen puku.

![kuvakaappaus](images/paint-blue-duplicate.png)

+ Nimeä uusi puku "kynänvihreä" ja väritä kynänvihreä.

![kuvakaappaus](images/paint-pencil-green.png)

[[[generic-scratch-rename-sprite]]]

+ Piirrä kaksi uutta sprites - yksi sininen neliö ja yksi vihreä neliö. Käytät näitä valitaksesi sinisen tai vihreän kynän.

![kuvakaappaus](images/paint-selectors.png)

+ Nimeä nuolet uudelleen niin, että niitä kutsutaan "siniseksi" ja "vihreiksi"

+ Lisää koodi "vihreään" spriteeseen niin, että kun sitä napsautetaan, `lähettää`{: class = "blockevents"} viestin "vihreä" kynän spriteille ja kertoo sen muuttavan puku- ja lyijykynän väriä.

![Broadcast vihreä](images/paint-broadcast-green.png)

[[[generic-scratch-broadcast-message]]]

+ Vaihda kynän spriteeseen. Lisää jonkinlainen koodi niin, että kun tämä sprite saa `lähetyksen`{: class = "blockevents"} vihreällä, sen pitäisi vaihtaa vihreä kynän puku ja vaihtaa kynän väri vihreäksi.

![Broadcast vihreä](images/broadcast-green.png)

Jos haluat asettaa kynän väriksi vihreiksi, napsauta värillistä laatikkoa `setin kynänvärillä`{: class = "blockpen"} ja napsauta vihreää spriteä valitsemalla sama väri vihreä kuin kynän väri.

+ Nyt voit tehdä saman sinisen kynän kuvakkeen: lisää tämä koodi siniselle neliön sprite:

```blocks
kun tämä sprite napsautti lähetystä [sininen v]
```

... ja lisää tämä koodi pencil sprite:

```blocks
kun saan [sininen v] kytkin puku [kynänsininen v] asetettu kynän väri [# 0000ff]
```

+ Lopuksi, lisää tämä koodi ilmoittamaan kynän sprite, joka väri alkaa ja varmista, että näyttö on selvä.

![Aloita lyijykynä](images/start-pencil.png)

Päätimme aloittaa sinisellä, mutta jos haluat, voit aloittaa eri värikynällä.

+ Testaa projektisi. Voitko vaihtaa sinisiä ja vihreitä kynää napsauttamalla sinisiä tai vihreitä neliölehtiä?

![kuvakaappaus](images/paint-pens-test.png)