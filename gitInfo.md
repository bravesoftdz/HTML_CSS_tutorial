# Git
# 2.1 Initializing a Repository

- for initialising a directory you have to cd your way to the
  desired working directory and use the command "git init" 
  or "git init "path" ".

- to make instructions not return anything to the console you
can use the -q flag (it stands for quiet).

# 2.2 The Staging Area and Status Command

- for creating a README file you should use "vim README" 
command.
- for closing the readme editor you should do "esc + :wq"
- "git status" tells you about overall status of the files 
which are in the working directory.
- for adding a new file in the working directory (making it 
tracked) you should use " git add "path" "

# 2.3 Making Commits

- git commit -m "description" - the instruction for git commit
 if you want to commit and add files at the same time you can 
 use the flag -am (only if the files are tracked).
- if you want to ammend a commit (you forgot a point for 
example) you can use "git commit -a --amend" (it 
condenses the previous commit and the current one into one)
- shows the list of git commits you can use "git log" 
for closing a huge list you can use :q 

# 2.4 Ignoring Files

- for requesting for the git console to exclude some files 
when adding and commiting you should make an .gitignore file.
- for adding comments you can use # simbol
- in the gitignore you can add the name of all files and 
folders you want git to ignore (it is always useful to 
categorize them by using comments)
- if you want to ignore files globally you have to write 
the files in the gitignore_global.txt file in the GitProjects
folder.

# 2.5 Viewing the Log

- git log unit parts (all commits are shown in reverse chrono 
  order):
  - the full commit hash
  - author
  - date
  - commit message
- for getting a shorter version of the log use the flag 
  --oneline
- for showing a certain number of commits in the past on
  the log you should use the flag -noOfCommits
- for more information about the commits you use the -p tag
  - the -p tag shows a bit of the diff (patch)
- for general information about the diff without much info 
  about the patch you can use the flag --stat 
- "--pretty=" is also another flag that can be used to 
  visualise logs. The options after pretty can be:
  - oneline - diference: full hash
  - short
  - full
  - fuller
  - format:"..." - creates a custom format for the information
    you have specific tags for each info (begins always with 
    %) and text specifics (ex. you can change the color and 
    reset it by calling %Cblue ... %Creset)
- for more info you can use "git log --help"
- git log -- graph shows a graph of all commits to different 
  branches.

# 3.1 Creating Branches

- git branch new-branch - creates a new branch. new-branch 
  represents
- git branch -d new-branch - deletes the specified branch 
(if you wanna force delete a branch you should use the -D 
flag instead).
- git branch -a - shows all branches and highlights the 
  current one.
- git checkout new-branch - for checking out a new branch
- git checkout -b new-branch - for creating and 
  checking out a new branch

# 3.2 Fetching and Pulling

- git pull . master (if it is a local reppo you use . else 
  you have to use the name of the remote reppo) - instruction
  for pulling changes from master branch (basically the 
  commits from the master branch merge with the commits 
  of the current branch and are being saved in the current 
  branch)
- git fetch . master - practically like pull but without 
merging the commits (just going halfwaym, or getting 
them ready)

# 3.3 Diffing Files

- diffing - compare files and view the changes between them.
- git diff branch1 branch2 - compares branch1 with branch2
- git diff FETCH_HEAD - compares the current branch with 
  what was fetched.
- git diff branch1 branch2 --name-only - it tells the names 
  of the files that are different.
- git diff branch1 branch2 --stat - more info version of the 
  above.  
  
# 3.4 Merging Branches

- merge - take some content from one branch and merge it into a 
  different branch.
- git merge branch - by branch it is inferred the branch you 
  want to merge with the current branch you are in.

# 3.5 Tags

- git tag - shows all the tags the current project has.
- if you want to add a new tag to the current commit you 
  have to write git tag tagName.
- for getting information about a tag you can use git show 
  tagName.

#4 Notes

- for adding a site as a project (if you wanna host it 
on github) you have to use username.github.io as the name 
of the project and you can visit it by writing the name as 
an address.
- for adding a website to a project you should make a branch
which is named gh-pages. You can save everything related to 
your site in there.
- search github pages for more info about how to make sites 
hosted on github.