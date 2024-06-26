## التراجع عن الأخطاء

أحيانًا تحدث أخطاء أثناء الرسم، لذلك سنضيف زر 'مسح' و زر للممحاة.

--- task ---

أضف كائن Block-X من قسم حروف في مكتبة الكائنات. لون مظهر الكائن باللون الأحمر و صغر حجمه قليلاً. هذا الكائن سيكون زر 'مسح'.

[[[generic-scratch3-sprite-from-library]]]

![لقطة الشاشة](images/paint-x.png)

--- /task ---

--- task ---

أضف التعليمة البرمجية التالية إلى كائن 'X-block' لمسح منصة العمل عندما يتم النقر على هذا الكائن.

![block-X](images/cross.png)

```blocks3
when this sprite clicked
erase all
```

--- /task ---

لا تحتاج إلى استخدام `بث`{:class="block3events"} لمسح كامل محتويات منصة العمل, لأن كتلة `مسح الكل`{:class="block3extensions"} تقوم بهذه العملية.

هل لاحظت بأن كائن القلم الرصاص يحتوي على مظهر للممحاة؟

![لقطة الشاشة](images/paint-eraser-costume.png)

يحتوي مشروعك على كائن منفصل للممحاة.

--- task ---

انقر على هذه الممحاة ثم حدد **إظهار**.

![لقطة الشاشة](images/show-eraser.png)

سيكون شكل المنصة كما يلي:

![لقطة الشاشة](images/paint-eraser-stage.png)

--- /task ---

--- task ---

أضف هذه التعليمة البرمجية لكائن الممحاة لبث `رسالة 'مسح'`{:class="block3events"} عندما يتم النقر على كائن الممحاة.

![الممحاة](images/eraser.png)

```blocks3
when this sprite clicked
broadcast (الممحاة v)
```

--- /task ---

عندما يتلقى كائن القلم الرصاص رسالة "مسح"، فيفترض أن يقوم بتحويل مظهره إلى مظهر الممحاة، وتحويل لون القلم إلى اللون الأبيض، أي نفس لون منصة العمل!

--- task ---

أضف بعض التعليمات البرمجية لإنشاء الممحاة.

--- hints ---
--- hint ---

أضف بعض التعليمات البرمجية إلى كائن قلم الرصاص: `عندما اتلقى`{:class="block3events"} رسالة `مسح`{:class="block3events"} `غير المظهر الى ممحاة`{:class="block3looks"} `اجعل لون القلم مساوياً`{:class="block3extensions"} إلى الأبيض

--- /hint ---
--- hint ---

إليك جميع الكتل التي تحتاجها:

```blocks3
set pen color to [#FFFFFF]
when I receive [الممحاة v]

switch costume to (الممحاة v)
```

--- /hint ---
--- hint ---

و هذا ما يجب أن تبدو عليه التعليمات البرمجية الخاصة بك:

![قلم رصاص](images/pencil.png)

```blocks3
when I receive [الممحاة v]
switch costume to (الممحاة v)
set pen color to [#FFFFFF]
```

--- /hint ---
--- /hints ---
--- /task ---

--- task ---

اختبر مشروعك لترى هل يمكنك مسح كامل محتويات منصة العمل و هل يمكنك مسح كتابات القلم.

![لقطة الشاشة](images/paint-erase-test.png)

--- /task ---

توجد مشكلة واحدة آخرى بالنسبة إلى القلم: هل لاحظت أنه يمكنك أن ترسم في أي مكان على منصة العمل حتى بالقرب من زر 'مسح' و زر 'الممحاة'!

![لقطة الشاشة](images/paint-draw-problem.png)

--- task ---

لحل هذه المشكلة, غير التعليمات البرمجية بحيث يكون القلم في حالة كتابة فقط إذا تم النقر بالماوس **و** كان `موقع ص` للماوس أكبر من `-120`:

![قلم رصاص](images/pencil.png)

```blocks3
when flag clicked
erase all
switch costume to (قلم رصاص أزرق v)
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

اختبر مشروعك. الآن بعد حل المشكلة يفترض أنك غير قادر على الرسم بجوار الأزرار الموجودة على منصة العمل.

![لقطة الشاشة](images/paint-fixed.png)

--- /task ---