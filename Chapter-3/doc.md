# The First Quest - Creating Your First Interactive Program

In this chapter, our adventure truly commences as we embark on our first task. We will craft our very first interactive program, a pivotal milestone on our journey into the world of game development. The goal here is to gain hands-on experience in fetching user input and presenting it to the user, setting the stage for more complex and exciting creations in the chapters to come. So, grab your coding sword, dear adventurers, and let's dive into the enchanting realm of interactive software!

## The Adventure Awaits

Up until now, our paths have been laid out, and our toolkit has been prepared. It's time to take the first step into the hearth of game development. Picture this as the moment when the hero steps out of their humble abode, ready to face the unknown.

## Your First Challenge

Our first challenge on this epic journey is to create an interactive program. This program will allow us to fetch user input and present information to the user. Think of it as the initial obstacle to overcome, the first puzzle to solve in our grand adventure.

## Gearing up

Before we dive into coding, let's prepare ourselves with a breif overview of what lies ahead. We'll discuss the concepts and tools we need to conquer this challenge successfully.

### Initial Program: Saying Hello

Let's start with a simple program. Below is a Odin program that prints "Hello Aspiring Game Developer" to the screen. Take a moment to examine it:

```go
package main

import "core:fmt"

main :: proc() {
    fmt.printf("Hello Aspiring Game Developer\n")
}
```

The above program is a basic example of a program that outputs a fixed message. To create and run this program, follow these steps:

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

[Previous Chapter: Chapter 2](../Chapter-2/doc.md)