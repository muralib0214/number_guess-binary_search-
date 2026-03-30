# 🎯 Number Guessing Game — Binary Search (Python)

### 🚀 An Intelligent Number Guessing Game using Binary Search Algorithm

## 📌 Project-Overview

This project is a Python-based Number Guessing Game where:

1.User thinks of a number

2.Computer guesses intelligently

3. Uses Binary Search Algorithm

4.Reduces search range by half every step

6. Ensures fast and efficient guessing

## 🎯Project-Objective

### The main goal of this project:

✅ Implement Binary Search Algorithm

✅ Practice Recursion

✅ Improve Problem Solving Skills

✅ Build Beginner-Friendly Python Project

✅ Learn Efficient Searching Algorithm

## ✨Features
🔍 Binary Search Based Guessing

⚡ Fast and Efficient Algorithm

💻 Command Line Interactive Game

🔁 Recursive Implementation

🛡️ Invalid Input Handling

📈 Optimized Performance

🎯 Beginner Friendly Code

## How-It-Works
### Step-by-Step Execution

Step 1 → User enters Start Range

Step 2 → User enters End Range

Step 3 → User thinks of a number

Step 4 → Program guesses middle number

Step 5 → User answers:

Y → Correct Guess

N → Wrong Guess

Step 6 → Program asks:

Is number greater than mid?

Step 7 → Search range reduces

Step 8 → Repeat until guessed

## Example-Execution

Number Guessing Game in Python

Enter Start Range: 1

Enter End Range: 100


Think of a number between 1 and 100.

Is the number 50? (Y/N): N

Is the number greater than 50? (Y/N): Y


Is the number 75? (Y/N): N

Is the number greater than 75? (Y/N): N


Is the number 62? (Y/N): Y

Congratulation Geek! Successfully Guessed Number.

## ⚡Algorithm-Used:

### 🔎 Binary Search Algorithm.

####Algorithm Steps:

1.Find middle element

2.Compare with target

3.Reduce search space

4.Repeat until found

## ⏱️Time-Complexity:

O(log n)

### Efficiency Example:
#### Range	Maximum Guesses
1 — 100	[7 guesses]

1 — 1,000	[10 guesses]

1 — 1,000,000	[20 guesses]

## 📂 Project-Structure
### number-guessing-game/

│

├── guess_number.py

└── README.md

## Requirements:
### Required Software

Python 3.x

Terminal / Command Prompt

No External Libraries Required

## ▶️How-To-Run
Step 1 — Clone Repository

git clone https://github.com/muralib0214/number_guess-binary_search-.git

Step 2 — Navigate to Project Folder

cd number-guessing-game

Step 3 — Run Python File

python guess_number.py

## 💻 Source-Code
### Python implementation for the 
### number guessing using 
### Binary Search

def guessNumber(startRange, endRange):
    if startRange > endRange:
        return True

    mid = (startRange + endRange) // 2

    print(f"Is the number {mid}? (Y/N): ", end="")
    user = input().strip()

    if user in ("Y", "y"):
        print("Congratulation Geek! Successfully Guessed Number.")
        return False

    elif user in ("N", "n"):
        print(f"Is the actual number greater than {mid}? (Y/N): ", end="")
        user = input().strip()

        if user in ("Y", "y"):
            return guessNumber(mid + 1, endRange)
        elif user in ("N", "n"):
            return guessNumber(startRange, mid - 1)
        else:
            print("Invalid input.")
            return guessNumber(startRange, endRange)
    else:
        print("Invalid input.")
        return guessNumber(startRange, endRange)


if __name__ == "__main__":
    print("Number Guessing Game in Python")

    startRange = int(input("Enter Start Range: "))
    endRange = int(input("Enter End Range: "))

    print(f"Think of a number between {startRange} and {endRange}")

    out = guessNumber(startRange, endRange)

    if out:
        print("Couldn't guess it.")

    print("Thank you for playing")

## 📚 Learning-Concepts

### This project helps you learn:

🧠 Binary Search Algorithm

🔁 Recursion

💻 Python Functions

🔀 Conditional Statements

📥 User Input Handling

⚡ Algorithm Optimization

## 🎯 Use-Cases
Python Beginner Project

Data Structures Practice

Coding Interview Preparation

Algorithm Learning

Academic Mini Project

## 🔮Future-Improvements

### Possible upgrades:

🎨 GUI Interface

🎮 Difficulty Levels

📊 Score System

🏆 Leaderboard

👥 Multiplayer Mode

🌐 Web Application Version

# Project-Difficulty:

Difficulty Level

🟢 Beginner → 🟡 Intermediate

Perfect For:

Students

Python Beginners

DSA Learners

## 🤝Contributing

Steps to contribute:

Fork repository

Create new branch\

Add improvements

Submit pull request

## ⭐Support

If you like this project:

⭐ Star the repository

🍴 Fork the project

📢 Share with others

# 👨‍💻 Author

Murali

Learning Data Structures & Algorithms 🚀


