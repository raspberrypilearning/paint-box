## কলমের প্রস্থ পরিবর্তন করুন

এর পরে আপনি আপনার প্রোগ্রামটি ব্যবহার করছেন কলমের বিভিন্ন প্রস্থের দ্বারা বিভিন্ন জিনিস আঁকতে অনুমতি দেওয়ার জন্য। তার জন্য যে কোড যুক্ত করবেন।.

\--- task \---

প্রথমে যে নতুন variable যোগ করবেন `width`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

**inside** the `forever`{:class="block3control"} পেন্সিল sprite কোডের এই লাইন লুপটি যুক্ত করুন:

```blocks3
when flag clicked
erase all
switch costume to (pencil-blue v)
set pen color to [#0035FF]
forever
go to (mouse pointer v)
+set pen size to (width :: variables)
if <<mouse down?> and <(mouse y) > [-120]>> then 
  pen down
  else
  pen up
end
```

\--- /task \---

কলমের প্রস্থ এখন variable এর মান হিসাবে সেট হয়ে যাবে: `width`{:class="block3variables"}.

\--- task \---

Right-click করুন `width`{:class="block3variables"} variable টি স্টেজে আসলে ক্লিক করুন **slider**.

![screenshot](images/paint-slider.png)

\--- /task \---

Variable এর মান পরিবর্তন করতে আপনি এখন স্লাইডারটি টেনে আনতে পারেন যা variable এর নীচে দৃশ্যমান।.

![screenshot](images/paint-slider-change.png)

\--- task \---

আপনার প্রকল্পটি পরীক্ষা করুন এবং দেখুন যে আপনি কলমের প্রস্থ সামঞ্জস্য করতে কোড যুক্ত করতে পারেন কিনা।.

![screenshot](images/paint-width-test.png)

\--- /task \---