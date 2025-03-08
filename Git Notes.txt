
Git :	is a version control system that helps developers track changes to their code. Its type of distributed version control system( Every person has its own full copy of project).
GitHub :	is a cloud-based hosting service that allows developers to manage Git repositories.

We can work on Git through Command Line Interface using Terminal.
***Add tab to auto name
This Terminal is same as linux terminal and commands are also same as linux commands. Some of the commands are as below:

1. pwd ( present working directory) it shows present path at which terminal is working.
2. cd ( change directory) it changes the path like cd folder/ -> it will change path to c drive.
3. ls (list content) will list all content from that folder.
4. q (quite)

git config --global user.email 'email' -> this command will save user email id. To see command git config --global user.email. We can also add name.


Three stage architecture:
							Working directory -> staging area -> git directory(repositories)
To add repositories:

step 1 : (git status) *** WE HAVE TO CHECK THIS IN EVERY PROCESS ***-  it will let you know the status of current work.

step 2 : staging process - to add all files (git add --a)

step 3 : commit process - to commit the repositories (git commit -m "Initial Commit") If we write only git commit it will open the editor, instead we prrinted a message in double quote.

step 4 : we can check the history by (git log) (git log -p -> to see commit log with comparision)

step 5 : if we change or update any of file, we can stage and commit that specific file by (git add filename.txt) and then commit with its descriptive message.

If we have to remove or delete git for that repositories (rm -rf .git)

If have to clone any repositories from website (git clone website.git)

File Status Lifecycle : 
						Untracked - before starting the process
						unmodified - version 1 files are staged
						modified - if any change/update done i.e version 2 
						staged - version 2 changes staged

To create a file using terminal (touch error.log)

.gitignore command : Suppose ther are some file(e.g. log file) which we don't have to load in github. So, we use this command to ignore the unwanted file.
						we create a file i.e ( touch .gitignore)
						In that file add unwanted file(with extension) and then stage and commit.  ( if there are multi log files you have to ignore you can write *.log in .gitignore file.)

git diff command : It compares the change of file/folder from working directory and staging area

git diff --staged command : it compares changes of previous commit and currently staged area

Skipping staging area :git commit -a -m "Direct commit"

To remove file from terminal : git rm filename.ext

To rename file from terminal : git mv filename.ext newfilename.txt

To untracked files, you will have to include that file into .gitignore an run below command
				git rm --cached filename.ext
				
To unstaged the file, you can (git restore --staged filename

To unmodify the change to previous version (git checkout -- filename.ext)

To push the repositories on github :
git push -u origin develop


To make shortcut of commands, we make alias of it. ( git config --global alias.shortcutWord 'command'
In Our lappy below are shortcut keys:
(git s) status		(git l) log 	(git c) commit 	(git aa) add --aa		(git a) add

Creating branches: (git checkout -b branchname)
switching branches: (git checkout branchname)
To check available branches : git branch

To merge branches : git merge brachname
To check mergerd branches : git branch --merged
To check branches which is not merged : git branch --no-merged

To delete branch : git branch -d branchname

Two types of branches : long run branches and topic branches.