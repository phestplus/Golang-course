## Exercise Submission Guidelines

This section explains how students should submit exercises for the **Mastering Golang** course. Following this process ensures submissions are **organized, reviewable, and conflict-free**.

---

### 1. Folder Structure for Submissions

Each student should create a **personal folder** inside the `exercises/` directory. This keeps exercises separated and easy to review.

**Recommended structure:**

```text
exercises/
├── john_smith_exercise/
│   ├── module1/
│   │   ├── step1_hello_world.go
│   │   └── step2_variables.go
│   ├── module2/
│   │   └── step5_arrays.go
│   └── module3/
│       └── step12_functions.go
├── jane_doe_exercise/
│   └── module1/
│       └── step1_hello_world.go
```
Rules:

1. Top-level folder: Your full name with underscores, followed by _exercise.

Example: john_smith_exercise



2. Module folders: Each module you are submitting exercises for gets a folder.

Example: module1, module2, etc.



3. Exercise files: Name each file with the step number and exercise name.

Example: step1_hello_world.go, step12_functions.go




> Optional: Add a header comment to each file:



// Author: John Smith
// Module: 1
// Step: 1 - Hello World


---

2. Submission Workflow (Recommended: Fork + Pull Request)

Because the repository is public, students cannot push directly. The safest method is via forks and pull requests.

Step 1: Fork the repository

1. Go to the repository page on GitHub.


2. Click Fork (top-right corner).


3. Clone your fork to your local machine:


```
git clone https://github.com/your-username/golang-course.git
cd golang-course
```


---

Step 2: Create your exercise folder

```
mkdir -p exercises/john_smith_exercise/module1
```
Replace john_smith with your GitHub/real name.

Add your solution files inside the module folder.



---

Step 3: Add your solution files

Example:
```
cd exercises/john_smith_exercise/module1
touch step1_hello_world.go
# Open the file and write your solution
```

---

Step 4: Stage and commit your changes
```
git add exercises/john_smith_exercise
git commit -m "Add Module 1 exercises for John Smith"
```

---

Step 5: Push to your fork

git push origin main

Or push to a separate branch:
```
git checkout -b john_smith_module1
git push origin john_smith_module1
```

---

Step 6: Open a Pull Request

1. Go to your fork on GitHub.


2. Click Compare & Pull Request.


3. Submit the PR to the main repository.


4. Include a short description:



Module 1 exercises submission
Student: John Smith
Includes: Step1_hello_world.go, Step2_variables.go

You will be notified when your submission is reviewed. Reviewers may provide feedback before merging.


---

3. Best Practices

Only submit exercise code; do not include compiled binaries.

Follow the folder and file naming conventions strictly.

Keep your code clean and modular — one step per file.

Optional: Include short comments explaining your logic.

If you make updates, commit new changes and push to your branch/fork — the PR will update automatically.



---

4. Notes for Instructors

The per-student folder structure makes it easy to track progress.

Using forks and PRs ensures students can submit safely without overwriting each other’s work.

You can use GitHub Actions to automatically check Go formatting (go fmt) or run unit tests on submissions.



---

✅ Summary

1. Fork the repo → clone locally.


2. Create your your_name_exercise folder.


3. Add module folders and solution files.


4. Commit & push to your fork or branch.


5. Open a Pull Request for review.



This workflow keeps submissions organized, safe, and professional, making it ideal for a GitHub-based course.