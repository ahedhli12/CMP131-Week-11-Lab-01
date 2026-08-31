# CMP 131 – Python Programming


> **Required file location:** Keep every Python file directly in the repository root. Do not create a `src` folder.

## Week 11 – Lab 1: Text File Operations

**Total Points: 100**

## Learning Objectives

After completing this lab, students should be able to:

* Create and open a text file using Python.
* Write user-provided content to a file.
* Read information stored in a text file.
* Display file content to the user.
* Append new content without deleting existing content.
* Use the correct file access modes.
* Properly close a file after completing an operation.
* Use a `with` statement to manage files safely.
* Organize a program using a `main()` function.
* Use comments to explain file-processing operations.
* Test a program to confirm that file content is stored correctly.

## Assignment Overview

Create a Python program that demonstrates the basic text-file operations of writing, reading, and appending.

The program will:

1. Ask the user to enter content.
2. Create a text file and write the content to it.
3. Read and display the original file content.
4. Ask the user for additional content.
5. Append the additional content to the file.
6. Read and display the updated file content.

The instructor is not providing completed Python code or an exact output design. Students must design, write, and test their own programs.

## Required Python File

Create a Python file named:

`file_operations.py`

Include a comment header containing:

* Student name
* Course number
* Week number
* Lab number
* Assignment title
* Date

Example header structure:

```python
# Student Name:
# Course: CMP 131
# Week: 11
# Lab: 1
# Assignment: Text File Operations
# Date:
```

# Program Requirements

## Part 1: Display a Program Title

Display a descriptive title when the program begins.

The title should clearly indicate that the program performs text-file operations.

Example:

```text
TEXT FILE OPERATIONS PROGRAM
```

Students may create their own title and output design.

## Part 2: Ask for the Original Content

Prompt the user to enter content that will be saved in a new text file.

The prompt must clearly explain that the entered content will become the original content of the file.

For example:

```text
Enter the content you want to write to the file:
```

Store the user’s entry in a meaningful variable.

## Part 3: Create and Write to the File

Create a text file named:

`my_file.txt`

Open the file using write mode.

Write the user-provided content to the file.

Writing to the file must:

* Create `my_file.txt` if it does not already exist.
* Replace its existing content if the file already exists.
* Store the exact content entered by the user.
* Properly close the file after the writing operation finishes.

Use a `with` statement to open and manage the file.

Include comments explaining:

* Why write mode is being used.
* What information is being written.
* How the file is automatically closed.

## Part 4: Read and Display the Original Content

After writing the original content, open `my_file.txt` using read mode.

Read all the content from the file and display it to the user.

Include a clear heading before displaying the content.

Example structure:

```text
Original File Content:
This is the original content.
```

The displayed text must come from the file. Do not display only the variable that was originally entered by the user.

Use a `with` statement for the reading operation.

## Part 5: Ask for Additional Content

Prompt the user to enter additional content that will be added to the existing file.

For example:

```text
Enter additional content to append to the file:
```

Store the additional content in a meaningful variable.

The new content must be added without deleting or replacing the original content.

## Part 6: Append the Additional Content

Open `my_file.txt` using append mode.

Append the additional user-provided content to the end of the file.

The appended content should begin on a new line so that the original and additional content remain easy to read.

Appending must:

* Preserve the original content.
* Add the new content at the end of the file.
* Place the additional content on a new line.
* Properly close the file when the operation finishes.

Use a `with` statement for the appending operation.

Include comments explaining the difference between write mode and append mode.

## Part 7: Read and Display the Updated Content

After appending the additional content, open `my_file.txt` using read mode again.

Read the complete updated content and display it to the user.

Include a clear heading before the updated content.

Example structure:

```text
Updated File Content:
This is the original content.
This is the additional content.
```

The displayed text must contain both:

* The original content
* The appended content

The updated information must be read from `my_file.txt`, not created by combining the program’s variables.

## Part 8: Organize the Program

Create a `main()` function to control the program.

The `main()` function should manage the following sequence:

1. Display the program title.
2. Ask for the original content.
3. Write the original content to `my_file.txt`.
4. Read and display the original content.
5. Ask for additional content.
6. Append the additional content.
7. Read and display the updated content.
8. Display a completion message.

Call `main()` to begin the program.

# Required File Modes

Use the correct file mode for each operation.

| Operation                             | Required Mode | Purpose                                            |
| ------------------------------------- | ------------- | -------------------------------------------------- |
| Create and write the original content | `"w"`         | Creates the file or replaces its existing content  |
| Read the original content             | `"r"`         | Reads content without changing the file            |
| Add additional content                | `"a"`         | Adds content without deleting the existing content |
| Read the updated content              | `"r"`         | Reads the complete updated file                    |

Do not use write mode when adding the second entry because write mode would delete the original content.

# Example Program Interaction

The exact formatting may vary, but the program should behave similarly to the following:

```text
TEXT FILE OPERATIONS PROGRAM

Enter the content you want to write to the file:
Python makes it possible to work with text files.

Original File Content:
Python makes it possible to work with text files.

Enter additional content to append to the file:
Files can be opened in different modes.

Updated File Content:
Python makes it possible to work with text files.
Files can be opened in different modes.

The file operations were completed successfully.
```

Students should create their own prompts, headings, and output formatting.

# Required Testing

## Test 1: Basic File Creation

Enter the following original content:

```text
This is my first line of text.
```

Confirm that:

* `my_file.txt` is created.
* The entered sentence is saved in the file.
* The original content is displayed correctly.
* The program runs without errors.

## Test 2: Append Additional Content

Enter the following additional content:

```text
This line was appended to the file.
```

Confirm that the updated file contains:

```text
This is my first line of text.
This line was appended to the file.
```

Verify that:

* The original content remains in the file.
* The additional content appears after the original content.
* The additional content begins on a new line.
* Both lines are displayed by the program.

## Test 3: Replace Previous File Content

Run the program again and enter different original content.

Confirm that:

* Write mode replaces the content from the previous program run.
* The new original content is written correctly.
* Content left over from the previous run does not remain in the file.
* The new appended content is added correctly.

## Test 4: Content Containing Numbers and Symbols

Test the program using content such as:

```text
CMP 131 - Week 11 Lab 1!
```

Then append:

```text
File modes: w, r, and a.
```

Confirm that:

* Letters, numbers, spaces, and punctuation are stored correctly.
* The complete updated content is displayed.
* The program runs without errors.

# Point Distribution

* Complete comment header and descriptive program title: 10 points
* Clear prompts and meaningful variable names: 10 points
* Correctly create and write to `my_file.txt`: 20 points
* Correctly read and display the original content: 15 points
* Correctly append additional content without deleting the original: 20 points
* Correctly read and display the updated content: 15 points
* Proper use of `with`, comments, formatting, and successful testing: 10 points

**Total: 100 points**

# Code Comments

Use comments to identify and explain the major sections of the program.

Include comments for:

* Program information header
* Program title
* `main()` function
* Original user input
* File creation
* Write operation
* First read operation
* Additional user input
* Append operation
* Final read operation
* Final output

Comments should briefly explain the purpose of each major section. They should not repeat every Python statement word for word.

# General Requirements

* Use Python to complete the program.
* Create the required `file_operations.py` file.
* Create and use a text file named `my_file.txt`.
* Include and call a `main()` function.
* Use meaningful and consistent variable names.
* Use a `with` statement for every file operation.
* Use write mode to create or replace the file content.
* Use read mode to retrieve content from the file.
* Use append mode to add new content.
* Preserve the original content during the append operation.
* Place the appended content on a new line.
* Display both the original and updated file content.
* Include a complete comment header.
* Include comments explaining all major file operations.
* Use clear prompts, headings, labels, and messages.
* Complete all required testing.
* Check spelling, capitalization, grammar, and punctuation.
* Make sure the program runs without errors.
* Follow the course AI-use policy.
* Record any AI assistance in `AI-Use-Report.md`.

# Required Organization

Organize the assignment as follows:

* `Week-11`

  * `Lab-01`

    * `CMP131-Week-11-Lab-01.md`
    * `AI-Use-Report.md`
    * `src`

      * `file_operations.py`

The `my_file.txt` file will be created when the Python program runs.

# Submission Requirements

Submit or push the complete `Lab-01` folder.

The submission must include:

* `file_operations.py`
* `AI-Use-Report.md`

Before submitting, verify that:

* The required Python file is included.
* The filename is exactly `file_operations.py`.
* The program contains a complete comment header.
* The program includes and calls a `main()` function.
* The program asks the user for original content.
* The program creates `my_file.txt`.
* The original content is written using write mode.
* The original content is read from the file and displayed.
* The program asks the user for additional content.
* The additional content is added using append mode.
* Appending does not erase the original content.
* The appended content begins on a new line.
* The updated content is read from the file.
* Both the original and appended content are displayed.
* A `with` statement is used for each file operation.
* Comments explain all major file operations.
* All required tests were completed.
* The program runs without errors.
* The AI-use report is complete.
* The latest work has been committed and pushed to GitHub.

# Suggested Git Commit Messages

* Create Week 11 Lab 1 Python file
* Add original content input
* Write original content to text file
* Read and display file content
* Add append operation
* Display updated file content
* Improve file-operation comments
* Test text file operations
* Complete Week 11 Python lab

---

## GitHub Starter Repository

Use the following public starter repository:

[CMP131-Week-11-Lab-01](https://github.com/ahedhli12/CMP131-Week-11-Lab-01)

### Getting Started

1. Open the starter repository using the link above.
2. Select **Use this template → Create a new repository** when the template option is available.
3. Choose your personal GitHub account as the owner.
4. Name your repository `LastName-FirstName-CMP131-Week-11-Lab-01`.
5. Set your repository to **Public**.
6. Clone your own newly created repository—not the instructor’s starter repository.
7. Open the entire cloned folder in Visual Studio Code.
8. Complete and test every required Python file.
9. Commit and push your work to GitHub.
10. Verify that your latest files appear on GitHub.
11. Complete `AI-Use-Report.md`.
12. Submit the required work through Blackboard Ultra and include your public repository link when requested.

### Required Repository Files

- `CMP131-Week-11-Lab-01.md`
- `AI-Use-Policy.md`
- `AI-Use-Report.md`
- `file_operations.py`

### Before You Submit

- [ ] All required Python files are in the repository root.
- [ ] Every required filename is exact.
- [ ] Each program runs successfully.
- [ ] Required tests and screenshots are complete.
- [ ] `AI-Use-Report.md` is complete and accurate.
- [ ] The latest commit is visible on GitHub.
