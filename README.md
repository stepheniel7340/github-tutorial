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
**_In your [IDE]( http://ide.cs50.io/)_**  
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
6. In github and copy and paste git remote add origin `git@github.com:username/reponame.git`
7. Lastly, `git push -u origin master`



---
## Workflow & Commands



---
## Rolling Back Changes