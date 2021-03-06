# GitHub Intro

- Step 1
------
	Login to github.com and signup for a free account.
	If you need a private repository then you need to signup for paid account.

- Step 2
------
	Login to your Linux machine and create a direcotry for git
```
	# mkdir /git
```
- Step 3
------
	Configure your username and email. So that if someone did any commit then everyone will know who have made it.
```
	# git config --global user.name "User Name"
	# git config --global user.email <email_id>
```
- Step 4
------
	Go to that directory and create a new directory for your repository if you
	have multiple branches within the repository in your git account.
	Else you can add your repository directly.
	
	- Case 1: Repository with default branch or a single branch.
		Go to your git directory
```
		# cd /git
```		
		Update the origin of your repository
```
		# git remote add -t <Branch_Name> -f origin https://<username>@github.com/<username>/<Repo_name>.git
		# git remote add -t master -f origin https://vmsnivas@github.com/vmsnivas/ansible.git
```		
		Clone your repository now.
```
		# git clone https://vmsnivas@github.com/vmsnivas/ansible.git
```		
	- Case 2: Repository with multiple branches.
		Go to your git directory.
```
		# cd /git
```		
		Create a direcotry with the name of the repository and child direcotries with the name of the branches you have.
```
		# mkdir -p <repo_name>/{branch1,branch2,....}
		# mkdir -p python/{master,notes,programs}
```		
		Go to the repo dir and initialize git.
```
		# cd python
		# git init
```		
		Set the origin of your repo.
```
		# git remote set-url origin https://<username>@github.com/<username>/<Repo_name>.git
		# git remote set-url origin https://vmsnivas@github.com/vmsnivas/python.git
```		
		Go to one of your branches and initialize git.
```
		# cd master
		# git init
```		
		Update the origin of your branch
```
		# git remote add -t branch1 -f origin https://<username>@github.com/<username>/<Repo_name>.git
		# git remote add -t master -f origin https://vmsnivas@github.com/vmsnivas/python.git
```		
		Now clone the contents of that specific branch from the repo.
```
		# git clone -b branch1 https://<username>@github.com/<username>/<Repo_name>.git
		# git clone -b master https://vmsnivas@github.com/vmsnivas/python.git
```