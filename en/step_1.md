This is a **Discover** project, this project will help you explore what the **micro:bit** can do and decide whether you want to learn more. 

### What you will make

Do you ever find yourself wondering what to do with your free time? You can use the micro:bit to help you make those decisions. 

In this project you are going to make a **random hobby selector**. 

You will: 
+ Use variables to store data
+ Display icons on the LEDs
+ Use `if... then` blocks to select which icons to show
+ Use gestures and buttons
+ Use random numbers to make choices

--- no-print ---

### Play ▶️

--- task ---

What happens if you `shake` the micro:bit?
What happens if you click the `A` or `B` buttons? 
What happens if you click the `logo`?

<div style="position:relative;height:100%;padding-bottom:125%;padding-top:0;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/---run?id=_gsk7kk1AJWXy" allowfullscreen="allowfullscreen" sandbox="allow-popups allow-forms allow-scripts allow-same-origin" frameborder="0"></iframe>
</div>

--- /task ---
--- /no-print ---

### Opening MakeCode

To get started creating your micro:bit project, you will need to open the MakeCode editor.

--- task ---

Open the MakeCode editor at [makecode.microbit.org](https://makecode.microbit.org)

--- collapse ---

---
title: Offline version of the editor
---

There is also a [downloadable version of the MakeCode editor](https://makecode.microbit.org/offline-app).

--- /collapse ---

--- /task ---

Once the editor is open, you will need to create a New Project and give your project a name. 

--- task ---

Click on the **New Project** button.

![The new project button inside of MakeCode.](images/new-project-button.png)

--- /task ---

--- task ---

Give your new project the name `hobby-selector` and click **Create**.

![The name 'hobby-selector' written in the New Project dialogue box.](images/new-project.png)

**Tip:** Give your project a helpful name that relates to the activity you’re creating. This will make it easier to find if you create other projects on MakeCode.

--- /task ---

### The MakeCode Editor

Created by the micro:bit Foundation, the **MakeCode editor** has everything you need to get started coding on micro:bit. 

![The MakeCode Editor window](images/makecode-tour.png)

On the left side there is a **simulator**, this contains a virtual micro:bit that you can use to test your code! 

It has all the features and buttons found on a V2 micro:bit, including:
+ LED display
+ Speaker
+ Microphone
+ Input buttons
    + A
    + B
    + Logo

In the centre there is the **blocks panel** which is colour-coded and allows you to access various code blocks.

On the right side is the **code editor panel** to drag and drop blocks into when creating your program.

### Show Icon

The MakeCode editor panel already contains two blocks: `on start` and `forever`.

You are going to use the `forever` block to see how the LEDs on the simulator work.

--- task ---

Click on the Basic blocks group in the Blocks panel. This will expand to show you the blocks available.

![The Basic menu with the 'show icon' block highlighted](images/basic-blocks.png)

Drag the `show icon` block and place it **inside** the `forever` block. 

This should fit in place like a puzzle.

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_iVKhocCVxR3f" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

--- task ---

Click the down arrow on the show icon block and choose any icon of your choice.

![The show icon menu expanded to display all available icons](images/show-icons.png)

--- /task ---

--- task ---

**Test:** Click the play button on the emulator, the LED display should light up, showing your chosen icon.

In this example we have chosen the `X` icon.

![The micro:bit simulator displaying an 'X' icon on its LEDs with the code blocks showing on the right](images/led-display.png)

Well done for getting the micro:bit to do something!

--- /task ---

### Choose your hobbies. 

--- task ---

Choose 3 hobbies/activities you like to do in your spare time. 

If you can't think of some here are some ideas to  get you started:
+ Gaming
+ Reading
+ Baking
+ Watching TV
+ Going for a walk
+ Playing a sport
+ Drawing

--- /task ---

--- task ---

Change your icon to one that represents your first hobby. 

--- /task ---

### Creating a variable

Create a variable that will be used to decide which activity you do. 

--- task ---

Open the `Variables` block menu, and click **Make a variable**.

![The Variables block menu, open with the "Make a variable" button highlighted](images/variable-menu.png)

--- /task ---

--- task ---

Call your new variable `activity`. 

![The "New Variable" name window, with the name activity written in the box](images/variable-name.png)

--- /task ---

You will now see that there are new blocks you can use to set, change or use the value stored in the `activity` variable. 

![The Variable block menu - with new blocks to set the value of the activity variable, to change the value of the activity variable and to use the value of the activity variable in your code.](images/variable-blocks.png)

--- task ---

Drag the `set [activity] to 0` block inside the `onstart` block.

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_YbT2My3k2aXu" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

### Which hobby will it be?

Next you are going to add the code that will show which activity the micro:bit has chosen. 

You will use `if... then` blocks to do this. 

--- task ---

Open the **Logic** menu and choose the `if 'true' then` block. 

![The Logic menu open with the "if 'true' then" block highlighted](images/if-block.png)

Drag it inside the `forever` loop block **above** your icon block. 

We have chosen a ghost to represent a gaming activity.

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_3fXJCKJ7LTAu" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

Now you are going to make it so that your icon shows only if the activity variable value is `1`.

--- task ---

Open the **Logic** menu and grab the `0 '=' 0` **condition block**. 

![The Logic menu with the condition block "0 '=' 0" highlighted](images/condition-block.png)

Drag that over the `true` part of your `if` block and drop it there. 

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_CPPLmMhR29Cg" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

--- task ---

Head back to the **Variables** menu and grab the small block that says `activity`. 

Drag that block to the **first** `0` in your new condition block. 

Change the second `0` to a `1`.

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_FpsdqdfWx9cu" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

--- task ---

Drag your `show icon` block **inside** the `if... then` block. 

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_CJoVdpb0YMFy" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

--- task ---

When you make a change to a code block, the simulator will restart.

**Test** When the program runs, you should see that nothing appears on the LEDs.

In the `on start` block:

**Change** the value from `0` to `1` in your `set 'activity' to 0` block.

**Re-test** When the program runs again after your last change, you should see the icon appear. 

**Make sure to set the value of the activity variable back to `0` in the `on start` block.**

--- /task ---

### Adding more hobbies

To add more hobby options to your program, you will need to add more conditions to your `if... then` block.

--- task ---

Click on the `+` symbol at the bottom of the `if... then` block. This will create an `else` block. 

--- /task ---

--- task ---

Click on the `+` symbol below the  `else` block. This will create an `else if... then` block. Do this one more time so you have two `else if... then` blocks.

--- /task ---

--- task ---

Now click on the `-` symbol next to the `else` block to remove the `else` block.

![Using the + symbol, three else if blocks are added to a condition. Finally, the else is removed from the end by clicking the - symbol next to it](images/adding-ifs.gif)

--- /task ---

--- task ---

Right click on the whole `condition` block in the first `if... then` block. Click just to the left of the activity variable, or just to the right of the value `0` to make sure you select the whole block.

Click `Duplicate` to make a copy of the whole block.

--- /task ---

--- task ---

Drag the duplicated `condition` block into the first `else if... then` block. Then change the number `1` to a `2`.

--- /task ---

--- task ---

Duplicate the `condition` one more time and drag it into the second `else if... then` block. Then change the number to a `3`.

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_9h6MfxbmaFYu" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

### Styling your hobbies

You will select more icons to represent the hobbies your micro:bit will randomise for you. 

--- task ---

**Choose:** Three images to represent your hobbies.

You can use the `show icon` block or create your own icon using the `show leds` block.

--- collapse ---

---
title: Using the show leds block
---

Inside the `Basic` menu, drag the `show leds` block below an `else if... then` block to use it.

![the Basic menu with the 'show leds' block highlighted](images/show-leds.png)

You can click on each of the squares to draw your picture. White squares will be lit on the micro:bit.

![The 'show leds' block with a smiley face created in white squares](images/draw-icon.png)

--- /collapse ---

--- /task ---

### Choose a random hobby

Use the `shake` gesture to randomly select a hobby for you.

--- task ---

Drag the `on shake` block from the `Input` menu.

![The Input menu with the 'on shake' block highlighted](images/on-shake.png)

--- /task ---

--- task ---

From the `Variables` menu, drag the `set activity` block inside the `on shake` block.

--- /task ---

--- task ---

From the `Math` menu, drag the `pick random 0 to 10` block inside the `set activity` block.

![The Math menu with the 'pick random 0 to 10' block highlighted](images/pick-random.png)

Change the numbers from `0 to 10` to `1 to 3`.

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_HeDV38b0odfW" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

### Clear the screen

Clear the screen if you want to randomise a new hobby.

--- task ---

Use the `on logo pressed` block from the `Input` menu.

![![The Input menu with the 'on logo pressed' block highlighted](images/onlogo-pressed.png)

--- collapse ---

---
title: V1 micro:bit users
---

The logo button is only available on the V2 of the micro:bit. Instead, use the `on button A pressed` block from the `Input` menu.

![The Input menu with the 'on button A pressed' block highlighted](images/button-a.png)

--- /collapse ---

--- /task ---

--- task ---

Drag the `clear screen` block from the `Basic` menu and place it inside the `on logo pressed` block.

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_RKbbriA5XD9a" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

--- task ---

Now drag the `set activity` block from the `Variables` menu and place it below the `clear screen` block. 

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_9v9URDdYb0Hv" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

--- task ---

**Test** When the program runs, check that all your code is working. 

**Click** the shake icon on the micro:bit to randomly choose a hobby. 

**Press** the logo (or A button on the V1 micro:bit) to make sure the screen clears.

--- /task ---

--- save --- 

### Uploading your program to the micro:bit

**Save** and download your code so you can test it out on a physical micro:bit.

--- task ---

Click on the `Download` button below the micro:bit simulator. 

![Highlighted download button on the MakeCode editor](images/download-button.png)

You will be asked to plug in your micro:bit, do that now, then click **Continue**. 

Now to Pair your micro:bit, click **Pair** and select your device from the list that appears, then click **Connect**.

![Select micro:bit dialog box showing a BBC micro:bit device.](images/select-microbit.png)

--- collapse ---

---
title: My micro:bit won't pair
---

If your micro:bit won't pair using the method above, it will download the program for you. 

**Windows:** Open **File Explorer** and check that you can see `MICROBIT` under `This PC` on the left hand side. If it is there, drag the downloaded `.HEX` file to it, your program will upload onto your micro:bit and you should be able to use it.

**MacOS:** Open **Finder** and check that you can see `MICROBIT` under `Locations` on the left hand side. If it is there, drag the downloaded `.HEX` file to it, your program will upload onto your micro:bit and you should be able to use it.

If your micro:bit isn't showing up, try unplugging it and plugging it back in. You can also try a different USB port or USB cable if they are available.

--- /collapse ---

--- /task ---

--- task ---

When you have downloaded your program to your physical micro:bit, it will run immediately.

**Test** You should now see icons randomly chosen when you shake the micro:bit.

--- /task ---

### Upgrade your project

You can upgrade your project to make it more engaging by:

+ Add more hobbies so you can have a wider range to choose from. Remember to:
  + Add a different symbol to display for each activity
  + Increase the number of `else if... then` blocks so you can add more icons
  + Increase the random range to more than three to match the number of added hobbies
