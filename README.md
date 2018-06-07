# gitflow-basics-for-interns
Gitflow basics for interns
------------------------------
<h3>How to Gitflow</h3>

**_Create Git Repository:_**
	(Github)
	1. Login to github
	2. Create a new repository by clicking `New Repository`
	3. Fill out the necessary details of your repository
	4. Click on create repository

**_Create a Develop Branch:_**
	(Terminal)
	1. Clone the repository
	2. Go to the directory of the cloned repository
	`Note: By default, the master branch will be currently selected`
	3. `git checkout -b develop` to create the develop branch
	Note: The newly created branch `develop` will become the selected branch
	4. `git push origin develop` to put the develop branch in the remote repository

**_Create New Issue for Each Task:_**
	(Github)
	1. Create issue by going to `Issues` and click `New Issue`
	2. Fill out the necessary details about the issue

**_Create New Branch for Each Issue:_**
	(Terminal)
	1. From the develop branch, create a new branch using: `git checkout -b <branch-name>`
	`Note: Branch name would usually go like: <task-name-issue#>`
	2. `git push -u origin <branch-name>`
	3. Complete the said task
	4. `git add .` to add the updated set of files
	5. `git commit -m "<task-description-fix-issue#>"` to save changes
	6. `git push origin <branch-name>`

**_Update the Develop Branch:_**
	(Github)
	1. Create a pull request to compare the develop branch and the task-branch
	2. Merge task-branch to the `Develop` branch
	3. Delete the repository branch of the finished task
	`Note: The delete button will be shown once the two branches are merged.`
	(Terminal)
	4. `git checkout develop` and `git pull` to update the develop branch
	5. `git branch -d <branch-name>` to delete the local branch

**_Merge the Develop Branch to Master Branch:_**
	`Note 1: Only the project manager should perform this task`
	`Note 2: Make sure all tasks passed all necessary tests before merging.`
	1. Create new pull request with `Base: Master` and `Compare: Develop`
	2. `Merge Pull Request`