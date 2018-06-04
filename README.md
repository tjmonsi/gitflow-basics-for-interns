# gitflow-basics-for-interns
Gitflow basics for interns
------------------------------
<h3>How to Gitflow</h3>

**_Create Git Repository:_**
	1. Login to github
	2. Create a new repository by clicking `New Repository`
	3. Fill out the necessary details of your repository
	4. Click on create repository

**_Create a Develop Branch:_**
	1. Clone the repository
	2. Initialize the repository
	3. `git checkout -b Develop`

**_Create New Issue for Each Task:_**
	1. Create issue by going to `Issues` and click `New Issue`
	2. Fill out the necessary details about the issue

**_Create New Branch for Each Issue:_**
	1. `git checkout -b <task-name-issue#>`
	2. `git push -u origin <branch-name>`
	3. Perform the task
	4. Add, commit, and push the task to the branch
	5. Pull request and merge branch to the `Develop` branch
	6. Delete the repository branch of the finished task
	7. `git branch -d <branch-name>` to delete the local branch
	8. `git checkout develop` and `git pull` to update the develop branch

**_Merge the Develop Branch to Master Branch:_**
	`Note: Make sure all tasks passed all necessary tests before merging.`
	1. Create new pull request with `Base: Master` and `Compare: Develop`
	2. `Merge Pull Request`