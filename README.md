# How to use Github 101 <br />
Here is a summary of commands for pushing, pulling, and branching after connecting your local machine to Github. <br />
## Utilizing git for teamwork and file management
**Clone:** <br />
this is used to copy the remote version (on Github) and make a local copy. <br />

**Method I:** <br />
Clone or download the existing repository from git: <br />
``` git clone https://github.com/user_name/repository_name ```<br />

**Method II (Remote):** <br />
1. Start git for a new folder: ``` git start ```  <br />
2. Access the existing repository from Github: <br />
``` git remote add origin https://github.com/user_name/repository_name ``` <br />
3. Check the access: ``` git remote -v ``` <br />

**Pull:** <br />
Use Pull to receive the latest version of the remote version; pulling will update the local version. <br />
1. To update from "branch_name_example," use ``` git pull origin branch_name_example ``` <br />
2. As before, we can use "-u" just before "origin": <br />
``` git pull -u origin branch_name_example ``` Following that, we can run the command ``` git pull ``` . <br /> 

**Push:** <br />
After cloning and all the modifications, push will update the remote version: <br />
1. Add all changes (either files or new lines): ```git add .``` <br />
2. Make modifications to a specific file: ``` git add "file_name.extension ``` <br />
3. Create a new commit with title "A" and description "B": ``` git commit -m A -m B ``` <br />
   or, use the shortcut, for steps 2 & 3: ``` git commit -am A -m B ``` <br />
   only in cases of file modification, this will add all modifed files and commit at the same time <br />
4. Push the changes to the "branch_name_example": ``` git push origin branch_name_example ``` <br />
5. To set a default branch for future pushes, we can use "-u" just before "origin": <br />
   ``` git push -u origin branch_name_example ``` After this, by simply writing  ``` git push ``` changes will be pushed to Github. <br />
   
**Branching, merging:** <br />
Branches are needed to create and modify new features while protecting the main version.  <br />
Merging and pulling are used to sync up two different branches. <br />

1. To check all local branches: ``` git branch ``` <br />
2. To create a new branch named "branch_name_example": ``` git checkout -b branch_name_example ``` <br />
3. switch to, for example, the "master" branch: ``` git checkout master ``` <br />
4. Check the current branch and the "branch_name_example" and show the changes that have been made: <br />
``` git diff "branch_name_example" ``` <br />
   (If there are confilicts between two versions then: press **q** to quit and you can address those confilits by merging) <br />
5. To update your side branch by master/main branch use ``` git merge master ``` or ``` git merge "branch_name" ```, and after the local merge, pull, commit, and push to update the remote version. <br />
6. Pull a branch or to merge with a remote branch: ``` git pull origin "branch_name_example" ``` <br />
7. Delete a local branch: ``` git branch -D "branch_name_example" ``` & to delete a branch on Github use the platform. <br />

**Forking:** <br />
To create an editable legal copy of any third-party code and add it to your repository. <br />
<br />
<br />

## How to document a Project on GitHub: <br />

**Adding illustrations to the README file:** <br />
Use the following command to add files to fist page on Github.  ``` ![ ](./Folder/Image.png) ``` <br />

**Other Github tools:** <br />

1. **Pandoc:** To convert any document such as word, pdf, or html to Github's markdown, we can use Pandoc on Linux as below: <br />
   1.1. Install pandoc on Linux from https://pandoc.org/ . <br />
   1.2. Open a terminal in the file directory and use the command:  <br />
      ``` pandoc -s example_file --to=gfm -o README.md ``` <br />
