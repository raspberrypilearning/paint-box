## Gwneud camgymeriadau

Weithiau mae camgymeriadau yn digwydd, felly fe wnawn ni ychwanegu botwm 'clirio' a dileuwr i dy brosiect!

+ Fe wnawn ni ychwanegu botwm i glirio'r llwyfan. I wneud hyn, ychwanega'r ciplun llythyren 'X-block' i'r llwyfan, a lliwia fe'n goch.

	![screenshot](images/paint-x.png)

+ Ychwanega côd i'r botwm dileu i glirio'r llwyfan pan mae'n cael ei glicio.

	```blocks
		pan caiff y cymeriad ei glicio
		clirio
	```

	Sylwa nad oes angen i ti anfon neges i glirio'r llwyfan, gan fod unrhyw giplun yn gallu gwneud!

+ Rwyt ti siwr o fod wedi sylwi bod ciplun dy bensil yn cynnwys gwisg dileuwr:

	![screenshot](images/paint-eraser-costume.png)
	

+ Mae dy brosiect hefyd yn cynnwys ciplun dewisydd dileuwr, gwna clic dde arno a dewis 'dangos'. Dyma sut ddylsai dy lwyfan edrych:

	![screenshot](images/paint-eraser-stage.png)

+ Mae modd i ti nawr ychwanegu côd i'r ciplun dileuwr, i ddweud wrth y pensil i newid i'r dileuwr.

	```blocks
		pan caiff y cymeriad ei glicio
		darlledu [eraser v]
	```

+ Pan mae'r pensil yn derbyn y neges yma, alli di greu dileuwr trwy newid gwisg y pensil i fod yn ddileuwr, a newid lliw y pensil i fod yr un lliw â'r llwyfan!

	```blocks
		pan fyddaf yn derbyn [eraser v]
		newid i wisg [eraser v]
		gosod lliw pin i [#FFFFFF]

	```

+ Profa dy brosiect, i weld os wyt ti'n gallu clirio a dileu y llwyfan.

	![screenshot](images/paint-erase-test.png)

+ Mae yna un problem arall gyda'r pensil - mae modd i ti dynnu llun unrhywle ar y llwyfan, yn cynnwys eicon y dewisydd!

	![screenshot](images/paint-draw-problem.png)

	I ddatrys hyn, mae angen i ti ddweud wrth y pensil i dynnu llun os yw'r llygoden wedi clicio _ac_os mae y-position y llygoden yn fwy na -120 (`llygoden y`{.blocksensing}`> -120` {.blockoperators}).
	Newida datganiad 'os' {.blockcontrol} y pensil i edrych fel hyn:

	![screenshot](images/pencil-gt-code.png)

+ Profa dy brosiect, nawr ni ddyle ti allu tynnu llun yn agos i'r blociau dewis.

	![screenshot](images/paint-fixed.png)



