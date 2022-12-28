# How to use Github 101
Here is a summary of commands for pushing, pulling, and branching after connecting your local machine to Github.


## Clone
Clone the remote version on Github and make a local copy.

**Method I - Clone:**

Clone or download the existing repository from git:

``` git clone https://github.com/user_name/repository_name ```

**Method II - Remote:**

1. Start git for a new folder:
``` git start ```

2. Access the existing repository from Github:

``` git remote add origin https://github.com/user_name/repository_name ```

3. Check the access:
``` git remote -v ```


## Push
After all the modifications, push will update the remote version:

1. Add all changes (either files or new lines):
```git add```

2. Make modifications to a specific file:
``` git add "file_name.extension ```

3. Create a new commit with title "A" and description "B":
``` git commit -m A -m B ```

   or, use the shortcut, instead of steps 2&3, add all modifed files and commit at the same time: ``` git commit -am A -m B ```
   (this canbe used in cases of file modification and not file creation)


4. Push the changes to the "branch_name_example":
``` git push origin branch_name_example ```

5. To set a default branch for future pushes, we can use "-u" just before "origin":
``` git push -u origin branch_name_example ```

   After this, by simply writing  ``` git push ``` changes will be pushed to Github.



## Branching, merging, and pulling:
Branches are needed to create and modify new features while protecting the main version. 
Merging and pulling are used to sync up two different branches.

1. To check all local branches:
``` git branch ```

2. To create a new branch named "branch_name_example":
``` git checkout -b branch_name_example ```

3. switch to, for example, the "master" branch:
``` git checkout master ``` 

4. Check the current branch and the "branch_name_example" and show the changes that have been made:
``` git diff "branch_name_example" ```

   (If there are confilicts between two versions then:
   press **q** to quit and you can address those confilits by merging)

5. To update your side branch by master/main branch use ``` git merge master ``` or ``` git merge "branch_name" ```, and after the local merge, pull, commit, and push to update the remote version.

6. Pull a branch or to merge with a remote branch:  
``` git pull origin "branch_name_example" ```

7. Delete a local branch:  
``` git branch -D "branch_name_example" ```
   & to delete a branch on Github use the platform.

## Forking:
To create an editable legal copy of any third-party code and add it to your repository.


## Using Pandoc for Github's markdown conversion

``` pandoc -s example.html --to=gfm -o README.md ```
