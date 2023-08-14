This is a **Discover** project, this project will help you explore what the **micro:bit** can do and decide whether you want to learn more. 

### What you will make

Here's a project to remind you to loosen up and strike a pose! This could be after a long day at school, or a way to cheer you and your friends up. You can program the micro:bit buttons to help you remember to have some silly fun.

In this project you are going to make a **silly reminder**. 

You will: 
+ Use variables to store data
+ Display icons, text and numbers on the LEDs
+ Play sounds
+ Use `if... then` blocks to select what to display
+ Use the pause blocks to create a countdown timer
+ Use buttons

--- no-print ---

### Play ▶️

--- task ---

What happens when the program starts?
What happens when the countdown runs?
What happens when the countdown finishes?
What happens if you `press` the A button?
What happens if you `press` the B button?

<div style="position:relative;height:100%;padding-bottom:125%;padding-top:0;overflow:hidden;">
<iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/---run?id=_gpECA3RDMhu2" allowfullscreen="allowfullscreen" sandbox="allow-popups allow-forms allow-scripts allow-same-origin" frameborder="0"></iframe>
</div>

--- /task ---

--- /no-print ---

### Opening MakeCode

To get started creating your micro:bit project, open the MakeCode editor.

--- task ---

Open the MakeCode editor at [makecode.microbit.org](https://makecode.microbit.org)

--- collapse ---

---
title: Offline version of the editor
---

There is also a [downloadable version of the MakeCode editor](https://makecode.microbit.org/offline-app).

--- /collapse ---

--- /task ---

Once the editor is open, create a New Project and give your project a name. 

--- task ---

Click on the **New Project** button.

![The new project button inside of MakeCode.](images/new-project-button.png)

--- /task ---

--- task ---

Create your project with the name `silly-reminder` and click **Create**.

![The name 'silly-reminder' written in the New Project dialogue box.](images/new-project.png)

**Tip:** Give your project a helpful name that relates to the activity you’re creating. This will make it easier to find if you create other projects on MakeCode.

--- /task ---

[[[makecode-tour]]]

### Display Icon

You will make use of the `on start` block to see how the LEDs on the simulator work.

--- task ---

Click on the `Basic` block menu in the Blocks panel. This will expand to show you the blocks available.

![The Basic block menu with the 'show icon' block highlighted](images/basic-blocks.png)

Drag the `show icon` block and place it **inside** the `on start` block. 

This should fit in place like a puzzle.

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_iVKhocCVxR3f" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

--- task ---

Click the down arrow on the show icon block and choose any icon of your choice.

![The show icon menu expanded to display all available icons](images/show-icon.png)

In this example we have chosen the `heart` icon.

--- /task ---

--- task ---

**Test:** Click the play button on the simulator. The LED display should light up, showing your chosen icon.

Well done for getting the LEDs on the micro:bit to light up!

--- /task ---

### Choose some poses

You will need to decide what silly faces/poses you will make whenever you push a micro:bit button. Here are some ideas for poses you could use:

+ Happy face icon for when you're feeling happy
+ An icon pose for when you're feeling excited
+ An icon pose to energise you when you're feeling tired
+ An icon pose for when you're feeling restless

### Create a timer for each pose

Create a variable that will be used as a timer for how long you should hold each pose.

--- task ---

Open the `Variables` block menu, and click **Make a variable**.

![The Variables block menu open with the "Make a variable" button highlighted](images/variable-menu.png)

--- /task ---

--- task ---

Name the new variable `timer`, then click the `Ok` button.

![The 'New variable name' window, with the name 'timer' written in the box](images/variable-examplename.png)

--- /task ---

New blocks will be created that you can place in your program to use and change the value stored in the `timer` variable. 

![The Variable block menu - with new blocks to set the value of timer, to change the value of timer and to use the value of timer in your code.](images/variable-blocks.png)

--- task ---

Drag the `set [timer] to 0` block inside the `onstart` block and change the `0` to `10`.

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_f4yMbPEpHFwv" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

### Set icon for each pose

You will now program the A and B input buttons on the micro:bit to help you select an icon for each pose.

--- task ---

Click on the `Input` block menu and drag the `on button A pressed` block.

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_TUwcRCfFsHCb" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

 Place it onto the **code editor panel** 

--- /task ---

--- task ---

From the `Basic` block menu, drag the `show leds` block inside the `on button A pressed` block.

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_7Ugf5a3JXb81" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

You can click on each of the squares to draw your pose. In this example, we have drawn a smiley face as a silly pose.

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:75%;height:75%;" src="https://makecode.microbit.org/---codeembed#pub:_XsR7jJ2wiTAx
" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

You will want the icon to be displayed for some time before changing so you will need to make use of a `pause ms` block. This is measured in milliseconds.

--- task ---

From the `Basic` block menu, drag a `pause (ms) 100` block below the `show leds` block inside the `on button A pressed` block.

![TODO - replace with embedded blocks](images/pause-ms.png)

--- /task ---

--- task ---

Change the 100 in the `pause (ms) 100` block to a longer time so the icon can be displayed for longer. We have set it to 2000ms (2 seconds) in this example.

![TODO - replace with embedded blocks](images/pause-2000.png)

--- /task ---

--- task ---

Right click on the `set timer` block inside the `on start` block. 

Click `Duplicate` to make a copy of it.

--- /task ---

--- task ---

Place the duplicated `set timer` below the `pause (ms) 2000` block inside the `on button A pressed` block.

![TODO - replace with embedded blocks](images/settimer-pressed.png)

--- /task ---

To create more than one pose that can be selected, you will need to use another input button on the micro:bit. This will be the `on button B pressed` block.

--- task ---

Right click on the entire `on button A pressed` block. 

Click `Duplicate` to make a copy of it.

![The 'on button A pressed' block showing a menu including 'Duplicate', Add Comment, Collapse Block, Delete Blocks and Help.](images/duplicate-block.png)

You will now have an exact copy of all the blocks of code inside `on button A pressed` on the code editor panel.

--- /task ---

--- task ---

Click the down arrow next to the A on your duplicated `on button A pressed` block. Change the `A` to `B`.

![The 'on button A pressed' block showing a drop-down menu from the A, with options for A, B and A+B together](images/button-options.png)

--- /task ---

--- task ---

Change the squares on the `show leds` block inside the `on button B pressed` block to create a new pose icon.

--- /task ---

--- task ---

When your program runs, you should see your icon appear.

**Test** Press the `A` button to test the icon that displays on the led. Take a note of how long it shows for

Do the same to test the `B` button.

**Change** You can change the value in your `pause ms` block to increase or decrease the time the icons are shown for on each button press.

--- /task ---

### Create a countdown

You will now create a countdown using the `timer` variable that you previously set to `10` to represent 10 seconds. 

The `timer` variable value will decrease by 1 each time.

--- task ---

From the `Basic` block menu, drag the `show number` block inside the `forever` block on the editor panel.

![The Basic block menu with the 'show number' block highlighted](images/show-number.png)

From on the `Variables` block menu, drag the `timer` variable inside the `0` on the `show number` block

![TODO - replace with embedded blocks](images/shownumber-timer.png)

--- /task ---

To check if the timer is greater than 0, then make it count down, you will need an `if..then..else` logic condition block. 

--- task ---

From the `Logic` block menu, drag the `if..then..else` logic block. 

![TODO - replace with screenshot of Logic block and if then else](images/ifelse-condition.png)

Place it below the `show number` block.

![TODO - replace with embedded blocks]()

--- /task ---

--- task ---

From the `Logic` menu, drag out a comparison block `0 = 0`.

![The Logic block menu with the condition block '0 = 0' highlighted](images/comparison-block.png)

Place it inside the `true` space within the `if..then..else` block.

![TODO - replace with embedded blocks]()

--- /task ---

--- task ---

From the `Variables` block menu, drag out the `timer` variable block and place it inside the first `0` on the `0 = 0` comparison block.

Change the `=` to a `>` than symbol using the drop down arrow on the comparison block.

![TODO - replace with embedded blocks]()

--- /task ---

To create a countdown, the timer variable value needs to reduce by `1` (but only if the timer is greater than `0`).

--- task ---

From the `Variables` block menu, drag the `change timer by 1` block and place it inside the `if.. then` section of blocks. 

Also change `1` to `-1`.

![TODO - replace with embedded blocks]()

--- collapse ---

---
title: Adding sound for dramatic effect
---

From the `Music` block menu, drag the `play..tone..Middle C for 1 beat.. until done` block. Place it below the `change timer by -1` variable block.

Click on the `Middle C` module and a piano keys console will appear. Choose a suitable note for your timer. In this example we have selected `Middle A`.

--- /collapse ---

--- /task ---

After each value of `timer` is displayed on the micro:bit, you need to add a 1-second pause.

--- task ---

Right click on any of the `pause ms` blocks already on the editor panel and duplicate it. 

Drag this below the `play tone..for 1 beat` block.

Change `2000`ms to `1000`ms. 

--- /task ---

After the countdown finishes, you need a message to tell the user to change their silly pose.

You can do this by making use of the `else`.

--- task ---

Inside the `Basic` menu, drag out the `show string` block. Place it insude the `else` part of the `if..then..else` block.

Change the string `Hello!` to `Pose!`.

--- /task ---

--- task ---

**Run** the program to check that all your code is working. 

**Press** the A button to see the pose icon displayed. 

**Press** the B button to see another pose icon displayed.  

**Check** the countdown timer is working and counting from 10 backwards. 

**Check** that a tone is played after each second counts down.  

--- /task ---

--- save --- 

--- task ---

[[[download-to-microbit]]]

--- /task ---

--- task ---

**Test** Run your program on the physical micro:bit. 

--- /task ---

### Upgrade your project

You can upgrade your project to make it more engaging by doing the following:

+ Add more silly poses so you can have a wider range to choose from.
+ Randomise the pose that gets selected after the timer reaches 0
+ Add other input gestures such as shake and on logo press.

