# Bash

```sh
To display the Bash help (manual) page for the specified built-in.
    > help <command>

To see a list of all built-ins with a short description, use
    > help -d

Commands:

ls - 
    The ls command's -l option prints a specified directory's contents in a long listing format. 
    If no directory is specified then, by default, the contents of the current directory are listed.
        > ls -l
    Using a long listing format (-l) and sorted by time (-t).
        > ls -lt
    The -a or --all option will list all files, including dotfiles.
        > ls -a
    The -A or --almost-all option will list all files, including dotfiles, but does not list implied (.) and (..) 
    Note that (.) is the current directory and (..) is the parent directory.
        > ls -A

tree - 
    The tree command lists the contents of a specified directory in a tree-like format. 
    If no directory is specified then, by default, the contents of the current directory are listed.

mkdir - make directory

cd - change directory
    The default directory is the home directory ($HOME, typically /home/username), 
    so cd without any directory takes you there
        > cd
    Or you could be more explicit:
        > cd $HOME
    A shortcut for the home directory is ~, so that could be used as well.
        > cd ~

nano - 

cat - concatenate files

grep - 

echo - 
    > echo "Hello World"
    echo is a Bash builtin command that writes the arguments it receives to the standard output. 
    It appends a newline to the output, by default.

touch - Create a new file
    > touch hello-world.sh
    Make the script executable by running chmod +x hello-world.sh

read - 
    The command 'read' reads one line of data from standard input into the variableName. 
    This is then referenced using $variableName and printed to standard out using echo.

gzip - files are compressed by gzip
```
