# How to use Github 101
Here is a summary of commands for pushing, pulling, and branching after connecting your local machine to the website.


## Remote or clone
## Method no. 1
to clone or download the existing repository from git:
"`` git clone https://github.com/user_name/repository_name "``


## Method no. 2
1. To start git for a new folder:
''' git start '''
2. To access the existing repository from git:
"git remote add origin": https://github.com/user_name/repository_name ```


3. Check the access:
git remote -v '''


## Push
1. To add all changes (either files or new lines):
'''git add'''


2. to make modifications to a specific file:
``` git add "file_name.extension" ```


3. To create a new commit with title A and description B:
``` git commit -m "A" -m "B" ```


4. To push the changes to Github:
"git push origin main" or "git push origin master"


5. To set a default branch for future pushes, we can use "-u" just before "origin master":
"git push -u origin master"


-------------------------------------------------


## branching:
1. To check current branches:
git branch '''


2. to create a new branch named "feature-1":
"`` git checkout -b feature-1 "``


3. To switch to the "master" branch:
''' git master checkout ''' 
