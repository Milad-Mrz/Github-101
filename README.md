# how to use github

## Method no. 1

git clone https://github.com/Milad-Mrz/test.git \n
git add .
git commit -m "..." -m "...2"
git push origin main or git push origin master

---------------------------
## Method no. 2


### to start git for new folder
git init
### to add all changes (either files or new lines)
git add .
### to add new commit with title A and description B
git commit -m "A" -m "B"
### after making a new repository to connect it with VS
git remote add origin https://github.com/Milad-Mrz/test2.git
## to check
git remote -v
## to set an defult branch for future pushes we can use  "-u" just before "origin master"
git push -u origin master
