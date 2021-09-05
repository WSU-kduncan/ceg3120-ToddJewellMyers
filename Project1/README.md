1. # My Project 1


## Setup

To initialize a repo within your AWS instance home directory, we use the command git init --bare then name. In this case I used git init --bare repo.git to create the repo. 

To add a user we type the command sudo adduser nameofuser 

to change permission to root we use the sudo su command. to change file permissions we use the chmod command followed by whatevr filename you want changed r is for read w is for write and x is for execute.
each file has permissions for a suer group and other allowing them to read write or execute the file.

to make a ssh key for our user we could sudo su nameofuser make a directory called .ssh by doing the command mkdir .ssh then we go to the AWS the .ssh file in authroized_keys and get our public key we go back to the user i named git and we cd .ssh vim authorized_keys and paste the public key in.


## Usage 

To use get clone we within are WSL 2 terminal tab use the command git clone --verbose ubuntu@18.233.173.239:gitServer.git to make this work I had to go to the .ssh directory open up the ssh key and copy to then paste within the AWS instance we go into the .ssh in AWS them vim authorized_keys and we paste the key within this this allows the clone for our gitServer.git

we use init to create Repositories. 

we use git add to tell Git to include these certain desired changes to a certian file for the next commit.

we use git commit to submit and record those changes to the local repository.

then we use git push to actually push the previosuly mentioned commands the git add which has the desired changes we want git commit which records them to the local repository adn then we are ready for git push which takes it from the local repository and uploads it onto the remote repository.

# Images

(gitServer1.png)

(gitServer2.png)
