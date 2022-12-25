# how to use github

## Method no. 1
1. to clone / download the repository from git: 
``` git clone https://github.com/user_name/repository_name ```

2. to add all changes (either files or new lines): 
``` git add . ``` 

or to add changes for specific file: 
``` git add "file_name.extention" ```  

3. to add new commit with title A and description B: 
``` git commit -m "..." -m "...2" ```

4. to push the changes to Github: 
``` git push origin main or git push origin master ```


---------------------------

## Method no. 2
1. to start git for new folder: 
``` git init ```
2. to add all changes (either files or new lines): 
``` git add . ```
3. to add new commit with title A and description B: 
``` git commit -m "A" -m "B" ```
4. after making a new repository to connect it with VS: 
``` git remote add origin https://github.com/user_name/repository_name ```
5. to check the access: 
``` git remote -v ```
6. to set an defult branch for future pushes we can use  "-u" just before "origin master": 
``` git push -u origin master ```

-------------------------------------------------

## branch:
1. to check current branchs: 
``` git branch ```
2. to create a new branch as "feature-1": 
``` git checkout -b feature-1 ```
3. to switch to "master" branch: 
``` git checkout master ```