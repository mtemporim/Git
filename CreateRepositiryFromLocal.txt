-- How to create a new repository from a local directory and sinchornizein with GitHub
 
-- Create a new folder that will be a branch main of repository 

(Git Bash in Windows)
mkdir /directory/NewRepository 
cd  /directory/NewRepository

(Windows cmd or PowerSheel)
mkdir c:/directory/NewRepository
cd  c:/directory/NewRepository

(Linux) 
mkdir c:/directory/NewRepository
cd  c:/directory/NewRepository

-- Create a REDME file 
echo "# NewRepository" >> README.md

-- Iniciate a nem repository in folder recently created
git init 

-- Add the files a staging area (in this case README.md)
git add . 

-- Create a initial commit 
git commit -m "Initial commit" 

-- Change the name "master" of branch to "main" 
git branch -M main

-- Create a repository "NewRepository" in Github without the option "Add a README file" on the web an get the URL


-- Link a local git repository directory to a remote repository
git remote add origim <URL>


-- Synchronize the local directory repository to a remote repository
git push -u origim main 
 
 