# Project 1: Interactive Python Terminal Quiz

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/THE-KINGBUWORLDVIEW/python-masterclass-starter-pack/blob/main/interactive_terminal_quiz.ipynb)

Welcome to your first masterclass project! In this module, we are building a fully functional interactive trivia game that runs directly in your terminal. This project is designed to bridge the gap between reading about code and actually writing a program that thinks, responds, and interacts with a user.

---

##  What You Will Learn
By the end of this project, you will have hands-on experience with the fundamental building blocks of Python:
* **Variables:** Storing data (like a player's score) so we can update it later.
* **Data Structures (Lists & Dictionaries):** Organizing a large amount of information cleanly.
* **Loops:** Telling the computer to repeat an action so we do not have to write the same code 10 times.
* **Conditionals:** Giving your program a "brain" to make decisions (e.g., *If* the answer is correct, *then* add a point).
* **User Input:** Making the program interactive by asking the user to type in their answers.

---

##  How the Code Works (Step-by-Step)

### Step 1: Setting the Stage (The Score Tracker)
Every game needs a scoreboard. We start by creating a simple variable called `score` and setting it to `0`. As the player gets questions right, our program will update this number.

### Step 2: Building the Question Bank (Lists & Dictionaries)
Instead of creating 10 separate variables for 10 questions, we use a single **List** (a collection of items). Inside that list, each question is stored as a **Dictionary**. A dictionary pairs "keys" (like the word `question`) with "values" (the actual text of the question). This structure allows us to hold the question, the multiple-choice options, and the correct answer all in one neat package.

### Step 3: The Engine (The Game Loop)
To ask all 10 questions, we use a **`for` loop**. This tells Python: *"Take a look at my list of questions. For every single question in that list, run the following block of code."* This is the engine of our game, pushing the questions to the screen one by one.

### Step 4: The Logic (Checking the Answer)
Once a question is on the screen, we use the `input()` function to pause the program and wait for the user to type A, B, C, or D. 
Next, we use an **`if / else` statement** to compare what the user typed against the correct answer stored in our dictionary. 
* **If** they match, we congratulate them and add 1 to the `score`.
* **Else** (if they don't match), we reveal the correct answer.

### Step 5: The Grand Finale (Calculating the Grade)
After the loop finishes asking all the questions, the game is over. We take the final `score`, divide it by the total number of questions, and multiply by 100 to get a percentage. Finally, we use another `if / else` statement to give the player a custom message based on how well they performed!

---

##  Challenge for Students
Once you have the game running smoothly, try customizing it! 
1. Change the topic from Python to your favorite movie, sport, or hobby.
2. Add 5 more questions to the dictionary.
3. Tweak the final grading percentages to be more strict or more forgiving.
