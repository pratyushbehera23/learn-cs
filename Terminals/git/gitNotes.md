# Git

```sh

git --version

# 

git config --global user.name "user-name"
git config --global user.email "user-email"

git config --global


#  

mkdir FolderName
cd FolderName

git init

ls / ls -a

#  

code .
# make program files of any lang. and code

git status

git add .

git commit -m "message"

#  

git log

git diff file_name

git checkout HASHCODE_of_gitLog

# 

git branch branch_name

git checkout branch_name

git checkout master

git merge branch_name

# 

git clone url_of_repo_to_clone_to_local
git log

# 

# Github collab (contribute to someone's repo):
# Fork the repo (repo copied to your github)
# Git clone _url_ (to local repo in your pc)
# Modify or add code
# Git push origin master
# Pull request to the owner of repo
```

```sh
# Generally, if you're creating locally first, you would go:

# Set up the Git repo locally, with no commits in it:
git init

# Add a new file:
git add file_name 
# Add multiple files:
git add . 

# Commit the change:
git commit -m "message"

# Tell Git where your remote is (once):
git remote add origin https://github.com/user/repo.git 

# Push the default 'master' branch to the above remote called 'origin':
git push origin master 

----------

If it already exists on Github (or a different remote server):

# Download the existing repo, with all of the history.
git clone https://bitbucket.org/user/repo.git

# Add a new file or modify any file of the repo, then:
git add file_name  OR  git add .

# Commit the change.
git commit -m "message"

# Push to the remote that you downloaded from with clone on branch master.
git push origin master

-----------

# Check status
git status

# Commit history
git log

# Changes made
git diff file_name

# Checkout previous commit
git checkout 50781d57bched23yd8fhb7f588ff0ac256 (e.g hash from - git log)

# Branch
git branch branch_name

# Checkout branch
git checkout branch_name

# Branch & checkout into it
git checkout -b branch_name

# Merge branch
git checkout master
git merge branch_name

# Check remote
git remote -v

#
git branch -M master
git push -u origin master
```
