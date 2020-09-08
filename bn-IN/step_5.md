## ভ্রম সংশোধন

কখনও কখনও ভুল হয়, সুতরাং একটি 'clear' button এবং একটি eraser button যুক্ত করুন।.

--- task ---

গ্রন্থাগার বা library এর অক্ষর বিভাগ থেকে 'X-Block' sprite যুক্ত করুন।. Sprite এর costume টি লালচে করে কিছুটা ছোট করুন।. এই Sprite টি হল 'clear' বোতাম।.

[[[generic-scratch3-sprite-from-library]]]

![screenshot](images/paint-x.png)

--- /task ---

--- task ---

Sprite ক্লিক করা হলে স্টেজটি সাফ করতে 'X-Block' sprite এ কোড যুক্ত করুন।.

![cross](images/cross.png)

```blocks3
when this sprite clicked
erase all
```

--- /task ---

আপনার `broadcast`{:class="block3events"} ব্যবহার করার দরকার নেই পর্যায়টি সাফ করার জন্য, `erase all`{:class="block3extensions"} block কাজটি করে।.

আপনি কি পেনসিল sprite টি একটি ইরেজার costume এর অন্তর্ভুক্ত তা দেখতে পান?

![screenshot](images/paint-eraser-costume.png)

আপনার প্রকল্পে একটি পৃথক ইরেজার sprite রয়েছে।.

--- task ---

এই ইরেজার sprite এ ডান ক্লিক করুন এবং তারপরে **show** ক্লিক করুন ।. আপনার কোডটি দেখতে কেমন হবে তা এখানে দেওয়া হলো:

![screenshot](images/paint-eraser-stage.png)

--- /task ---

--- task ---

`'eraser' broadcast`{:class="block3events"} সম্প্রচার পাঠাতে ইরেজার sprite এ কোড যুক্ত করুন, যখন ইরেজার sprite ক্লিক করা হয়।.

![eraser](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (eraser v)
```

--- /task ---

পেন্সিল sprite যখন 'ইরেজার/eraser' বার্তাটি গ্রহণ করবে, তখন এটির costume টি ইরেজারে স্যুইচ করা উচিত এবং পেনের রঙটি সাদাতে পরিবর্তন করা উচিত, যা স্টেজের মতো রঙ!

--- task ---

ইরেজার তৈরি করতে কিছু কোড যুক্ত করুন।.

--- hints ---
 --- hint ---

পেন্সিল sprite এ কিছু কোড যুক্ত করুন: `When I receive`{:class="block3events"} the `eraser`{:class="block3events"} message `Switch to costume eraser`{:class="block3looks"} `Set pen color`{:class="block3extensions"} to white

--- /hint --- --- hint ---

আপনার প্রয়োজনীয় কোড block গুলি এখানে রইল:

```blocks3
set pen color to [#FFFFFF]
when I receive [eraser v]

switch costume to (eraser v)
```

--- /hint --- --- hint ---

আপনার কোডটি দেখতে এমন হওয়া উচিত:

![pencil](images/pencil.png)

```blocks3
when I receive [eraser v]
switch costume to (eraser v)
set pen color to [#FFFFFF]
```

--- /hint ------ /hints --- --- /task ---

--- task ---

আপনি পর্যায়/stage সাফ করতে এবং পেন্সিল লাইনগুলি মুছতে পারেন কিনা তা দেখতে আপনার প্রকল্পটি পরীক্ষা করুন।.

![screenshot](images/paint-erase-test.png)

--- /task ---

পেন্সিল নিয়ে আরও একটি সমস্যা রয়েছে: আপনি ক্লিয়ার/clear এবং ইরেজার/eraser বোতামগুলির নিকটবর্তী স্টেজের যে কোনও জায়গায় আঁকতে পারেন!

![screenshot](images/paint-draw-problem.png)

--- task ---

এটি ঠিক করতে কোডটি পরিবর্তন করুন যাতে মাউস ক্লিক করলে তবেই কলমটি নীচে নামে ও **and** `y` মাউস পয়েন্টারের অবস্থান `-120` এর চাইতে বেশি হয়:

![pencil](images/pencil.png)

```blocks3
when flag clicked
erase all
switch costume to (pencil-blue v)
set pen color to [#0035FF]
forever
  go to (mouse pointer v)
+if <<mouse down?> and <(mouse y) > [-120]>> then 
  pen down
  else
  pen up
end
```

--- /task ---

--- task ---

আপনার প্রজেক্ট পরীক্ষা করুন. আপনি এখন বোতামগুলির কাছাকাছি আঁকতে সক্ষম হবেন না।.

![screenshot](images/paint-fixed.png)

--- /task ---