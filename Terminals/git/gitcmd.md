# Git

```sh
Start:
1. Download install open the ‘Git Bash App’
    Check git version
    > git --version

2. You need to set who you are before creating any commit. 
    That will allow commits to have the right author name and email associated to them.
    In the terminal type the following commands in sequence to configure gitbash with your GitHub username and email address:
        > git config --global user.name “GitHub_user_name_here”
        ‘Press enter’
        > git config --global user.email “GitHub_email_address_here”
        ‘Press enter’
    It has nothing to do with authentication when pushing to a remote repository 
    (e.g. when pushing to a remote repository using your GitHub, BitBucket, or GitLab account)

3. You can check whether you have configured with the correct details by typing the below command:
    > git config –list
    ‘Press Enter’
    You can now close the terminal.

4. Next, let us learn how to create a public repository. 
    Log in to GitHub and then click on the ‘+’ symbol on the top right corner of the screen. 
    Then click on ‘New Repository’. 
    Enter a repository name of your choice, an optional Description, choose Public option, and then click on Create Repository.

5. In a location of your choice in your PC, create a new folder where you will be adding your codes. 
    Open the folder and right click anywhere on the screen. 
    Then click on “Git Bash Here” to open the terminal.
    Open the newly created repository from your GitHub account and click on the ‘copy’ symbol to copy the HTTP link (which will be used while cloning).

6. Open the terminal and type the command below:
    > git clone (right click and Paste the copied link)
    ‘Press Enter’

7. You will now find a folder with the same name as the name of the repository, inside the folder you have created
    Change the directory in the terminal to get inside the folder by typing the below command:
    > cd {folder_name}
    ‘Press Enter’

8. Open any text editor where you have written your code and save it with any suitable name inside the same folder 
    (Note: The name of the folder will be the same as the name of the repository).

9. In the terminal, type ls and press enter, to check the list of files in the folder. 
    You will be able to find the new file in the list of files.

10. You now need to write the following commands to add, commit and push the file to the repository.
    > git add .
    ‘Press Enter’
    > git commit –m “Any suitable message”
    ‘Press Enter’
    > git push
    ‘Press Enter’

If you now open the repository in your browser and refresh, you will be able to find the newly added file there.


1: Create your first repository, then add and commit files:

    Once Git is installed, navigate to the directory you want to place under version control and create an empty Git repository:
        > git init
    This creates a hidden folder, .git, which contains the plumbing needed for Git to work. 

    Next, check what files Git will add to your new repository; this step is worth special care:
        > git status

    Review the resulting list of files; you can tell Git which of the files to place into version control 
    (avoid adding files with confidential information such as passwords, or files that just clutter the repo):
        > git add <file/directory name #1> <file/directory name #2> < ... >

    If all files in the list should be shared with everyone who has access to the repository, 
    a single command will add everything in your current directory and its subdirectories:
        > git add .
    This will "stage" all files to be added to version control, preparing them to be committed in your first commit.
    For files that you want never under version control, create and populate a file named .gitignore before running the add command.

    Commit all the files that have been added, along with a commit message:
        > git commit -m "Initial commit"
    This creates a new commit with the given message. A commit is like a save or snapshot of your entire project. 
    You can now push, or upload, it to a remote repository, and later you can jump back to it if necessary.
    If you omit the -m parameter, your default editor will open and you can edit and save the commit message there.

    Adding a remote
    To add a new remote, use the git remote add command on the terminal, in the directory your repository is stored at.
    The git remote add command takes two arguments:
        1. A remote name, for example, origin
        2. A remote URL, for example, https://<your-git-service-address>/user/repo.git
            > git remote add origin https://<your-git-service-address>/owner/repository.git
    NOTE: Before adding the remote you have to create the required repository in your git service, 
        You'll be able to push/pull commits after adding your remote.


2: Clone a repository

    The git clone command is used to copy an existing Git repository from a server to the local machine.
    For example, 
        To clone a GitHub project:
            > cd <path where you would like the clone to create a directory>
            > git clone https://github.com/username/projectname.git
        To clone a BitBucket project:
            > cd <path where you would like the clone to create a directory>
            > git clone https://yourusername@bitbucket.org/username/projectname.git
    This creates a directory called projectname on the local machine, containing all the files in the remote Git repository. 
    This includes source files for the project, as well as a .git sub-directory which contains the entire history and configuration for the project.

    To specify a different name of the directory, e.g. MyFolder:
        > git clone https://github.com/username/projectname.git MyFolder
    Or to clone in the current directory:
        > git clone https://github.com/username/projectname.git .
    Note:
        1. When cloning to a specified directory, the directory must be empty or non-existent.
        2. You can also use the ssh version of the command:
            > git clone git@github.com:username/projectname.git
    The https version and the ssh version are equivalent. 
    However, some hosting services such as GitHub recommend that you use https rather than ssh.

```
