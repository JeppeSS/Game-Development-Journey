# Embarking on the Coding Odyssey

As you stand on the threshold of your game development journey, the tools of the trade are at your fingertips: the Odin programming language and `Visual Studio Code`. The adventure is about to get even more exciting as we dive into the heart of coding and game development.

Visualize yourself in a dimly lit room, your computer screen casting an otherworldly glow. An electrifying sense of anticipation courses through you as you prepare to unlock the secrets of game development. In this chapter, we will unravel the fundamentals that underpin this captivating realm. These concepts will serve as the bedrock upon which your game development skills will flourish.

## The Canvas of Code

Before we dive into the practical side of things, it's time to create a dedicated workspace for your game development projects. Similar to an artist preparing their canvas, you are about to set the stage for your coding masterpieces.

### Step 1: Crafting a Project Sanctuary

Begin by selecting a location on your computer where you will house all your game development creations. Envision this place as your sanctuary, a sacred realm where your ideas will spring to life. If you are comfortable with the command line, let's embark on this journey together:

```shell
C:\Documents> mkdir Game-Dev-Sanctuary
```

> **Note**: Commands are highlighted like this to make them stand out.

The `mkdir` command, much like a magician conjuring a portal, creates a new folder in your chosen location. We name this realm as **Game-Dev-Sanctuary**, where your game development dreams will flourish.

### Step 2: Navigating to Your workspace

Now, let's step into your newly formed workspace:

```shell
C:\Documents> cd Game-Dev-Sanctuary
```

The `cd` command, akin to a wise guide leading you through an enchanted forest, allows you to enter your sanctuary. Your command line will now read:

```shell
C:\Documents\Game-Dev-Sanctuary>
```

### Step 3: Establishing the Playground

To maintain impeccable organization for your projects, it is wise to create a subfolder for each endeavor. Picture these subfolders as chambers within your creative sanctuary. Let's craft one for your tutorial project:

```shell
C:\Documents\Game-Dev-Sanctuary> mkdir Tutorial-1
```

With this act, you have laid the foundation for your first game development masterpiece. Now, step into this chamber:

```shell
C:\Documents\Game-Dev-Sanctuary> cd Tutorial-1
```

These steps, akin to a ritual of preparation, ensure that your workspace is primed to host your coding odyssey. In the upcoming sections, we shall roll up our sleeves and embark on the thrilling journey of creating your very first interactive program. The skills you acquire here will serve as the brushstrokes on your canvas, setting the stage for your grand game development adventures!

## Crafting Your First Tome Of Magic

Now, you are ready to inscribe the ancient runes of magic. The first script we shall write is a simple program that will inscribe the text "Hello Aspiring Game Developer" onto the console. The purpose of this script is to ensure that we have everything set up correctly and to provide you with a glimpse of how we turn our code into reality. For now, don't fret over the details; we will delve deeper into them later.

### Step 1: Unfurling Your Tome

As you stand in your previously crafted chamber:

```shell
C:\Documents\Game-Dev-Sanctuary\Tutorial-1>
```

It's time to unfurl your code tome. If you followed along and installed `Visual Studio Code`, you can now open a new scroll using the following command. If you haven't installed it yet, you can create a new file as you usually do:

```shell
C:\Documents\Game-Dev-Sanctuary\Tutorial-1> code main.odin
```

Let's break down the command: `code` is a shortcut that comes with the installation of `Visual Studio Code`, which opens the editor. The second part, **main.odin**, tells Visual Studio Code to open the file if it exists or create a new file with that name.

> **Tip**: You can think of this like opening a blank canvas to paint your code.

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

**Explanation**:
* `package main` : This line informs the computer that you're creating a program, and it belongs to a package named **main**. The **main** package is special; it's where the execution of the program starts.

* `import "core:fmt"` : This line imports a package called **fmt** from a library named **core**. Packages are collections of code that provide various functions and tools, similar to a toolbox. The **fmt** package is commonly used for formatting and printing text.

* `main :: proc()  { ... }` : This part defines the **main** procedure, which is the entry point for your program. Think of it as the starting line in a race. Let's break it down further:
    
    * `proc()` : This keyword tells us that this is a procedure, in this case, a procedure that doesn't take any arguments due to the empty parentheses.

    * `main` : This is the name of the procedure.

    * `{ ... }` :  This is the scope of our procedure. Everything between the opening bracket **{** and the closing bracket **}** belongs to this procedure.

* ` fmt.printf("Hello Aspiring Game Developer\n")` :  This line calls a procedure named **printf** from the **fmt** package to write or print the text "Hello Aspiring Game Developer," followed by a newline character **\n** (which moves the cursor

 to the next line).

**In simple terms, this program does the following**:
* It uses built-in tools from the **fmt** package to print a message to the terminal.
* The message it prints is "Hello Aspiring Game Developer".

With your first script ready, you're about to learn how to cast this spell effectively.

### Step 3: Casting Your Code Spell

Now, it's time to cast your first coding spell! We're going to transform the code you've crafted into a language that your computer can comprehend. Begin by opening your trusted command center, which you can find either in the form of the `Terminal` for Linux users or the `Command Prompt` for Windows users:

```shell
C:\Documents\Game-Dev-Sanctuary\Tutorial-1>
```

With your command center at the ready, let's reveal your arsenal. Depending on your operating system, you can use the following commands:

* **For Windows**:
    ```shell
    C:\Documents\Game-Dev-Sanctuary\Tutorial-1> dir
    ```

    The `dir` command unveils all the hidden treasures in your current location. Your `Command Prompt` will now display:

    ```shell
    Directory of C:\Documents\Game-Dev-Sanctuary\Tutorial-1

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
C:\Documents\Game-Dev-Sanctuary\Tutorial-1>
```

Now, it's time to invoke your coding magic. Execute the following command:

```shell
C:\Documents\Game-Dev-Sanctuary\Tutorial-1> odin build main.odin -file
```

Let's decipher this incantation. The word `odin` is a reference to the Odin compiler, your trusted magical translator that we installed in the previous chapter. `build` is the command that beckons the Odin compiler to perform its translation. This is where `main.odin`, your chosen spellbook, comes into play - it's the file you wish to translate. Since it's a single file, we conclude with the `-file` flag.

> **Tip**: Think of this like transforming your written spell into a magic scroll that your computer can understand.

Now, let's once again unveil your treasures:

```shell
C:\Documents\Game-Dev-Sanctuary\Tutorial-1>dir

 Directory of C:\Documents\Game-Dev-Sanctuary\Tutorial-1

12/10/2023  20.31    <DIR>          .
10/10/2023  20.29    <DIR>          ..
12/10/2023  20.31           381.952 main.exe
12/10/2023  19.46               107 main.odin
```

In your treasure chest, you'll now find a new executable file. Depending on your operating system, it may appear as `main.exe`, `main.bin`, or just `main`. The time has come to test the effectiveness of your spell:

```shell
C:\Documents\Game-Dev-Sanctuary\Tutorial-1> main.exe
Hello Aspiring Game Developer
```

Bravo! Your first coding spell has been cast, and it works like a charm!

## Theory: From Code to Computer Understanding

Congratulations on successfully casting your first coding spell! You've taken the first step on a fascinating journey into the world of game development. Now, let's take a moment to understand how your code is transformed into something your computer can comprehend.

**Code as a Language**: Think of code as a special language that allows you to communicate with your computer. This language consists of instructions and commands, just like you'd give directions to a friend. In our case, the computer is your willing and obedient friend, ready to follow your every command.

**Translating Code**: Your computer doesn't understand human language; it speaks in its own binary language of 0s and 1s. To bridge this gap, we use a magical tool called a compiler. This compiler, in our case the Odin compiler, takes the code you've written and translates it into the computer's language. It's like having a translator between you and a friend who speaks a different language.

**Creating an Executable**: The result of this translation is an executable file, like the `main.exe` we created. This file contains your code transformed into the computer's language. When you run it, the computer follows the instructions you've given in your code, just like following a recipe in a cookbook.

**Seeing the Magic**: When you run the executable, it interacts with your computer's hardware and software to perform actions, such as displaying "Hello Aspiring Game Developer" on the screen. It might seem like magic, but it's all based on the logic you've crafted in your code.

**The Journey Ahead**: As you delve deeper into game development and coding, you'll learn more about the intricacies of this magical process. You'll gain the ability to create complex spells (code) that can bring entire virtual worlds to life.

This chapter has introduced you to the basics of setting up your workspace, writing your first lines of code, and casting your first spell. Remember that the journey has just begun, and there's a lot more to explore and learn in the realm of coding and game development. So, prepare yourself for an exciting adventure as you continue to unlock the secrets of this captivating world.

Now that you've embarked on your coding odyssey, be curious, keep experimenting, and don't be afraid to make mistakes. Learning is an essential part of this journey, and each line of code you write brings you closer to becoming a proficient game developer.

May your code always be bug-free, and your games, legendary! Good luck on your adventure!

## Exercises

Now, we are going to practice what we have learnt so far!

### Exercise 1: Setting Up Your Exercise Workspace

**Objective**: Practice creating directories and navigating the workspace.

Follow the steps outlined in the chapter to create a project sanctuary and subfolders for your game development exercises.

**Instructions**:
1.  Use the command line to create a new project directory and navigate to it.
    * Take a look at the `mkdir` and `cd` commands.

2. Within your project directory, create a new text file with a unique name.
    * Take a look at the `code` command.

> **Tip**: Think of this as creating a new canvas for your coding exercises.

### Exercise 2: Writing Your First Code

**Objective**: Write a simple program to display a message on the console.

Create an Odin program that displays a message on the console. You can use the example code provided in the chapter as a guideline.

**Instructions**:
1. Write a program that prints a message other than "Hello Aspiring Game Developer."

> **Tip**: This is like crafting your own magical incantation.

### Exercise 3: Building and Running Your Code

**Objective**: Compile and execute your Odin program.

Compile your Odin program using the Odin compiler, following the steps outlined in the chapter.

**Instructions**:
1. Compile your Odin program.
    * Take a look at the `odin build` command.

2. Run the executable and verify that it displays the message you intended.

3. Experiment by modifying some parts of the code and recompiling to see the changes - can you provoke any errors?

> **Tip**: Think of this as practicing your magical coding skills.

### Exercise 4: Understanding the Code

**Objective**: Analyze and try to understand the code provided in the chapter.

Carefully read and dissect the Odin code provided in the chapter.

**Instructions**:
1. Write down what each part of the code does, such as the `package main`, `import "core:fmt"`, and the `main :: proc()` section.

2. Try to explain the purpose of each part in simple terms to reinforce your understanding.

> **Tip**: This is like studying the spells in your magical book.

### Exercise 5: Expanding Your Code

**Objective**: Modify the code to add more content.

Take the code you wrote in Exercise 2 and expand it. For example, create a program that writes multiple messages.

**Instructions**:
1. Make changes to the code.
    * Take a look at `fmt.printf()`

> **Tip**: This is like experimenting with your own magical variations.

These exercises are designed to help you apply and reinforce the concepts introduced in the chapter. By working through them, you'll become more familiar with setting up your workspace, writing code, and compiling and running programs. This will serve as a solid foundation for your game development journey.

## Key Concepts and Commands

**Commands**:
1. `mkdir`: This command is used to create a new directory or folder. For example, `mkdir Game-Dev-Sanctuary` creates a directory called "Game-Dev-Sanctuary."

2. `cd`: The `cd` command is used to navigate to a selected directory. For instance, `cd Game-Dev-Sanctuary` allows you to enter the "Game-Dev-Sanctuary" directory.

3. `dir` (For Windows): The `dir` command lists the files and directories in the current directory.

4. `ls` (For Linux): The `ls` command lists the files and directories in the current directory.

5. `code`: The `code` command (specific to Visual Studio Code) opens the Visual Studio Code editor, allowing you to work on your code files. For example, `code main.odin` opens a file called "main.odin" in Visual Studio Code.

**Technical**:

1. **Programming Language**: A programming language is a set of instructions and commands that you use to communicate with your computer. Your code is written in a programming language, and it guides the computer on what actions to perform.

2. **Compiling**: Compiling is the process of translating your human-readable code, written in a high-level programming language, into machine-readable code that a computer can understand and execute. In this chapter, you've used the `odin` compiler to compile your Odin code into an executable file.

3. **Executable File**: An executable file, like `main.exe`, contains your code transformed into the computer's language. When you run it, the computer follows the instructions you've given in your code, much like following a recipe in a cookbook.

4. **File Structure**: Understanding how to organize and structure your files and directories is crucial in software development. It helps keep your projects organized and easily manageable.