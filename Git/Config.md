[<-- Back to Git](https://github.com/mtemporim/Git-And-Github/tree/main/Git)  

### Some information about git config options


**git config** - Show options of git config commands  
 
 
 I write a fews words about 3 main option  
 **--global**  Contain the configuration of all user  
 **--system**  Contain the configuration of Git system  
 **--local**   Contain the configuration of specific repository   
 

 Add user and e-mail for all user 
```bash
git config --global user.name "Your Name"
```
```bash
git config --global user.email "Your E-mail"
```
To show user.name and  user.email
```bash
git config --global user.name 
```
```bash
git config --global user.email 
```
Show name of default branch
```bash
git config init.defaultBranch 
```
Change name of default branch
```bash
git config --global init.defaultBranch main
```
Show all configurations 
```bash
git config --global --list 
```
Store permanently a credential token in local machine
```bash
git config --global credential.helper store 
```
Store temporarily a credential token in local machine
```bash
git config --global credential.helper cache 
```
Show type of store type of credential 
```bash
git config --global  credential.helper 
```
Show directory where is the store file configuration 
```bash
git config --global --show-origin  credential.helper
```