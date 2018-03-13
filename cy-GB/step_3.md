## Pensiliau lliw

Awn ati i ychwanegu pensiliau lliw gwahanol i dy brosiect, a gadael i'r defnyddiwr ddewis rhyngddyn nhw!

+ Clicia ar giplun y pensil, clicia 'Gwisgoedd' a cer ati i ddyblygu gwisg 'pencil-blue'.

	![screenshot](images/paint-blue-duplicate.png)

+ Ail-enwa dy wisg newydd yn 'pensil-gwyrdd', a lliwia'r pensil yn wyrdd.

	![screenshot](images/paint-pencil-green.png)

+ Nesaf, bydd angen creu dau giplun newydd, a byddi di'n defnyddio rhain i ddewis y pensil glas neu gwyrdd.

	![screenshot](images/paint-selectors.png)

+ Pan mae'r eicon gwyrdd wedi ei ddewis, bydd angen i ti 'ddarlledu' {.blockevents} neges i'r ciplun pensil, yn dweud wrtho i newid ei wisg a'r lliw pensil.

	I wneud hyn, yn gyntaf ychwanega y côd yma i'r eicon gwyrdd:

	```blocks
		pan caiff y cymeriad ei glicio
		darlledu [gwyrdd v]
	```

	I greu y bloc 'darlledu' {.blockevents}, clicia'r saeth lawr a dewisa 'neges newydd...'

	![screenshot](images/paint-broadcast.png)

	Galli di wedyn deipio 'gwyrdd' i greu dy neges newydd.

	![screenshot](images/paint-green-message.png)

+ Mae angen i ti nawr ddweud wrth y ciplun pensil beth i wneud pan mae'n derbyn y neges. Ychwanega'r côd yma i dy giplun pensil:

	```blocks
		pan fyddaf yn derbyn [gwyrdd v]
		newid i wisg [pensil-gwyrdd v]
		gosod lliw pin i [#00ff00]

	```

	I osod dy bensil i liwio yn wyrdd, clicia'r bocs lliw yn y bloc 'gosod lliw' {.blockpen}, a clicia ar yr eicon dewisydd gwyrdd.

+ Cer ati i wneud yr un peth ar gyfer yr eicon pensil glas, gan ychwanegu'r côd yma i dy giplun dewisydd glas:

	```blocks
		pan caiff y cymeriad ei glicio
		darlledu [glas v]

	```
	...ac ychwanegu'r côd yma i'r ciplun pensil: 

	```blocks
		pan fyddaf yn derbyn [glas v]
		newid i wisg [pensil-glas v]
		gosod lliw pin i [#0000ff]
	```

+ Yn olaf, mae angen i ti ddweud wrth ciplun dy bensil pa wisg a lliw pensil i ddewis, ac i glirio'r sgrin pan mae'r prosiect wedi cychwyn. Ychwanega'r côd yma i ddechrau côd y pensil 'pan mae baner wedi ei glicio' {.blockevents} (cyn y ddolen 'am byth' {.blockcontrol}):

	```blocks
		clirio
		newid i wisg [pensil-glas v]
		gosod lliw pin i [#0000ff]

	```

	Os oes well gyda ti, galli di ddechrau gyda phensil lliw gwahanol!

+ Profa dy brosiect. Alli di newid rhwng pensiliau glas a gwyrdd?

	![screenshot](images/paint-pens-test.png)



