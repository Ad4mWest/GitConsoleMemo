# Working with the console

## Useful features
• *Commands do not need to be printed and executed in turn. You can specify them in a list - split by two ampersands `&&`;*
• _The console has its own memory buffer with the last few commands. You can navigate through them using the arrow keys `up() & down()`;_
• *To avoid entering the full name of a file or folder, you can type the first characters of the name and press **Tab** twice. If the file or folder is in the current directory, the command line will add the path itself;*
• _For example, you are in the **dev** folder. Start typing `cd first` double-click **Tab**. If the **first-project** folder is inside **dev**, the command line will automatically substitute its name. All that remains is to press **Enter**;_

## Navigation
• `pwd` (from the English print working directory, "show working folder") - show me which folder I'm in;
• `ls` (from the English list directory contents, "display directory contents") - show files and folders in the current folder;
• `ls -a` - show also hidden files and folders, the name of which begins with the symbol `**.**`;
• `cd first-project` (from the English change directory, "change directory") - go to the folder **first-project**;
• `cd first-project/html` - go to the **html** folder, which is located in the **first-project folder**;
• `cd` - go to a higher level, to the parent folder;
• `cd ~` - go to the home directory **(/Users /Username)**;
• `cd /` - go to the root directory.

## Working with files and folders

### Creation
• `touch index.html` (English touch, "touch") - create a file **index.html ** in the current folder;
• `touch index.html style.css script.js` - if you need to create several files at once, you can print their names in one line separated by a space;
• `mkdir second-project` (from the English make directory, "create a directory") create a folder named **second-project** in the current folder.

### Copying and moving
• `cp file.txt ~/my-dir` (from the English soru, "copy") - copy the file to another location;
• `mv file.txt ~/my-dir` (from the English move, "move") - move a file or folder to another location.

### Reading
• `cat file.txt` (from the English concatenate and print, "combine and print") - print the contents of a text file **file.txt .**

### Deleting
• `rm about.html` (from the English remove, "delete") - delete the file **about.html**;
• `rmdir images` (from the English remove directory, "delete directory") - delete the folder **images**;
• `rm -r second-project` (from English remove, "delete" + recursive, "recursive") - delete the folder **second-project** and everything it contains.

# Getting started with Git

## Initializing the repository
• `git init` (from the English initialize, "initialize") — initialize the repository.

## Synchronization of local and remote repositories
• `git remote add origin` https://github.com/YandexPracticum/first-project.git (from English remote, "remote" + add, "add") — link the local repository to the remote one with **URL** https://github.com/YandexPracticum/first-project .git ;
• `git remote -v` (from the English verbose, "detailed") — check that the repositories are really connected;
• `git push -u origin main` (from the English push, "push") — for the first time, upload all commits from the local repository to the remote one with the name origin.
• Your branch can be called master, not main. Tweak the command if necessary.
• `git push` (from English push, "push") — upload commits to a remote repository after it has been linked using the `-u` flag.

## Preparing the file for commit
• `git add todo.txt` (from the English add, "add") — prepare the file **todo.txt** to commit;
• `git add --all` (from the English add, "add" + all, "all") — prepare for the commit immediately all files in which there were changes, and all new files;
• `git add.` — prepare the current folder and all files in it for commit.

## Creating and publishing a commit
• `git commit -m "Comment to commit."` (from the English commit, "commit", commit" + message, "message") — make a commit and leave a comment to make it easier to understand what changes have been made;
• `git push` (from English push, "push") — add changes to the remote repository.

## View commit information
• `git log` (from the English log, "log [records]") — output a detailed commit history;
• `git log --oneline` (from the English log, "log [records]" + oneline, "one line") — show brief information about commits: an abbreviated hash and a message.

## View file status
• `git status` (from English status, "status", "status") — show the current state of the repository.

## Adding changes to the last commit
• `git commit --amend --no-edit` (from English amend, "fix") — add changes to the last commit and leave the message the same;
• `git commit --amend -m "New message"` — change the message to the last commit to a new message.
• Exit the editor **Vim:** press **Esc**, enter `:qa!`, press **Enter**.

## "Rollback" of files and commits
• `git restore --staged hello.txt` (from the English restore, "restore") — translate the file **hello.txt** from the **staged** state back to **untracked** or **modified**;
• `git restore hello.txt` — return the file **hello.txt** to the latest version that was saved via **git commit or git add**;
• `git reset --hard b576d89` (from the English reset, "reset", "reset" + hard, "harsh") — delete all uncomplicated changes from staging and the "work zone" up to the specified commit.

## View changes
• `git diff` (from the English difference, "difference", "difference") — show the changes in the "work zone", that is, in **modified** files;
• `git diff a9928ab 11bada1` — output the difference between two commits;
• `git diff --staged` — show the changes that are added to the **staged** files.

# Markdown cheat sheet

## Text Selection
You can highlight text in markdown using the characters `_` or `*`. For example:
Example of _cursive_ and **bold** text.

## Headings
Headers can be created using the `#` symbol. The larger the `#`, the smaller the header. For example:

# First level header
## Second level header
### Third level header

## Code Selection
To highlight the text as code, put it in triple quotes ```.

```
mkdir my_project
cd my_project
git init
```
These are just some of the features of markdown. Other you can find there: 
- https://gist.github.com/fomvasss/8dd8cd7f88c67a4e3727f9d39224a84c
- https://www.markdownguide.org/cheat-sheet/

