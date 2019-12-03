# GitHub Tutorial

_by Stephenie Lin_

---
## Git vs. GitHub
**Git**: A tool using command lines to keep track of code or changes over time, it does not require Github    
**Github**: A website used to store Git, allows users to share and collaborate, it requires Git  


---
## Initial Setup  
**_Github sign-up_** 
1. Go to [github.com](https://github.com/)
2. Click "Sign Up" on the top right corner   
3. Enter Username, Email address, and password   
4. Verify your account
5. Select your plan free or $7 per month
6. Do the survey and "submit"
_That's it!_ 

**_Next, set up an SSH key_**  
Follow the directions in this [link](https://github.com/hstatsep/ide50)  

**_Why do we need an SSH key?_**  
SSH key is used to access your account. We need it because rather than signing in multiple times to enter our account we only have to sign in once. An SSH key is also used to link your local repo to remote repo.        

---
## Repository Setup
### **_In your [IDE]( http://ide.cs50.io/)_**  
**Enter the following in your terminal** 
1. `cd into the directory` (ex. `cd github-learning`)
2. `git init`
3. Add or edit stuff on your file
4. `git add .`
5. `git commit -m “message”` (ex. `git commit -m “change cat to dog”`)

**_On [Github](https://github.com/)_**
1. Click “new repository” on top right corner
2. Create a name for your repo
3. Click “create repository”
4. Make sure it’s on SSH

**_Back in your [IDE]( http://ide.cs50.io/)_**
1. Make a folder and name it the same as your repo name (ex. `mkdir folder`)
2. `cd folder`, and create a `README.md file` (`touch README.md`)
3. `git init` to the folder
4. `git add .`
5. `git commit -m "message"`
6. In github, copy and paste git remote add origin `git@github.com:username/reponame.git`
7. Lastly, `git push -u origin master`



---
## Workflow & Commands
`git status`: checks which file/files are added on stage and ready to be committed  
`git add .`: adds all files to staging area     
`git commit -m "message"`: takes a "snapshot" of file on the staging area, or commits file to staging area    
`git push`: pushes or sends commits to Github from cloud (IDE)  


---
## Rolling Back Changes
#### Mistakes can be undone with these steps  
**Undo edits:** Enter `git checkout "filename"`  
**Undo adds:** Enter `git reset HEAD "filename"`   
**Undo commits:** Enter `git reset --soft HEAD~1`   
**Undo push:** Enter `git log`, copy the SHA, lastly type `git revert "SHA"`   

--- 
## Error Handling 
* If you `git init` in the wrong directory use `rm -rf .git`  

Remove a repository on local      
1. go to IDE  
2. type `rm -rf`   

Remove a repository on remote   
1. go to Github   
2. click on the repository you want to remove
3. click on "settings"
4. click on "danger zone"
5. click on "delete this repository"
6. Type in name of repository to confirm
7. click "I understand the consquences, delete this repository".