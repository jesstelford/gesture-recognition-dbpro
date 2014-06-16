# [[DBP] Discrete Handwriting (Gesture) Recognition](http://forum.thegamecreators.com/?m=forum_view&t=82264&b=6)

First up, What is Gesture Recognition?

Well, basically, it is a method whereby the computer can match one continuous user-inputed stroke with a pre-defined stroke and rate it on its accuracy (-1 to 1).

`save.sav` is a sample Gestures Save file (yes, you can make your own)

Basically, follow the isntructions in the app.
When viewing stored gestures, the bigger red square/circle is the starting point for drawing (if you do it backwards, it wont be recognized!).

It's not fool-proof, so if you have two gestures that are similar, it'll pick the best match (maybe not what you wanted, but mathmatically, its choice is correct).

There are accuracy settings available also.
pointsPerStroke - is how smooth the gesture has to be - Lower the value for better recognition, raising it will force the user to be more accurate.
scaleSize - because this is a prototype, and the final is intended for a system that has no FPU (can't handle Float's very well), I made it so that it stored the final gesture as a series of integers. The higher this value, the more accurate the final stored gesture is (not that it matters, since by putting it up to, say, 1000, you would only be gaining about 1px more of accuracy!)

The original is taken from an article by Oleg Dopertchouk - [Recognition of Handwritten Gestures](http://www.gamedev.net/reference/articles/article2039.asp).
