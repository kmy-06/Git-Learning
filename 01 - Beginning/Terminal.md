## Version Control -> Working Folder

> pwd: print working directory (Display current path of the directory) [Output '/Users/...(foldername)' ]

> mkdir {+ an argument(new_folder_name)}: make directory (Create directory/New Folder with a given name) [No output] | Folder = Repository |

$$\text{Error when creating the same file twice -> mkdir: created-using-the-command-line: File exists}$$

> ls: list (Display all files in current directory)

> ls -A: list Flag All (Display all files including "." files which are hidden)

> cd {+ an argument(folder_name)}: change directory (Navigates to subdirectory under current directory)

> cd ..: navigates back to parent directory (yeah two dots)

<h6>$$\uparrow$$ 25 Feb</h6>

> A space is expected after command-line functions like mkdir & cd, etc. (It is called 'delimiter')

> Note that for mkdir {+ an argument(new_folder_name)}: Only two options -> 1) hyphens: file-name | 2) double quotes: "file name"

> Deleting files using command-line function usually bypasses the trash can (non-recoverable) | Better to delete files in Finder.

> export PS1='%1~ > ' : Use this command-line in terminal if you want every line to look like:

$$\text{Git-Learning} >$$

> The above terminal style shows the current directory (Git-Learning) with the '>' sign: export PS1='%1~ > '

> git init: Create Git repository (a .git hidden folder) [Output: below (ignore all the hints)] | Step 1 | Check using: ls -A

```
ch01_01 > git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint:
hint: 	git config --global init.defaultBranch <name>
hint:
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint:
hint: 	git branch -m <name>
Initialized empty Git repository in /Users/kongmoyu/Desktop/Head-First/Git-Learning/ch01_01/.git/
```
```
ch01_01 > ls -A
.git
```
> Give Git a few details about yourself, once and for all projects on your machine (in any directory) [No output] | Step 2 |:

```
ch01_01 > git config --global user.name "Private_Info_Surname Moyu"
ch01_01 > git config --global user.email "my.name@dhs.edu.sg"
```
> The above personal information in Git can be change anytime using the same commands.

> Basically, Git is all about: <b>Store Progress-Revisions To A Good Place When Working On A Project :)</b>

