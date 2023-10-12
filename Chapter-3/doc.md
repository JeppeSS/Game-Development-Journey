# Embarking on the Coding Odyssey

As you stand on the threshold of your game development journey, the tools of the trade are at your fingertips: the Odin programming language and `Visual Studio Code`. The adventure is about to get even more exciting as we dive into the heart of coding and game development.

Visualize yourself in a dimly lit room, your computer screen casting an otherworldly glow. An electrifying sense of anticipation courses through you as you prepare to unlock the secrets of game development. In this chapter, we will unravel the fundamentals that underpin this captivating realm. These concepts will serve as the bedrock upon which your game development skills will flourish.

## The Canvas of Code

Before we dive into the practical side of things, it's time to create a dedicated workspace for your game development projects. Similar to an artist preparing their canvas, you are about to set the stage for your coding masterpieces.

### Step 1: Crafting a Project Sanctuary

Begin by selecting a location on your computer where you will house all your game development creations. Envision this place as your sanctuary, a sacred realm where your ideas will spring to life. If you are comfortable with the command line, let's embark on this journey together:

```shell
C:\Users\YourUsername\Documents> mkdir Game-Dev-Sanctuary
```

The `mkdir` command, much like a magician conjuring a portal, creates a new folder in your chosen location. We name this realm as **Game-Dev-Sanctuary**, where your game development dreams will flourish.

### Step 2: Navigating to Your workspace

Now, let's step into your newly formed workspace:

```shell
C:\Users\YourUsername\Documents> cd Game-Dev-Sanctuary
```

The `cd` command, akin to a wise guide leading you through an enchanted forest, allows you to enter your sanctuary. Your command line will now read:

```shell
C:\Users\YourUsername\Documents\Game-Dev-Sanctuary>
```

### Step 3: Establishing the Playground

To maintain impeccable organization for your projects, it is wise to create a subfolder for each endeavor. Picture these subfolders as chambers within your creative sanctuary. Let's craft one for your tutorial project:

```shell
C:\Users\YourUsername\Documents\Game-Dev-Sanctuary> mkdir Tutorial-1
```

With this act, you have laid the foundation for your first game development masterpiece. Now, step into this chamber:

```shell
C:\Users\YourUsername\Documents\Game-Dev-Sanctuary> cd Tutorial-1
```

These steps, akin to a ritual of preparation, ensure that your workspace is primed to host your coding odyssey. In the upcoming sections, we shall roll up our sleeves and embark on the thrilling journey of creating your very first interactive program. The skills you acquire here will serve as the brushstrokes on your canvas, setting the stage for your grand game development adventures!

## Crafting Your First Tome Of Magic

Now, you are ready to inscribe the ancient runes of magic. The first script we shall write is a simple program that will inscribe the text "Hello Aspiring Game Developer" onto the console. The purpose of this script is to ensure that we have everything set up correctly and to provide you with a glimpse of how we turn our code into reality. For now, don't fret over the details; we will delve deeper into them later.

### Step 1: Unfurling Your Tome

As you stand in your previously crafted chamber:

```shell
C:\Users\YourUsername\Documents\Game-Dev-Sanctuary\Tutorial-1>
```

It's time to unfurl your code tome. If you followed along and installed `Visual Studio Code`, you can now open a new scroll using the following command. If you haven't installed it yet, you can create a new file as you usually do:

```shell
C:\Users\YourUsername\Documents\Game-Dev-Sanctuary\Tutorial-1> code main.odin
```
Let's break down the command: `code` is a shortcut that comes with the installation of `Visual Studio Code`, which opens the editor. The second part, **main.odin**, tells Visual Studio Code to open the file if it exists or create a new file with that name.

### Step 2: Scribing the Runes

As you gaze upon the blank scroll, you feel the power at your fingertips, waiting for your words to bring it to life. Now, inscribe the following into your tome; try writing it down instead of copying and pasting:

```go
package main

import "core:fmt"

main :: proc() {
    fmt.printf("Hello Aspiring Game Developer\n")
}
``` 

Let's dissect this magical script. I don't expect you to fully grasp it all at once; simply follow along, read it a few times, and continue. We will revisit these concepts, and eventually, they will become clear.

* `package main` : This line informs the computer that you're creating a program, and it belongs to a package named **main**. The **main** package is special; it's where the execution of the program starts.

* `import "core:fmt"` : This line imports a package called **fmt** from a library named **core**. Packages are collections of code that provide various functions and tools, similar to a toolbox. The **fmt** package is commonly used for formatting and printing text.

* `main :: proc()  { ... }` : This part defines the **main** procedure, which is the entry point for your program. Think of it as the starting line in a race. Let's break it down further:
    
    * `proc()` : This keyword tells us that this is a procedure, in this case, a procedure that doesn't take any arguments due to the empty parentheses.

    * `main` : This is the name of the procedure.

    * `{ ... }` :  This is the scope of our procedure. Everything between the opening bracket **{** and the closing bracket **}** belongs to this procedure.

* ` fmt.printf("Hello Aspiring Game Developer\n")` :  This line calls a procedure named **printf** from the **fmt** package to write or print the text "Hello Aspiring Game Developer," followed by a newline character **\n** (which moves the cursor to the next line).

In simple terms, this program does the following:

* It uses built-in tools from the **fmt** package to print a message to the terminal.
* The message it prints is "Hello Aspiring Game Developer".

With your first script ready, you're about to learn how to cast this spell effectively.

### Step 3: Casting Your Code Spell

Now, it's time to cast your first coding spell! We're going to transform the code you've crafted into a language that your computer can comprehend. Begin by opening your trusted command center, which you can find either in the form of the `Terminal` for Linux users or the `Command Prompt` for Windows users:

```shell
C:\Users\YourUsername\Documents\Game-Dev-Sanctuary\Tutorial-1>
```

With your command center at the ready, let's reveal your arsenal. Depending on your operating system, you can use the following commands:

* **For Windows**:
    ```shell
    C:\Users\YourUsername\Documents\Game-Dev-Sanctuary\Tutorial-1> dir
    ```

    The `dir` command unveils all the hidden treasures in your current location. Your `Command Prompt` will now display:

    ```shell
    Directory of C:\Users\YourUsername\Documents\Game-Dev-Sanctuary\Tutorial-1

    12/10/2023  20:29    <DIR>          .
    10/10/2023  20:29    <DIR>          ..
    12/10/2023  19:46               107 main.odin
                1 File(s)            107 bytes
    ```

* **For Linux**:
    ```shell
    YourUsername@Something:~/Game-Dev-Sanctuary/Tutorial-1$ ls
    ```

    The `ls` command unveils the contents of your treasure chest. Your `Terminal` will now reveal:

    ```shell
    main.odin
    ```

There, you have it - the **main.odin** file that you've meticulously crafted, containing your magical code. Now, let's proceed with casting your spell. Return to your command center:

```shell
C:\Users\YourUsername\Documents\Game-Dev-Sanctuary\Tutorial-1>
```

Now, it's time to invoke your coding magic. Execute the following command:

```shell
C:\Users\YourUsername\Documents\Game-Dev-Sanctuary\Tutorial-1> odin build main.odin -file
```

Let's decipher this incantation. The word `odin` is a reference to the Odin compiler, your trusted magical translator that we installed in the previous chapter. `build` is the command that beckons the Odin compiler to perform its translation. This is where `main.odin` your chosen spellbook, comes into play - it's the file you wish to translate. Since it's a single file, we conclude with the `-file` flag. 

Now, let's once again unveil your treasures:

```shell
C:\Users\YourUsername\Documents\Game-Dev-Sanctuary\Tutorial-1>dir

 Directory of C:\Users\YourUsername\Documents\Game-Dev-Sanctuary\Tutorial-1

12/10/2023  20.31    <DIR>          .
10/10/2023  20.29    <DIR>          ..
12/10/2023  20.31           381.952 main.exe
12/10/2023  19.46               107 main.odin
```

In your treasure chest, you'll now find a new executable file. Depending on your operating system, it may appear as `main.exe`, `main.bin`, or just `main`. The time has come to test the effectiveness of your spell:

```shell
C:\Users\YourUsername\Documents\Game-Dev-Sanctuary\Tutorial-1> main.exe
Hello Aspiring Game Developer
```

Bravo! Your first coding spell has been cast, and it works like a charm!

## Theory: From Code to Computer Understanding

## Exercises
