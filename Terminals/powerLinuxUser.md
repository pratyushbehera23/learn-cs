# Linux_

Linux kernel opensource, so many communities have created their own version called as linux distributions(distros) and made to fit specialized need like personal, server, phones,..

## Linux distros

- Ubuntu
- Debian
- Alpine
- Fedora
- CentOS

## File system

Files and directories are organized in a tree hierarchical structure like windows.

### Windows FS

Drives

- (C-Drive) -> C:\Users\Pratyush\Desktop\ ..
- (D-Drive) -> D:\foldername\ ..
- ..

### Linux FS

- / - root directory
  - bin - binaries/programs
  - boot - booting files
  - dev - devices accessing files
  - etc - configuration files (editable text configuration)
  - home - home directories for users
  - root - home directory of the root user
  - lib - library files like software library dependencies
  - var - variables (frequently updated files like log files, app data, ..)
  - proc - files that represent running processess

> In linux everything is a file directories, processess, devices, network sockets, pipes ..

## Commands

Most of these distributions support same set of commands but few different too.

Shell commands
bin - folder
bash - a program (bash is short for born again shell) - enhanced version of original shell program

In linux we use a forward slash (/) to separate files & directories but in windows we use a backslash (\)
Linux is a case-sensitive OS.

echo -
echo $0 -
whoami -
history -
!{any-number-from-history}  eg. !2  -  runs the second command from history

Package managers: (like npm, yarn, pip, NuGet) -
apt (advanced package tool) -
apt-get  -  older package manager
apt list -
apt update -
apt install nano -
apt remove nano -

nano    -  

pwd    -  
ls    -  
ls -1   -  
ls -l   -  
cd   -  
