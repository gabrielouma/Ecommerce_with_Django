# Task 1: Cloning and Forking
1. Cloning a Repository
Choose a public GitHub repository of interest (for example Ecommerce with Django).

2. Open a git bash and clone the repository: using git clone commad


3. Explore the repository's structure, files, and history:

cd tensorflow
ls
git log --oneline

![alt text](<Screenshot 2024-06-23 113640.png>)

#  Forking a Repository

* Go to the repository page on GitHub and click the "Fork" button at the top right.
![alt text](<git fox.png>)

On the top right of the repository page, you'll find a "Fork" button.

Click it. This creates a copy of the repository under your GitHub account.

3. Clone Your Fork:

Use the same git clone command as before, but with the URL of your fork.
![alt text](<Screenshot 2024-06-23 114054.png>)

# Task 2: Managing Branches
* Creating and Switching Branches
 git checkout -b feature-update

Switch to the newly created branch:

git checkout feature-update

![alt text](<Screenshot 2024-06-23 114414.png>)

# 4. Making Changes and Committing:

* Make changes to a file or add a new file:
 
 echo "print('Hello, World!')" > hello.py

* Commit the changes:

   To make changes to a file in your forked repository on GitHub and commit them via the web interface, follow these steps:

    Navigate to Your Forked Repository:

    Go to GitHub and navigate to the forked repository where you want to make changes.

   Locate the File:

   In the repository, locate the file you want to edit (in this case, hello.py). You can find it by browsing through the directory structure.

   Edit the File:

   Click on the file name (hello.py) to open it. Then, click on the pencil icon (🖉) at the top right of the file view to enter edit mode.
   ![alt text](<Screenshot 2024-06-23 131005.png>)
   Make Your Changes:

   Edit the file content in the text editor. For example, you might change the content to:

git add hello.py
git commit -m "Add hello.py with a print statement"

![alt text](<Screenshot 2024-06-23 115209.png>)

5. Merging Changes

* Switch back to the main branch:

git checkout main


* Merge the changes from the feature-update branch

git merge feature-update

![alt text](<Screenshot 2024-06-23 115707.png>)

# Task 3: Handling Conflicts

In your forked repository on GitHub, make changes to the same file (e.g., hello.py) and commit them via the web interface.
Pull the changes to your local machine: usign git pull

![alt text](<Screenshot 2024-06-23 121030.png>)

# 7. Resolving Conflicts

   Resolving conflicts in Git typically occurs when you have conflicting changes in the same file between different branches.

   Identify the Conflict:

   Git will notify you if there's a conflict during a merge or rebase operation. It will mark the conflicting sections in the file hello.py with special markers like <<<<<<<, =======, and >>>>>>>.

   Open the File:

   Open hello.py in a text editor. Look for the conflict markers (<<<<<<<, =======, >>>>>>>) and the conflicting changes between them.

   Resolve the Conflict:

   Decide how to merge the conflicting changes. You may want to keep some parts, discard others, or modify them to create a unified version.

  Remove Conflict Markers:
   
  Delete the conflict markers (<<<<<<<, =======, >>>>>>>) and ensure the file looks correct after merging the changes.

Save the File:

  Save the changes to hello.py in your text editor.

  Add and Commit the Resolved File:

  After resolving the conflict, add the modified hello.py file to the staging area and commit the merge resolution:

 Create a new branch to resolve the conflic using this command:

 git checkout -b conflict-resolution

 Resolve the conflict manually in the file (edit hello.py to resolve the differences).

 Commit the changes and merge the branch back into main:

git add hello.py
git commit -m "Resolve conflict in hello.py"
git checkout main
git merge conflict-resolution

![alt text](<Screenshot 2024-06-23 121622.png>)

# Task 4: GitHub Pages
Enabling GitHub Pages

Create a simple HTML file

 <!DOCTYPE html>
 <html lang="en">
    
 <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Pages</title>
 </head>
 <body>
    <h1>Hello, GitHub Pages!</h1>
 </body>
 </html>

  2. commit and push the file:

     git add index.html
     git commit -m "Add index.html for GitHub Pages"
     git push origin main

  * Enable GitHub Pages in the repository settings:
 * Go to the repository on   GitHub.
 *  Click on "Settings."

  ![alt text](<Screenshot 2024-06-23 132049.png>)

   Scroll down to the "GitHub Pages" section.

 *  Select the source branch (main) and save.

 9. Accessing the Published Page:

  - Visit the GitHub Pages URL for your repository and verify that the HTML file is accessible online.

  ![alt text](<Screenshot 2024-06-23 132331.png>)

  Task 5: Open Source Exploration

10. Exploring Open Source Projects

  Search for an open-source project on GitHub related to your interests (e.g., Django).

  Explore the project's documentation, issues, and contribution guidelines.
11. Opening an Issue

    Open a new issue in the chosen open-source project, suggesting an improvement, reporting a bug, or asking for clarification.

    # Challenges:
    * Forgetting to switch branches before making changes can lead to errors, and accidental branch deletions or loss of branch names can cause confusion.

    * Forgetting to commit and push changes can lead to errors, and accidental loss of changes can cause confusion.

    * Forgetting to resolve conflicts can lead to errors, and accidental loss of changes can cause confusion.

    # mitigations
    * Have a good understanding of Git commands and workflows.

    * Double-check commands before executing them to avoid mistakes.

    * Communicate and collaborate effectively with team members or peers when working on shared repositories.

    * Regularly review Git documentation and best practices.

    

