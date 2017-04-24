

SHELF SPACE
===========

From here on there'd be more of a description of the task, rather than tips on how to get there. I think these steps would kind of logically follow each other. I like how e.g. with step 3 there's the discovery of an edge case that's not handled, which is pretty much how programming often is in real life too.

Step 0: start a new program (projects -> new).

Step 1:
Create a variable to keep track of the available shelf space in an aisle. By default any variable will be 0 at start, which is fine for now. Get this to display on the pixel display.

Step 2:
Obviously, we need a way to change that variable. Let's make button A increase the value, and button B decrease. Make sure that the display updates accordingly.

Step 3a:
What happens if you press B when the indicator is already at 0? Negative space is obviously not what we want. Modify your program so that it never drops below 0 (using an if-then conditional found under Logic).

Step 3b:
It might be a good idea to let people know that they've tried to do something that can't be done. Modify your program so that when pressing B while the available space is 0, the buzzer sounds.

Step 4:
What happens if you keep pressing A? There's only so many space available in real life, so let's modify your program so that it can't go over a certain amount.

Step 5:
When there's more than 9 spaces available, the display starts scrolling, and it's harder to see that at a glance. Experiment with other ways of displaying this information. Look at the "plot bar graph" command under the "LED" section.
