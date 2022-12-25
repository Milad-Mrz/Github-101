# how to use github

## Method no. 1

1. git clone https://github.com/Milad-Mrz/test.git
2. git add .
3. git commit -m "..." -m "...2"
4. git push origin main or git push origin master

---------------------------
## Method no. 2

1. to start git for new folder
git init
2. to add all changes (either files or new lines)
git add .
3. to add new commit with title A and description B
git commit -m "A" -m "B"
4. after making a new repository to connect it with VS
git remote add origin https://github.com/Milad-Mrz/test2.git
5. to check
git remote -v
6. to set an defult branch for future pushes we can use  "-u" just before "origin master"
git push -u origin master

-------------------------------------------------
## branch:

1. to check current branchs:
git branch

2. to create a new branch as "feature-1"
git checkout -b feature-1

3. to switch to "master" branch
git checkout master