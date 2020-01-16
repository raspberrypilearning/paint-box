## Άλλαξε το πάχος του μολυβιού

Στη συνέχεια, θα προσθέσεις κώδικα για να επιτρέψεις στο άτομο που χρησιμοποιεί το πρόγραμμά σου να σχεδιάζει πράγματα με διαφορετικό πάχος μολυβιού.

\--- task \---

First, add a new variable called `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Add this line **inside** the `forever`{:class="block3control"} loop of the pencil sprite's code:

```blocks3
όταν στην πράσινη σημαία γίνει κλικ
καθάρισε τα πάντα
άλλαξε ενδυμασία σε (μολύβι-μπλε v)
όρισε χρώμα πένας σε [#0035FF]
για πάντα 
  πήγαινε σε (mouse pointer v)
  + όρισε μέγεθος πένας σε (width :: variables)
  εάν <<mouse down?> και <(y ποντικιού) > [-120]>> τότε 
    κατέβασε πένα
  αλλιώς 
    σήκωσε πένα
  end
```

\--- /task \---

The pen width now repeatedly gets set to the value of the `width`{:class="block3variables"} variable.

\--- task \---

Right-click on the `width`{:class="block3variables"} variable displayed on the Stage, and then click on **slider**.

![screenshot](images/paint-slider.png)

\--- /task \---

You can now drag the slider that is visible below the variable to change the variable's value.

![screenshot](images/paint-slider-change.png)

\--- task \---

Test your project and see if you can add code to adjust the pen width.

![screenshot](images/paint-width-test.png)

\--- /task \---