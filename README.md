# This is GIT basics

# GIT Commands

# it initialises a git repository, precisely creates a local .git file which is going to keep track of all changes
git init 

# below command add files to staging are based on file pattern has passed to it,  ( . ) represents all files and folders 
git add *.txt

# status command gives the information about changed file which is added to staging are and non tracked files for example if some files have been added to .gitignore file (e.g. *.log files ) then those will not be cached into the staging hence will be listed into non-tracked files in output of status command. 
git status

# if any specific file want to remove from staging (cached index), we can use below command to do so
git rm —cached file1.txt

# once we perform commit command then only it actually reflect into the branch
git commit -m ‘message’  

# to create a branch named login
git branch login

#switch to login branch
git checkout login

#add few files to newly created login branch and commit the same to it then we can merge login branch into master branch
git commit -m ‘login features added’

# here merge command will add new features into master branch from login, output of this command will list out all newly added files
git merge login

# this command checks if any remote origin has added to local git repository, if added already, output of this command will list out the same
git remote

# if any origin has not added then we can use below command to to do so, we can also add multiple remote origin 
git remote add   
git remote add origin https://github.com/kalikant/gitSample.git

# below command help to push all my local file to remote repository, pay attention to origin which are you pushing into incase you have multiple origans.
 
git push -u origin master

# subsequent push to remote repository
git push

# to download entire code base
git clone https://github.com/kalikant/gitSample.git

# git pull command helps to up to date your local repository with remote one.
git pull
