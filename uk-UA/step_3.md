## Створюємо олівець

Почнемо з того, що створимо олівець, який можна використати, щоб намалювати сцену.

+ Відкрийте проект "Scratch" "Paintbox" в Інтернеті на  jumpto.cc/paint-go </ 0> (: target = "_ blank") або завантажте з  http://jumpto.cc/paint-get </ 1> {: target = "_ blank"}, а потім відкрийте його, якщо ви користуєтесь редактором в режимі офлайн.</li> </ul> 
    
    Ви побачите олівець і гумку:
    
    ![скріншот](images/paint-starter.png)
    
    + Add some code to the pencil sprite to make it follow the mouse `forever`{:class="blockcontrol"} so that you can draw:
    
    ```blocks
        коли натиснуто прапорець
         назавжди
           перейти до [курсор миші v]
         кінець
    ```
    
    + Натисніть на прапорець, а потім перемістіть курсор миші на сцену, щоб перевірити, чи працює код.
    
    Наступний крок, давайте зробимо так,щоб наш олівець малював `if`{:class="blockcontrol"}, при натисканні мишки.
    
    + Додайте цей код до вашого олівця:
    
    ![скріншот](images/paint-pencil-draw-code.png)
    
    + Перевірте свій код ще раз. На цей раз, перемістіть олівець навколо сцени і утримуйте кнопку миші. Чи можете ви малювати олівцем?
    
    ![скріншот](images/paint-draw.png)
    
    ## \--- collapse \---
    
    ## заголовок: Якщо у вас виникли проблеми...
    
    Якщо ви помітили, що олівець малює лінію з середини, а не кінчика, вам доведеться змінити центр.
    
    ![Costume center](images/costume-center.png)
    
    Перетин олівця слід розмістити ** трохи нижче ** кінчика олівця, але не на самому кінці.
    
    A changes in a sprite's 'costume center' isn't registered until another tab is clicked, so click on another costume, or on the 'Scripts' tab to finalise your changes to the costume center.
    
    \---collapse\---