## Make the Buzzer go off!

#### Step 1:
Clip one of the crocodile clips to one of the legs of the buzzer and the other end of the clip to the pad marked "0" on the BBC Micro:bit. Use the other crocodile clip to connect the other leg to the Micro:bit pad marked "GND".

![Connecting your buzzer](https://github.com/camallen/unipart_bbc_microbit/blob/master/images/clips_microbit.png "Connecting your buzzer")

#### Step 2:
Under the "Music" section there's a block labeled "play tone". Put this into the "forever" block that's already in your program.

#### Step 3:
Notice this "Middle C"? Some blocks have parameters that you can change, or hook up to other things.

For instance, you could take many of the blocks from "Input" and hook them up:

Notice how the pitch of the buzzer goes up when you shake your BBC Micro:bit?

####  Step 4:
You can also use variables<sup>1</sup>.
Drag the item variable into the tone pitch parameter. Now from the Input section, add an "on button A pressed" block into your program. This one doesn't attach into "Forever" but is it's own thing. Inside this new block, change the variable with a "change item by 50" block. You can also rename "item" to something more descriptive like "pitch".

Now every time you press the A button, the pitch will go up.
____

<sup>**1**</sup> **Variables**: are place holders for changing values. Use them in your code to dynamically refer to their latest assigned value.

Pro tip: try to name them so they mean something when you read the code :)
``` ruby
box_count = 0
print "Box count is currently: " + box_count
# outputs Box count is currently: 0

box_count = box_count + 10

print "Box count is currently: " + box_count
# outputs Box count is currently: 10
```
