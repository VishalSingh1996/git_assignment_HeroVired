# Git Assignment HeroVired

## Project Overview

This repository contains work for multiple assignments including:

- Basic CalculatorPlus App with new feature (Square Root)
- Git LFS (Large File Storage) handling for large files
- Geometry Calculator using Git stash and branch management

This repository is created as part of a Git assignment for Hero Vired.

---

## Repository Name

> **git\_assignment\_HeroVired**

---

# Tasks Completed

## Question 1: CalculatorPlus Application

### 1. Initial Setup

- Created repository: `git_assignment_HeroVired`
- Created and switched to `dev` branch.
- Added basic Calculator code with Addition, Subtraction, Multiplication, and Division methods.

### 2. Implement Square Root Feature

- Created a new branch: `feature/sqrt`
- Uncommented and completed the `square_root` function:

```python
import math

def square_root(self, x):
    return math.sqrt(x)
```

- Tested the Square Root functionality successfully.

### 3. Bug Fix in Division

- Found a bug where division by zero was not handled.
- Switched to `dev` branch.
- Fixed the `divide` function:

```python
def divide(self, a, b):
    if b == 0:
        raise ValueError("Cannot divide by zero.")
    return a / b
```

- Merged the bug fix into `feature/sqrt` branch to keep it updated.

### 4. Pull Request and Review

- Created a Pull Request from `feature/sqrt` to `main`.
- Requested code review from a classmate.
- Incorporated feedback from the reviewer.

### 5. Final Merging

- Merged `feature/sqrt` into `dev`.
- Performed testing in `dev`.
- Merged `dev` into `main`.

### 6. Releases

- **Version 1.0** after basic Calculator.
- **Version 2.0** after adding Square Root and fixing Divide bug.

### Tools Used:

- **Visual Studio Code**: for writing code and testing.
- **Git CLI**: for branching, committing, merging, and pull requests.

---

## Question 2: Git LFS (Large File Storage)

### 1. Branch Creation

- Created new branch: `lfs`.

### 2. Git LFS Setup

- Installed Git LFS:

```bash
git lfs install
```

- Tracked large files:

```bash
git lfs track "*.zip"
```

- `.gitattributes` file was automatically created.

### 3. Uploading Large File

- Uploaded a file larger than 200MB.
- Committed and pushed the file:

```bash
git add .
git commit -m "Added large file using Git LFS"
git push origin lfs
```

### 4. Verification

- Cloned the repository on another system.
- Confirmed large files downloaded successfully using Git LFS.

### Tools Used:

- **Git CLI**: for Git LFS installation, adding, pushing.
- **GitHub**: for LFS management and verification.

---

## Question 3: Geometry Calculator using Git Stash

### 1. Branch Creation

- Created a branch: `geometry-calculator`.

### 2. Circle Area Feature

- Created a new branch: `feature/circle-area`.
- Wrote partial code:

```python
def calculate_circle_area(self, radius):
    return math.pi * radius ** 2
```

- Stashed incomplete work:

```bash
git stash
```

### 3. Rectangle Area Feature

- Created a new branch: `feature/rectangle-area`.
- Wrote partial code:

```python
def calculate_rectangle_area(self, length, width):
    return length * width
```

- Again stashed the incomplete work:

```bash
git stash
```

### 4. Completing Features

- Switched to `feature/circle-area` branch.
- Retrieved stashed changes:

```bash
git stash pop
```

- Completed and pushed circle feature.

- Switched to `feature/rectangle-area` branch.

- Retrieved stashed changes.

- Completed and pushed rectangle feature.

### 5. Pull Requests

- Created two pull requests:
  - `feature/circle-area` ➞ `dev`
  - `feature/rectangle-area` ➞ `dev`
- Got both PRs reviewed and approved.

### 6. Final Merging

- After testing both features in `dev`, merged into `main`.

### Tools Used:

- **Visual Studio Code**: for coding and testing.
- **Git CLI**: for branching, stashing, committing, merging.
- **GitHub**: for pull requests and code management.

---

# How to Run the Applications

## CalculatorPlus

```bash
python calculatorplus.py
```

## Geometry Calculator

```bash
python geometrycalculator.py
```

---

#  Contributor

- Kevin Koreth

---

#  Important Learning Points

- Creating and managing feature branches
- Handling large files using Git LFS
- Managing multiple incomplete features using Git Stash
- Bug fixing and code review workflows
- Best practices for working in a team using Git and GitHub

---

#  Final Releases

- **Version 1.0** - Basic Calculator
- **Version 2.0** - Added Square Root and bug fix

---

#  Thank you! 
