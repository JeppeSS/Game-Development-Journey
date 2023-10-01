# The First Quest - Creating Your First Interactive Program

Welcome back, aspiring game developer! In this chapter, we're diving headfirst into the heart of game development by creating your first interactive program. This isn't just code; it's the spark that will ignite your journey into crafting immersive gaming experiences. So, grab your digital sword and let's embark on this enchanting quest into the world of interactive software.

## Setting the Stage for Your Epic Journey

Up until now, you've been on the sidelines, learning the basics and preparing your toolkit. But now, the stage is set for your grand entrance. Imagine this moment as your hero stepping out of their humble abode, ready to face the unknown. Your adventure begins here.

## Understanding the Significance

Why is creating an interactive program so significant in game development? Let's unravel the importance:

- **Player Engagement**

- **Compile the Program:**
    - Open your computer's terminal or command prompt.
    - Navigate to the directory where you saved the **`.odin`** file.
    - Compile the program by entering the following command:

## Your First Challenge

Our first challenge on this epic journey is to create an interactive program. This program will allow us to fetch user input and present information to the user. Think of it as the initial obstacle to overcome, the first puzzle to solve in our grand adventure.

## Gearing up

Before we dive into coding, let's prepare ourselves with a breif overview of what lies ahead. We'll discuss the concepts and tools we need to conquer this challenge successfully.

### Initial Program: Saying Hello

Let's start with a simple program. Below is a Odin program that writes "Hello Aspiring Game Developer" to the screen. Take a moment to examine it:


```go
package main

import "core:fmt"

main :: proc() {
    fmt.printf("Hello Aspiring Game Developer\n")
}
```
Now you might think, what kind of foul magic is this? Do not fear my friend, we will get to the bottom of this. The above program is a basic example of a program that writes a fixed message to the terminal. For now we will ignore most parts of this program, but dont worry we will get back to this later. First we will try to get this program running.

To create and run this program, follow these steps:

- **Create a .odin File:**
    - Open a text editor (e.g., Notepad, Visual Studio Code, or any code editor of your choice).
    - Write the code above into the editor.
    - Save the file with a **`.odin`** extension (e.g., **`hello.odin`**)
- **Compile the Program:**
    - Open your computer's terminal or command prompt.
    - Navigate to the directory where you saved the **`.odin`** file.
    - Compile the program by entering the following command:

        ```
        odin build hello.odin -file
        ```
        This command tells the compiler to compile **`hello.odin`** and procude an executable file named **`hello.exe`** or just **`hello`** depending on your operating system.
- **Run the Program:**
    - After successfully compilation, you can run the program by entering the following command:

        **Windows:**

        ```bash
        .\hello.exe
        ```

        **Linux:**
        ```bash
        ./hello
        ```
        You should see the "Hello Aspiring Game Developer" message displayed on the screen.

With these modifications, you not only learn how to code but also how to create, compile, and run a Odin program, which is a fundamental skill in software development.

Let's try to disect the most essential of the program:

```go
main :: proc() {
}
```

What we got here is the starting point of the program, this is also called the entry point of the program. 

## Your First Interactive Program

Now, let's enchance this program to make it interactive:

## Exercises

### Exercise 1: Character Introduction

Imagine you're crafting the beginning of a role-playing game (RPG). Modify your interactive program to introduce a character to the player. Ask the user to enter the name of their character and a class. Then, display a message like:

 **"Welcome, [Character Name] the [Character Class]!**

 
 This exercise sets the stage for character-driven adventures.  

### Exercise 2: Character Stats

Enhance your RPG-inspired program by asking the user to define their character's attributes, such as strength, agility, and intelligence. Display the character's stats to the player.

This exercise introduces the concept of character development in games.

### Exercise 3: Character Interaction

Expand your program to simulate an interaction between the player's character and a non-playable character (NPC). Create a scenario where the player's character encounters an NPC and exchanges dialogue. Prompt tbe user to enter dialogue for both characters, and display the conversation.

This exercise introduces the concept of dialogues and interaction in storytelling.