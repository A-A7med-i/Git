# Commands part 3

## Branching

### branches in Git are movable pointers that represent independent lines of development within a repository. They enable parallel development, isolation, collaboration, and provide a structured approach to managing features or bug fixes.

![Branch](https://github.com/ahmedsami76/AraBigData/blob/main/Git/images/git10.jpg?raw=true)


## 1- alias 
```shell
git log --oneline --decorate --graph --all
```
#### the previous command use to show commits in a graphical 
![graph](https://github.com/A-A7med-i/Git/blob/main/Images/graph.jpg?raw=true)
#### or we can use alias to become easy
```shell
alias graph="git log --oneline --decorate --graph --all"
```
#### same the previous 
## 2-New branch
```shell
git branch name of branch
```

```shell
git branch 
```

```shell
git switch name of new branch
```

![new branch](https://github.com/A-A7med-i/Git/blob/main/Images/new%20branch.jpg?raw=true)

#### after switch to test branch i will make new commit and see graph

![test branch](https://github.com/A-A7med-i/Git/blob/main/Images/test%20branch.jpg?raw=true)


## 3- merge linear branch
```shell
git merge name of branch 
```
![merge](https://github.com/A-A7med-i/Git/blob/main/Images/merge.jpg?raw=true)
### delete branch
```shell
git branch -d name of branch 
```
![delete branch](https://github.com/A-A7med-i/Git/blob/main/Images/delete%20branch.jpg?raw=true)

## 4- merge nonlinear branch
### I create branch and make a commit in it
![non linear 1](https://github.com/A-A7med-i/Git/blob/main/Images/non%20linear%201.jpg?raw=true)
### In branch master i create a commit
![non linear 2](https://github.com/A-A7med-i/Git/blob/main/Images/non%20linear%202.jpg?raw=true)
### Edite the name of branch master to main then i merge test in main
![non linear 3](https://github.com/A-A7med-i/Git/blob/main/Images/non%20linear%203.jpg?raw=true)

# Working with remote

## 3- i initial repo in my physical machine and we assume this is remote repo

![remote](https://github.com/A-A7med-i/Git/blob/main/Images/remote.jpg?raw=true)
![init remote](https://github.com/A-A7med-i/Git/blob/main/Images/init%20remote.jpg?raw=true)

## 5- cloning this remote repo
```shell
git clone link of remote repo
```
![clone](https://github.com/A-A7med-i/Git/blob/main/Images/clone.jpg?raw=true)

## 6- change the remote

![edite remote](https://github.com/A-A7med-i/Git/blob/main/Images/edite%20remote.jpg?raw=true)

## 7- fetch 
```shell
git fetch origin
```
![fetch](https://github.com/A-A7med-i/Git/blob/main/Images/fetch.jpg?raw=true)

## 8- merge updates 
```shell
git merge
```
![merge fetch](https://github.com/A-A7med-i/Git/blob/main/Images/merge%20fetch.jpg?raw=true)

## 9- pull =fetch + merge
### remote have change
```shell
git pull origin
```
![pull](https://github.com/A-A7med-i/Git/blob/main/Images/pull.jpg?raw=true)

## 10- push 
### local have change
![local before push](https://github.com/A-A7med-i/Git/blob/main/Images/local%20before%20push.jpg?raw=true)
```shell
git push -u origin master
```
* -u (--set-upstream) => create branch master and synchronize updates
### After push in local
![after push](https://github.com/A-A7med-i/Git/blob/main/Images/after%20push.jpg?raw=true)
### After push in remote
![remote after](https://github.com/A-A7med-i/Git/blob/main/Images/remote%20after.jpg?raw=true)





