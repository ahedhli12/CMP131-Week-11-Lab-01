# CMP 131 – Python Programming

> **Required file location:** Keep every Python file directly in the repository root. Do not create a `src` folder.

## Week 11 – Lab 1: Text File Operations

**Total Points: 100**

## Learning Objectives

After completing this lab, students should be able to:

- Create and open a text file using Python.
- Write user-provided content to a file.
- Read information stored in a text file.
- Display file content to the user.
- Append new content without deleting existing content.
- Use correct file access modes.
- Manage files safely using a `with` statement.
- Organize a program using a `main()` function.
- Test that stored file content is correct.

## Assignment Overview

Create one Python program named `file_operations.py` that demonstrates writing, reading, and appending to a text file.

The program will:

1. Ask the user to enter original content.
2. Create a text file and write the content to it.
3. Read and display the original file content.
4. Ask the user for additional content.
5. Append the additional content without deleting the original content.
6. Read and display the updated file content.

The instructor is not providing completed Python code or an exact output design. Students must design, write, and test their own program.

# Program Requirements

Create `file_operations.py`.

Your program must:

- Display a descriptive title.
- Ask the user for original text content.
- Create a text file named `my_file.txt`.
- Write the original content to the file.
- Close or safely release the file after writing.
- Open the file for reading.
- Read and display the stored content.
- Ask the user for additional content.
- Open the same file in append mode.
- Add the new content without removing what was already stored.
- Open the file again for reading.
- Display the complete updated file content.
- Use appropriate file modes for writing, reading, and appending.
- Use `with` statements to manage file access safely.
- Organize the program using a `main()` function.

The finished program should leave `my_file.txt` containing both the original and appended information.

## Required Testing

Test the program more than once. Confirm that:

- The file is created when the program runs.
- The original content is written correctly.
- The original content can be read back and displayed.
- Appending does not erase the original content.
- The updated file contains both entries.
- The final displayed content matches the file.
- The program runs without errors.

# Code Comments

Include a comment header containing:

- Student name
- Course number
- Week number
- Lab number
- Assignment title
- Date

Use comments to identify major sections such as original input, writing, reading, appending, updated reading, and final output.

# General Requirements

- Use meaningful variable names.
- Keep `file_operations.py` directly in the repository root.
- The program may create `my_file.txt` when it runs.
- Use safe and appropriate file-processing techniques.
- Make sure the program runs without errors.
- Follow `AI-Use-Policy.md`.
- Complete `AI-Use-Report.md` honestly.

# Submission Requirements

Your repository must include:

- `CMP131-Week-11-Lab-01.md`
- `file_operations.py`
- `AI-Use-Policy.md`
- `AI-Use-Report.md`

Before submitting:

1. Run and test the program.
2. Confirm `my_file.txt` is created and updated correctly.
3. Confirm the Python filename is correct and located in the repository root.
4. Complete the AI-use report.
5. Commit and push your latest work.
6. Verify the newest files on GitHub.
7. Submit through Blackboard Ultra as directed.

**Do not push your work to the instructor's starter repository.**
