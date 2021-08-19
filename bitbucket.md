
1.	Install GIT
2.	Request for BITBUCKET repository access
3.	Check whether GIT Bash terminal is available in windows apps
4.	Configuration Steps:
Configuring your repository for first time: 

Enter the following commands on your Git Bash, when you configure your Git for the first time.

`git config --global user.name "User Name"` (Please provide your name here)

`git config --global user.email email_id` (Please provide your email id here)  

 git config – to configure the code from Remote repository to local repository

5.  Login to BITBUCKET and access the repository
6.	Search for your project repository  EX : REPO_NAME
 
## Cloning your Repository:

Cloning is nothing but creating a local copy of your Bitbucket folder structure. 
* Now, create a folder in your local machine
* Open the FOLDER where you want to clone repository -` Right click -> Git Bash here -> command prompt will open`
* Now run the below command to Clone the code in your folder.
    
    `git clone “your repository url” `

* Now cd to the folder, where repository is cloned.
Note: Developer creates Feature Branch and you can see your concerned repository under your project

## Creation of Feature Branch/Working branch:
* Create working feature branch for the team for each sprint/release

## Working procedure:

Developers are suppose to work from Feature Branch only , so create a Feature Branch from Bitbucket using below steps :

* Click on Create branch from options available next to master/main 
* Enter the branch name (ex: feature) -- choose branch from option.

## Git Pull:
* If Developer wants to get the latest changes from the Develop branch they can use pull command. 

`Note:` Since multiple developers are working on the same code, it is always best practice to run the pull command while adding the latest code to the local repository. 
* It avoids the merge code conflicts.
* To pull code from Remote repository to local repository, you can use “git pull” command. 

* `git pull` OR `git pull origin branch_name` 

`Note:` When you run the pull command, it will fetch the default branch code.

* git checkout – to switch from one branch to another branch (EX: master to feature)
 
* make changes in your code/scripts

* Check the status of the files
    Red colour indicates the files are in Untracked stage.

* `git add .` --- This command will add all the files to your local repository

* `git add filename` - This command will add the filename(only one file) you mentioned/added to your local repository
To check the status again whether the files are in tracked stage or not, please run git status command.
Green color indicates the files are in Tracked stage

* `git commit –m “Description”` – This would commit the files that you have added to your local repository

* `git push origin branch_name`   - This command will push your files to your Bitbucket server.

Finally, the code will be pushed to the Bitbucket repository successfully. You can refresh the Bitbucket page to see the latest code that is pushed.

## Pull Request creation:

Pull request is a mechanism for a developer to notify team members/leads that they have completed a feature. Once their feature branch is ready, the developer files a pull request via their Bitbucket server.
* If we want to merge the code from Feature Branch to Develop Branch, create a Pull request

`NOTE:` For creating a pull request, Developer must need to commit the changes to the local repository.

* Click on Create Pull request option 

* Select branch to be merged ( From(Current branch) – To(Target branch) )
 
* Click on Continue to Add Reviewer name to review the code before merge 
 
* Click on Create and It will trigger an automatic mail to  the reviewer
 
* The reviewer has to click on merge button to approve the pull request

* After merging, reciepient will receive below email


## Merge conflicts:

* Merge conflict issue will arise only when Developer creates pull request.
* When Developers are facing the Merge Conflicts, below steps to be followed to get the issue resolved.

## Commands Summary:
* `git checkout branch_name`
* `git pull`
* `git status`
* `git add .`
* `git commit –m “give description”`
* `git push`
