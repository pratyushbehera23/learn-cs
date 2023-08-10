# Repo

## Create repository: (for every new project)

Open github -> click [+] on top-right corner -> New repository
Enter repository name, description, public/private -> Create repo
Copy the link

## Link local proj to github repo

### To copy from PC to Github

PC: Goto the project folder -> right click -> git bash here

```sh
    > git init
    > git add .
    > git commit -m "initial commit"
    > git remote add origin _link_ # (copied github repo link)
    > git push -u origin master
```

### To copy from Github to PC

PC: Goto the project folder -> right click -> git bash here

```sh
    > git clone _link_
    > cd foldername # (folder created after cloning the repo)
    # {add/write your code}
    > git add .
    > git commit -m "initial commit"
    > git push
```

> Process: Working directory -> (`git add`) -> Staging area -> (`git commit`) -> local repository -> (`git push`) -> remote repository (Github)
