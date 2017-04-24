## Sound the alert when we've run out of shelf space!

#### Step 1:

Start a new program (Create Code -> Blocks editor).

#### Step 2:
Create a variable to keep track of the available shelf space in an aisle. By default any variable will be 0 at start, which is fine for now but maybe you want to start with the number of available shelfs.

Hint: "Variables" menu item.

#### Step 3:
Get the spaces variable to show on the LED pixel display.

Hint: "Basic" menu item.

#### Step 4:
Obviously, we need a way to change that variable. Let's make button A increase the value, and button B decrease. Make sure that the display updates accordingly.

Hint: "Input" menu item.

#### Step 4a:
What happens if you press B when the indicator is already at 0? Negative space is obviously not what we want. Modify your program so that it never drops below 0.

Hint: Use an "if-do conditional" found under "Logic" menu item.

#### Step 4b:
It might be a good idea to let people know that they've tried to do something that can't be done. Modify your program so that when pressing B while the available space is 0, the buzzer sounds.

Hint: Modify the "if-do conditional" to have an else block via the settings / gear icon.

#### Step 5:
What happens if you keep pressing A? There's only so many space available in real life, so let's modify your program so that it can't go over a certain amount.

Hint: Use an "if-do conditional" found under "Logic" menu item.

#### Step 6:
When there's more than 9 spaces available, the display starts scrolling, and it's harder to see that at a glance. Experiment with other ways of displaying this information.

Hint: Look at the "plot bar graph" command under the "LED" section.
