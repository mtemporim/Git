[<-- Back to Git](https://github.com/mtemporim/Git-And-Github/tree/main/Git)  

# How to create a new repository from a local directory and sinchornize with GitHub  

### Create a new folder in local machine that will be a branch main of repository  

Git Bash in Windows  
```bash
mkdir /directory/NewRepository
```
```bash
cd  /directory/NewRepository
```
Windows cmd or PowerSheel  
```bash
mkdir c:/directory/NewRepository
```
```bash
cd  c:/directory/NewRepository
```
Linux
```bash
mkdir c:/directory/NewRepository
```
```bash
cd  c:/directory/NewRepository
```

Create a REDME file 
```bash
echo "# NewRepository" >> README.md
```

### Iniciate a nem repository in folder recently created
```bash
git init 
```
Add the files a staging area (in this case README.md)
```bash
git add . 
```
Create a initial commit 
```bash
git commit -m "Initial commit" 
```
Change the name "master" of branch to "main" 
```bash
git branch -M main
```

### Create a repository "NewRepository" in Github without the option "Add a README file" on the web an get the URL

Link a local git repository directory to a remote repository
```bash
git remote add origim <URL>
```

Synchronize the local directory repository to a remote repository
```bash
git push -u origim main 
``` 
 