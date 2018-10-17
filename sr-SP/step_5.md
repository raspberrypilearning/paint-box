## Грешке

Понекад се дешавају грешке, па хајде да додамо дугме 'обриши' и гумицу.

+ Додај лик 'Х-блок'. Наћи ћеш га у библиотеци, у одељку "Слова". Обоји костим у црвено. То ће постати дугме 'обриши'.

![слика екрана](images/paint-x.png)

+ Додај код овом лику да обрише позорницу када се кликне на њега.

![Обриши позорницу](images/clear-stage.png)

Notice that you don't need to send a message to clear the stage, you can just use the clear block from this sprite.

Вероватно си приметио/ла да твој лик оловке има костим гумице:

![слика екрана](images/paint-eraser-costume.png)

+ Твој пројекат такође има посебан лик гумице. Кликни десним тастером миша на њега и изабери 'прикажи'. Твоја позорница би требало да изгледа овако:

![слика екрана](images/paint-eraser-stage.png)

+ Add code to the eraser sprite, to tell the pencil to switch to an eraser when the sprite is clicked.

![Разгласи гумица](images/broadcast-eraser.png)

When the pencil receives the "eraser" message, you can switch the pencil costume to the eraser, and switch the pencil colour to white - the same colour as the stage!

+ Add some code to create the eraser

\--- hints \--- \--- hint \--- Додај код лику оловке: **Када примим** поруку **гумица** **Замени костим са** гумица **Нека боја оловке буде** бела \--- /hint \--- \--- hint \--- Ево како би требало да изгледа код унутар лика оловке:

```blocks
када примим [гумица v]
замени костим са [гумица v]
нека боја оловке буде [#FFFFFF]
```

\--- /hint \--- \--- /hints \---

+ Испробај свој пројекат да провериш да ли можеш да бришеш на позорници.

![слика екрана](images/paint-erase-test.png)

Постоји још један проблем са оловком - можеш да црташ било где на позорници, укључујући и близу икона за избор!

![слика екрана](images/paint-draw-problem.png)

Да то поправиш, мораш да кажеш оловци да црта само ако је миш кликнут *и* ако је y-координата миша већа од -120:

![слика екрана](images/pencil-gt-code.png)

+ Испробај пројекат; сада не би требало да можеш да црташ близу блокова за избор.

![слика екрана](images/paint-fixed.png)