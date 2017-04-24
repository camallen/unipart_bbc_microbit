## Make the Buzzer go off!

Let's write the code to make the buzzer go off. Once we've written it, we'll make it run on our Micro:bits.

#### Step 1:
Clip one of the crocodile clips to one of the legs of the buzzer and the other end of the clip to the pad marked "0" on the BBC Micro:bit. Use the other crocodile clip to connect the other leg to the Micro:bit pad marked "GND".

![Connecting your buzzer](https://github.com/camallen/unipart_bbc_microbit/blob/master/images/clips_microbit.png "Connecting your buzzer")

#### Step 2:
Make the Micro:bit constantly do something. Under the "Basic" section there's a block labeled "forever". Click this to activate it in your code.

![Do something forever](https://github.com/camallen/unipart_bbc_microbit/blob/master/images/forever.png "Do something forever")

#### Step 3:
Under the "Music" section there's a block labeled "play tone". Put this into the "forever" block that's already in your program.

![Play a tone](https://github.com/camallen/unipart_bbc_microbit/blob/master/images/middle_C.png "Play a tone")

#### Step 4:
Notice this "C"? Some blocks have parameters that you can change, or hook up to other things.

Let's try and use a different input source. How about we try using the accelerometer?

![Choose a block to wire up](https://github.com/camallen/unipart_bbc_microbit/blob/master/images/choose_block_inputs.png "Choose a block to wire up")

For instance, press "Input" menu and then click the "acceleration (mg)" block and drag it to replace the "C" block in "play tone".

![Dynamic tones](https://github.com/camallen/unipart_bbc_microbit/blob/master/images/play_tone.png "Dynamic tones")

Notice how the pitch of the buzzer goes up when you shake your BBC Micro:bit a certain direction? This is what we call an edge case, we need to ignore negative acceleration values!

Select the "Math" menu and select the "absolute of" block and drag it wrap the acceleration input block. For those wondering, this maths block will ignore negative values and turn them positive.

![Dynamic tones](https://github.com/camallen/unipart_bbc_microbit/blob/master/images/play_tone_abs.png "Dynamic tones")

####  Step 5:
You can also use variables. Variables are place holders for changing values. Use them in your code to refer to their latest value.

*Pro tip: try to name them so they mean something when you read the code :)*

Select "Variables" from the menu and drag the "Item" block to replace the "acceleration (mg)" block. Now from the Input section, add an "on button A pressed" block anywhere into your program. Note: This one doesn't attach into "Forever" but is it's own thing.

Inside this new block, add a "change item by 1" block. You can modify the change amount value to 50 and also rename "item" to something more descriptive like "pitch".

![Button pitch change](https://github.com/camallen/unipart_bbc_microbit/blob/master/images/button_pitch_change.png "Button pitch change")

Now every time you press the A button, the pitch will go up. Also note that you can

####  Step 6:
**Make the code run on the Micro:bit**
Once we're happy with the code, We need to make it run on the Micro:bit.

Press the "Compile" button to download a runnable '\*.hex' file. Then drag this to the BBC Micro:bit device location on your PC.

**Ask for help** or see https://www.microbit.co.uk/device/usb for more detailed instructions on how to download and run code on the Micro:bit.
