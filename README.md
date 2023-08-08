# git_assignment_HeroVired

# Question 1 :-

Presented here is a Python application called "CalculatorPlus.py." This application is designed to perform basic arithmetic operations, including addition, subtraction, multiplication, and division. An additional feature has been integrated, allowing for the calculation of square roots.

Stepwise Procedure
Initiate by creating a Git repository named "git_assignment_HeroVired" and proceed to clone the repository to your local environment.

Clone using the repository's SSH link:

``` 
git clone <GitHub repo SSH link>
```

Create a new branch, "dev" for making code modifications within this branch.

Create and switch to the "dev" branch:
```
git checkout -b dev
```

Develop a Python file named "CalculatorPlus" and introduce the basic arithmetic calculations.

Stage the newly created file in the "dev" branch and commit the changes.

Check the status of staged files:
```
git status
```

Add the file to the staging area:
```
git add CalculatorPlus.py
```

Commit the staged changes with a descriptive message:
```
git commit -m "Add commit message here"
```

Merge the recent "dev" branch commit into the "main" branch.

Switch to the "main" branch:
```
git checkout main
```

Merge recent "dev" commits into the "main" branch:
```
git merge dev
```

Push changes from local "main" to "origin/main":
```
git push
```

Release the initial version of the code.

![image](https://github.com/madans95/git_assignment_HeroVired/assets/49802479/fa8ad262-5aac-4fb1-87a4-c7f0fc9436eb)

Create a new branch named "feature_sqrt" and switch to it.

Create the branch:
```
git branch feature_sqrt
```
Switch to the newly created branch:
```
git checkout feature_sqrt
```
Integrate the 'sqrt' code into the "feature_sqrt" branch and temporarily stash it.

Stash the changes:
```
git stash
```

Due to a critical bug reported in the main branch, switch back to the "dev" branch for bug fixing.

i. Implement a fix for the "divide function" code in the "CalculatorPlus.py" file within the "dev" branch.

ii. Stage and commit the changes to the "CalculatorPlus.py" file in the "dev" branch. Push the corrected code to the remote "Dev Origin.
```
git checkout dev

“git add CalculatorPlus.py”

“git commit -m "message" 

“git log”      -- to check the newly added commit info

“git push”  -- the origin/dev will be moved to the latest commit or the same as local HEAD in Git Log.
```

Create a "Pull Request" from the remote repository to merge code from "dev" into "main," allowing collaborators to review the changes.

After the Pull Request is reviewed and approved by collaborators, return to the "feature/sqrt" branch and retrieve the temporarily stashed code for the "Square" function.

Retrieve the stashed changes:
```
git stash pop
```
Proceed to merge the code into the "dev" branch and then push it to the remote "Dev Origin."

Switch to the "dev" branch:
```
git checkout dev
```
Merge the changes from the "feature/sqrt" branch:
```
git merge feature/sqrt
```
Push the changes:
```
git push
```
Test the functionality to confirm smooth operation. Initiate a Pull Request from the "Dev Origin" to the "Main Origin" to reflect all changes in the main branch.

ii. Create a 'version 2' release using GitHub.

![image](https://github.com/madans95/git_assignment_HeroVired/assets/49802479/0b49a72a-3b88-4dc8-8005-7cd77d5ec025)

# Question 2:-

Uploaded a 200 MB ".pdf" file using Git LFS

Install Git LFS.
```
git lfs install
```

Create a Branch LFS and checkout into it. 
```
git branch lfs
git checkout lfs
git status
```

Keep a pdf file of more than 200 MB in the directory git is initialized
& Track the large file(pdf in this case).
```
git lfs track "*.pdf"
git status
```

Add the files & Commit it.
```
git add .gitattributes
git add 200MB PDF File-lfs.pdf
git commit -m "Track the Large 200MB file via Git LFS"
```

To View all the LFS files getting tracks.
```
git lfs track
```

Push the commit to the origin lfs.
```
git push -u origin lfs
```

Clone the Repo in any other folder to Check if the Large File is getting downloaded properly.
```
git clone < ssh repo link>
```

# Question 3:-
 
Create new branch named "geometry-calculator"
```
git branch -b geometry-calculator
```

Create a new file "geometry-calculator.py" and add initial code to it.

Created a new branch named "feature/circle-area" from "geometry-calculator" to work on the circle-area feature.
```
git checkout -b feature/circle-area
```
Add Circle Area Feature in the "feature/circle-area" branch.

Stash Changes for Circle Area Feature:

Before committing the changes, stash them using git stash to save the incomplete feature implementation.
```
git stash
The File should not appear while checking the git status
```
git status
```
Create a New Branch for Rectangle Area Feature:

Create a new branch named "feature/rectangle-area" from "geometry-calculator" to work on the rectangle area.
```
git checkout -b feature/rectangle-area
```

Add code for Rectangle Area Feature in the "feature/rectangle-area" branch & Stash it.
```
git stash
```
The File should not appear while checking the git status
```
git status
```
Switch Back to Circle Area Branch commit and Push Circle Area Feature:

Switch back to the "feature/circle-area" branch to continue working on the circle-area feature.
```
git checkout feature/circle-area
```
View all the stash presents.
```
git stash list
```
Retrieve the stash for circle-area code
```
git stash apply {stash-id of the stash made for circle-area code}
```
Complete the circle area feature implementation and save the changes.
```
git add *
git commit -m ”commit circle-area code
```
Switch Back to Rectangle Area Branch & commit and Push Rectangle Area Feature:

Switch back to the "feature/rectangle-area" branch to continue working on the rectangle area feature.
```
git checkout feature/rectangle-area
```
Retrieve the stashed changes
```
git stash list
git stash apply {stash-id of the stash made for rectangle-area code}
```
Complete the rectangle area feature implementation and save the changes.
```
git add *
git commit -m ”commit rectangle-area code
```
Create Pull Requests:

Merge two branch "feature/rectangle-area" and "feature/circle-area" to "geometry-calculator"
```
git checkout geometry-calculator
git merge feature/rectangle-area
git merge feature/circle-area
```

Create a pull request to the ‘dev’ branch.
Fromm the git hub create a pull request from "geometry-calculator" to "dev" Branch.

Review and Merge
Have another team member or reviewer review your pull requests.
After receiving approval, merge both pull requests into the main branch.



