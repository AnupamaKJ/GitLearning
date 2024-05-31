- Sample files to follow along: https://1drv.ms/u/s!AmxrofZZlZ-whOIll...
 - Official Git web site: https://www.git-scm.com/ 
- Official GitHub.com web site: https://github.com/ 
- Git and GitHub.com cheat sheet: https://education.github.com/git-chea...  
- Git Reference Manual: http://git-scm.com/docs 
- Git Overview Book: http://git-scm.com/book/en/v2 
- Sample ignore files: https://github.com/github/gitignore 
- Hyper.is Terminal: https://hyper.is/

Git
Git is open source and free source control management (SCM)
https://onedrive.live.com/?authkey=%21AJdw967%5FoljMamM&id=B09F9559F6A16B6C%2178117&cid=B09F9559F6A16B6C
Commands
1)	To Set user name (We will come to know who made the changes)
Git config --global user.name “AnupamaKJ”
2)	To set email ID
Git config –global user.email kjanupama2009@gmail.com
3)	To set the branch
Git config –global init.default branch main
4)	Help
5)	Git config –h
6)	git help config

$ git help
usage: git [--version] [--help] [-C <path>] [-c name=value]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
•	clone  -->  Clone a repository into a new directory  
•	init -->  Create an empty Git repository or reinitialize an existing one  

work on the current change (see also: git help everyday)  
•	add -->  Add file contents to the index  
•	mv -->  Move or rename a file, a directory, or a symlink  
•	reset -->  Reset current HEAD to the specified state  
•	rm -->  Remove files from the working tree and from the index  

examine the history and state (see also: git help revisions  
•	bisect -->  Use binary search to find the commit that introduced a bug  
•	grep -->  Print lines matching a pattern  
•	log  -->   Show commit logs  
•	show -->  Show various types of objects  
•	status -->  Show the working tree status  

grow, mark and tweak your common history  
•	branch -->  List, create, or delete branches  
•	checkout -->  Switch branches or restore working tree files  
•	commit --> Record changes to the repository  
•	diff -->  Show changes between commits, commit and working tree, etc 
•	merge -->  Join two or more development histories together  
•	rebase -->  Reapply commits on top of another base tip  
•	tag -->  Create, list, delete or verify a tag object signed with GPG  

collaborate (see also: git help workflows)  
   fetch --> Download objects and refs from another repository  
   pull --> Fetch from and integrate with another repository or a local branch  
   push --> Update remote refs along with associated objects  

'git help -a' and 'git help -g' list available subcommands and some concept guides. See 'git help <command>' or 'git help <concept>'
1.	to read about a specific subcommand or concept.

### Commands ###
-->  Clear  
--> Git init (to initialize the repository)
.git folder will be generated, need to select “show hidden items” options on right click

--> .git folder contains all necessary repository files
--> Git status  -- Status of our repository
--> Git  add <file name> -- Ex: git add initial.htm
--> use "git rm --cached <file>..." to unstage  
git rm –cached <initial.htm>

### Create a .gitignore file ###
--> It will igore the files for adding repository  
--> # ignore all .txt files  
    *.txt  
--> On running git status, it will ignore files with .txt files

### Add Files ###
--> git add --all  
--> git add -A  
--> git add . (to add all)

### To commit the code ###
 git commit -m "first commit - commiting all files to the repository"
 git commit -a -m "my second commit"

 ### To get difference in the code ###
 git diff

 press q --> for quitting

 ### Three types of working Env ###
 1. Working files --> where we can make and edit files
 2. Staging --> holding pen until u are ready to add it to the history books
 3. commits --> Are where you can commit things and this is added as a log or an entry into the history books

 ### To remove the file from the stating ###
 git restore --staged(file name)  
Ex: git restore --staged index.htm

### To remove file from the folder ###
git rm (file name)  
ex: git rm "secret recipe.htm"

### to rename the file ###
git mv (Existing file name) (new name)
Ex: git mv "KCC Logo.png" "Primary LOGO.png"

### to list out all comments ###
git log --> detailed comments 
git log --oneline --> all comments in one line  

--> to update the command  
git commit -m (new command) --amend  

git commit -m "Changed file name to Primary LOGO.png" --amend

git help log (opens up the manual)

git log -p

git reset 

git rebase -i --root


####  Branch ####
--> git branch FixTemp -- To Create new branch  
--> git branch -- To check the number of branches  and active branch with * mark   
--> git switch (branch name) -- To switching other branch   
--> git switch -c (new branch name)  --> it will create new branch with "C"  
ex: git switch -c (UpdateText)


####  Merge the code to the main branch ####
--> git merge -m (Message) (From which branch need to copy)  
ex: git merge -m "Merge fixtemp back to main" FixTemp

#### To delete the branch ####
--> git branch -d (Branch name which needs to delete)
ex: git branch -d FixTemp










