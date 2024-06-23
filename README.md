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

4. Making Changes and Committing:

* Make changes to a file or add a new file:
 
 echo "print('Hello, World!')" > hello.py

* Commit the changes:

git add hello.py
git commit -m "Add hello.py with a print statement"

![alt text](<Screenshot 2024-06-23 115209.png>)

5. Merging Changes

* Switch back to the main branch:

git checkout main


* Merge the changes from the feature-update branch

git merge feature-update

![alt text](<Screenshot 2024-06-23 115707.png>)

Task 3: Handling Conflicts

In your forked repository on GitHub, make changes to the same file (e.g., hello.py) and commit them via the web interface.
Pull the changes to your local machine: usign git pull

![alt text](<Screenshot 2024-06-23 121030.png>)

7. Resolving Conflicts

Create a new branch to resolve the conflic using this command:

git checkout -b conflict-resolution

Resolve the conflict manually in the file (edit hello.py to resolve the differences).
Commit the changes and merge the branch back into main:

git add hello.py
git commit -m "Resolve conflict in hello.py"
git checkout main
git merge conflict-resolution

![alt text](<Screenshot 2024-06-23 121622.png>)

