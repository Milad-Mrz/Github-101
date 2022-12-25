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

4. Push the changes to the "branch_name":
``` git push origin branch_name ```

5. To set a default branch for future pushes, we can use "-u" just before "origin":
``` git push -u origin branch_name ```


## Branching:
1. To check current branches:
``` git branch ```

2. To create a new branch named "A":
``` git checkout -b A ```

3. To switch to the "master" branch:
``` git master checkout ``` 
