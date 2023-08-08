# git_assignment_HeroVired

Question 1 :-

Presented here is a Python application called "CalculatorPlus.py." This application is designed to perform basic arithmetic operations, including addition, subtraction, multiplication, and division. An additional feature has been integrated, allowing for the calculation of square roots.

Stepwise Procedure
Initiate by creating a Git repository named "git_assignment_HeroVired" and proceed to clone the repository to your local environment.

Clone using the repository's SSH link:

"git clone <GitHub repo SSH link>"

Create a new branch, "dev," for making code modifications within this branch.

Create and switch to the "dev" branch:

git checkout -b dev

Develop a Python file named "CalculatorPlus" and introduce the basic arithmetic calculations.

Stage the newly created file in the "dev" branch and commit the changes.

Check the status of staged files:

git status

Add the file to the staging area:

git add CalculatorPlus.py

Commit the staged changes with a descriptive message:

git commit -m "Add commit message here"

Merge the recent "dev" branch commit into the "main" branch.

Switch to the "main" branch:

git checkout main

Merge recent "dev" commits into the "main" branch:

git merge dev

Push changes from local "main" to "origin/main":

git push

Release the initial version of the code.

![image](https://github.com/madans95/git_assignment_HeroVired/assets/49802479/fa8ad262-5aac-4fb1-87a4-c7f0fc9436eb)

Create a new branch named "feature/sqrt" and switch to it.

Create the branch:

git branch feature_sqrt

Switch to the newly created branch:

git checkout feature/sqrt

Integrate the 'sqrt' code into the "feature/sqrt" branch and temporarily stash it.

Stash the changes:

git stash

Due to a critical bug reported in the main branch, switch back to the "dev" branch for bug fixing.

i. Implement a fix for the "divide function" code in the "CalculatorPlus.py" file within the "dev" branch.

ii. Stage and commit the changes to the "CalculatorPlus.py" file in the "dev" branch. Push the corrected code to the remote "Dev Origin."

*******edit*********

Create a "Pull Request" from the remote repository to merge code from "dev" into "main," allowing collaborators to review the changes.

After the Pull Request is reviewed and approved by collaborators, return to the "feature/sqrt" branch and retrieve the temporarily stashed code for the "Square" function.

Retrieve the stashed changes:

git stash pop

Proceed to merge the code into the "dev" branch and then push it to the remote "Dev Origin."

Switch to the "dev" branch:

git checkout dev

Merge the changes from the "feature/sqrt" branch:

git merge feature/sqrt

Push the changes:

git push

Test the functionality to confirm smooth operation. Initiate a Pull Request from the "Dev Origin" to the "Main Origin" to reflect all changes in the main branch.

ii. Create a 'version 2' release using GitHub.

![image](https://github.com/madans95/git_assignment_HeroVired/assets/49802479/0b49a72a-3b88-4dc8-8005-7cd77d5ec025)




