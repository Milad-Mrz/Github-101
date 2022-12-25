# How to use Github 101
Here is a summary of commands for pushing, pulling, and branching after connecting your local machine to the website.


## Clone or remote 
**Method I:**

Clone or download the existing repository from git:

``` git clone https://github.com/user_name/repository_name ```

**Method II:**
1. Start git for a new folder:
``` git start ```

2. Access the existing repository from git:

``` git remote add origin https://github.com/user_name/repository_name ```

3. Check the access:
``` git remote -v ```


## Push
1. Add all changes (either files or new lines):
```git add```

2. Make modifications to a specific file:
``` git add "file_name.extension ```

3. Create a new commit with title "A" and description "B":
``` git commit -m A -m B ```

or in short instead step 2 & 3 to add and commit at the same time: (only in case of file modification not creation)

``` git commit -am A -m B ```


4. Push the changes to the "branch_name":
``` git push origin branch_name ```

5. To set a default branch for future pushes, we can use "-u" just before "origin":
``` git push -u origin branch_name ```

after this by simply writting  ``` git push ``` changes will be pushed to Github



## Branching, merging and pulling:
1. To check all branches:
``` git branch ```

2. To create a new branch named "A":
``` git checkout -b A ```

3. switch to for example the "master" branch:
``` git checkout master ``` 

4. Check current code to the "branch_name" and show changes that have been made:
``` git diff "branch_name" ```

(If there are confilicts between two versions then:
press **q** to quit and you can address those confilits by merging)

5. To update your side branch by master/main branch: 
``` git merge master ```

or  ``` git merge "branch_name" ```

(after the merg, pull, commit, and push again)

6. Pull branch (to merge on current system):
``` git pull origin "branch_name" ```

7. Delete a local branch:
``` git branch -D "branch_name" ```
to delete a branch on Github use the platform

## Forking:
to creat editable legal copy of any third-party code and add it to your repository.