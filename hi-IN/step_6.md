## पेंसिल की चौड़ाई बदलना

Let's allow the user to draw using a range of different pencil sizes.

+ पहले, `चौड़ाई`{:class="blockvariable"} नामक नया वेरिएबल जोड़े।

[[[generic-scratch-add-variable]]]

+ इस लाइन को अपनी पेंसिल के कोड `हमेशा के लिए(forever)`{:class="blockcontrol"} लूप के*अंदर* जोड़ें:

```blocks
    पेन का अाकार (चौड़ाई) पर सेट करे
```

पेंसिल की चौड़ाई अब बार-बार 'चौड़ाई' वेरिएबल(variable) के मान पर सेट की जाएगी।

+ Right click on the variable display on the stage and click 'slider'.

![screenshot](images/paint-slider.png)

You can now drag the slider below the variable to change its value.

![screenshot](images/paint-slider-change.png)

+ Test your project, and see if you can modify the pencil width.

![screenshot](images/paint-width-test.png)

If you prefer, you can set the minimum and maximum value of 'width' that's allowed. To do this, right-click on the variable again and click 'set slider min and max'. Set the minimum and maximum values of your variable to something more sensible, like 1 and 20.

![screenshot](images/paint-slider-max.png)

Keep testing your 'width' variable until you're happy.