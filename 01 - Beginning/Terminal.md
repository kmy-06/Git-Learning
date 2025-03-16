## Version Control -> Create Working Folder With Git

> pwd: print working directory (Display current path of the directory) [Output '/Users/...(foldername)' ]

> mkdir <argument(new_folder_name)>: make directory / create a new project folder [No output] | Folder = Repository | Step_1 |

$$\text{Error when creating the same file twice -> mkdir: created-using-the-command-line: File exists}$$

> ls: list (Display all files in current directory)

> ls -A: list Flag All (Display all files including "." files which are hidden: `shift`+ `cmd` + `.`)

> cd <argument(folder_name)>: change directory (Navigates to subdirectory under current directory) 

> cd ..: navigates back to parent directory (yeah two dots)

<h6>$$\uparrow$$ 25 Feb 2025</h6>

> A space is expected after command-line functions like mkdir & cd, etc. (It is called 'delimiter')

> Note that for mkdir <argument(new_folder_name)>: Only two options -> 1) hyphens: file-name | 2) double quotes: "file name"

> Deleting files using command-line function usually bypasses the trash can (non-recoverable) | Better to delete files in Finder.

> export PS1='%1~ > ' : Use this command-line in terminal if you want every line to look like:

$$\text{Git-Learning} >$$

> The above terminal style shows the current directory (Git-Learning) with the '>' sign: export PS1='%1~ > ' ((temporarily))

> git init: initialize a Git repository within THAT folder (a .git hidden folder) [Output: below (ignore all the hints)] | Step_2 | Check using: ls -A

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
Initialized empty Git repository in /Users/moyu/Desktop/Head-First/Git-Learning/ch01_01/.git/
```
```
ch01_01 > ls -A
.git
```
> Give Git a few details about yourself, once and for all projects on your machine (in any directory) [No output] | Just_Do_It |:

```
ch01_01 > git config --global user.name "Private_Info_Surname Moyu"
ch01_01 > git config --global user.email "my.name@dhs.edu.sg"
```
> The above personal information in Git can be change anytime using the same commands.

> Basically, Git is all about: <b>Store Progress-Revisions To A Good Place When Working On A Project :)</b>

<h6>$$\uparrow$$ 27 Feb 2025</h6>

> For permanent change to:

$$\text{Current Directory} >$$

> Restart terminal and type `nano ~/.zshrc` and Enter. Then, if you are in Pico (not Nano) - Pine Integrated Composer: A text editor that runs inside your terminal, Change your prompt to: `PROMPT='%1~ > '`. Press Enter to save and quit Pico with `control + x`.

> git add <filename>: Add the file (e.g checklist.md) to git.

> git commit -m "My first commit": Commit with a message to provide a meaningful reminder as to why you made this change. (The -m is called a flag, it stands for message) [Output: below (Looks fine)]

```
HawtDawg > git commit -m "My first commit"
[master (root-commit) 0596350] My first commit
 1 file changed, 5 insertions(+)
 create mode 100644 Checklist.md
```

> When you commit, A commit object is created (e.g 0596350). It stores all your changes and info in binary format, which is very hard for humans to read but super safe and efficient for Git :)

> There are two parts for Git's Working Directory:
> 1) The 'Index' staging area, house temporary changes.
> 2) The Git's memory bank (.git) stores contents in the object database.

<h6>$$\uparrow$$ 2 Mar 2025</h6>

> Multiple states of files in a Git repository.




