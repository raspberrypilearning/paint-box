## Διόρθωσε λάθη

Μερικές φορές συμβαίνουν λάθη, οπότε πρόσθεσε ένα κουμπί "καθαρισμός" και μια γόμα.

\--- task \---

Πρόσθεσε το αντικείμενο 'X-block' από την ενότητα των γραμμάτων της βιβλιοθήκης. Χρωμάτισε την ενδυμασία του αντικειμένου με κόκκινο χρώμα και κάνε την λίγο μικρότερη. Αυτό το αντικείμενο θα είναι το κουμπί "Καθαρισμός".

[[[generic-scratch3-sprite-from-library]]]

![screenshot](images/paint-x.png)

\--- /task \---

\--- task \---

Πρόσθεσε κώδικα στο αντικείμενο "X-block" για να καθαρίσεις το Σκηνικό, όταν γίνει κλικ στο αντικείμενο.

![σταυρός](images/cross.png)

```blocks3
when this sprite clicked
erase all
```

\--- /task \---

Δεν χρειάζεται να χρησιμοποιήσεις `εκπομπή`{:class="block3events"} για να καθαρίσεις το Σκηνικό, επειδή το μπλοκ `σβήσε τα πάντα`{:class="block3extensions"} κάνει αυτή την ενέργεια.

Βλέπεις ότι το αντικείμενο μολυβιού περιλαμβάνει μια ενδυμασία γόμας;

![screenshot](images/paint-eraser-costume.png)

Το έργο σου περιλαμβάνει επίσης ένα ξεχωριστό αντικείμενο γόμας.

\--- task \---

Click on this eraser sprite and then select **show**.

![screenshot](images/show-eraser.png)

Here is how your Stage should look now:

![screenshot](images/paint-eraser-stage.png)

\--- /task \---

\--- task \---

Add code to the eraser sprite to send an `'eraser' broadcast`{:class="block3events"} when the eraser sprite is clicked.

![eraser](images/eraser.png)

```blocks3
όταν γίνει κλικ σε αυτό το αντικείμενο
μετάδωσε (γόμα v)
```

\--- /task \---

When the pencil sprite receives the 'eraser' message, it should switch its costume to the eraser and switch the pen colour to white, which is the same colour as the Stage!

\--- task \---

Add some code to create the eraser.

\--- hints \--- \--- hint \---

Add some code to the pencil sprite: `When I receive`{:class="block3events"} the `eraser`{:class="block3events"} message `Switch to costume eraser`{:class="block3looks"} `Set pen color`{:class="block3extensions"} to white

\--- /hint \--- \--- hint \---

Here are all the blocks you need:

```blocks3
όρισε χρώμα πένας σε [#FFFFFF]

όταν λάβω [γόμα v]

άλλαξε ενδυμασία σε (γόμα v)
```

\--- /hint \--- \--- hint \---

Here is what the code should look like:

![pencil](images/pencil.png)

```blocks3
όταν λάβω [γόμα v]
άλλαξε ενδυμασία σε (γόμα v)
όρισε χρώμα πένας σε [#FFFFFF]
```

\--- /hint \--- \--- /hints \--- \--- /task \---

\--- task \---

Test your project to see if you can clear the Stage and erase pencil lines.

![screenshot](images/paint-erase-test.png)

\--- /task \---

There's one more problem with the pencil: you can draw anywhere on the Stage, including near the 'clear' and eraser buttons!

![screenshot](images/paint-draw-problem.png)

\--- task \---

To fix this, change the code so that the pen is only down if the mouse is clicked **and** the `y` position of the mouse pointer is greater than `-120`:

![pencil](images/pencil.png)

```blocks3
όταν στην πράσινη σημαία γίνει κλικ
καθάρισέ τα  όλα
άλλαξε ενδυμασία σε (μολύβι-μπλε v)
όρισε χρώμα πένας σε [#0035FF]
για πάντα 
  πήγαινε σε (mouse pointer v)
  + εάν <<mouse down?> και <(y ποντικιού) > [-120]>>> τότε 
  +   κατέβασε πένα
  + αλλιώς 
  +   σήκωσε πένα
  + end
end
```

\--- /task \---

\--- task \---

Test your project. You now should not be able to draw near the buttons.

![screenshot](images/paint-fixed.png)

\--- /task \---