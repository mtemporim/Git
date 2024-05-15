[<-- Back to Git](https://github.com/mtemporim/Git-And-Github/tree/main/Git)


# Here is some inicials commands about Git.

## After intall Git there is some commands to run.  

>[!NOTE]
>
>These commands prepare your recently installed git to run in Windows


### On Git Bash - Set name and e-mail 

```bash
git config --global user.name "Your Name"
```
```bash
git config --global user.ema "Your E-mail"
```
[References](https://docs.github.com/en/get-started/getting-started-with-git/setting-your-username-in-git)


### On Visual Studio Code

If you want to make explicit the GIT command interpreter as default in VSCode, do the following procedure

Access the "**File**" menu 
--> "**Preferences**" 
--> "**Settings**"

Click "**Open Settings (JASON)**" in the upper right corner near "..." and add the following lines in the settings.json file:

```json
"terminal.integrated.defaultProfile.windows": "Git Bash",
"terminal.integrated.tabs.enabled": true,
```

When you click on the terminal, the "Git Bash" interpreter will open

>[!CAUTION]
>
>This action will replace your PowerShell shell interpreter with Git Bash - make sure you want to do this


## Follow some GIT commands 

**git init** - Initializes a new empty repository or reinitialize an existing one
Initialize empty
```bash
git init 
```
Reinitialize
```bash
git init (name of repositoty) 
```

**git clone** - Clone/copy an existing repository
```bash
git clone (url)
```

**git status** - Show information about staging area (Remember that the staging area is a place between the work area and the area that the repository is saved)
```bash
git status
```
**On branch main**     *--Local*  
**Your branch is up to date with 'origin/main'.**     *--It inform that occurred updates in branch main*  
**Changes not staged for commit:**     *--Info about update that not in staging area yeat*  
**(use "git add <file>..." to update what will be committed)**     *--Suggestion about what that can be made with git commands in case was a file added*  
**(use "git restore <file>..." to discard changes in working directory)**     *--Suggestion about what that can be made with git commands in case should discard updates*  
**modified:   directory1/file1.txt**     *--List of updates - Item 1 of list, the file file1.txt on directory1 was updated in this case*  
**Untracked files:**     *--List of items added in repository that was made but not add in staging area yeat*  
**(use "git add <file>..." to include in what will be committed)**     *--Info that suggest what should have make with this updates, that is, Should be added in the staging area*  
**directory1/test1.txt**     *--It show that was create a file called teste1.txt inside a directory called directory1*  
**test2.txt**     *--It show that was create a file called test2.txt in a branch main*  
**no changes added to commit (use "git add" and/or "git commit -a")**     *--It show that the added files not is prepared to commit yeat because not was runned git add command in these files, and sugest to run a git commit for files in exists in repository that was updated*  

**git add** - Add a file to the staging area
```bash
git add (name off file)
```
Add all update was made or something that was add in all work/index area 
```bash
git add .
```

git status "after git add" - In git status case above, after run "git add directory 1/test1.txt" and "git add test2.txt" or "git add ." , if run git status again will be show this way

**On branch main**     *--Local*  
**Your branch is up to date with 'origin/main'.**     *--It inform that occurred updates in main branch*  
**Changes to be committed:**     *--Info about update that should be committed*  
**(use "git restore --staged <file>..." to unstage)**     *--Suggestion about what that can be made with git commands in case should remove itens of staging area*  
**new file:   directory1/test1.txt**     *--It show info about what happened with this item, in this case create a new file insine a directory1 in branch main*  
**modified:   directory1/file1.txt**     *--It show info about what happened with this item, in this case was update the file1.txt inside directory1*  
**new file:   test2.txt**     *--It show info about what happened with this item, in this case create new file in branch main  


**git commit** - Get all the updates/adds that was in staging area to be versionaized and efectively insert this update in repository
```bash
git commit -m "Description of your commit"
```
If you remove "-m" option, you have to insert the commit description on your git bash or other command interpreter/IDE 
```bash
git commit
```

**git log** - Show informations about all the commits that was made in your repository 
```bash
git log
```
Example
**commit 9547a3rfc5kjh345gf47125f146c85a093ef8e4b (HEAD -> main, origin/main, origin/HEAD)**     *--Commit code and the place in repository where the commit occured*  
**Author: Author Name  <e-mail Author>**     *--Who made a commit and e-mail*  
**Date:   Thu May 11 15:47:06 2023 -0300**     *--Timestamp and UTC*  
**Create file.txt**     *--Title commit*  
**Creating a file with primary information with a link to the documentation and some infor**     *Description commit*  


**git push** - Send the commited operations to repository in internet 
```bash
git push origin main
```
**git branch** - It show all branchs in repository and what branch is 
```bash
git branch
```
Change the name "master" of branch to "main" 
```bash
git branch -M main
```
It create a new branch called NewBranch from main branch 
```bash
git branch NewBranch
```
**git remote** - Link a local git repository directory to a remote repository
```bash
git remote add origim <URL>
```
**git checkout** - It Access the new branch recently created 
```bash
git checkout NewBranch
```
