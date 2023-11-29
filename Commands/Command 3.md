# Commands part 3

## Branching

### branches in Git are movable pointers that represent independent lines of development within a repository. They enable parallel development, isolation, collaboration, and provide a structured approach to managing features or bug fixes.

![Branch](https://github.com/ahmedsami76/AraBigData/blob/main/Git/images/git10.jpg?raw=true)


## 1- alias 
```shell
git log --oneline --decorate --graph --all
```
#### the previous command use to show commits in a graphical 
![graph]()
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

![new branch]()

#### after switch to test branch i will make new commit and see graph

![test branch]()


## 3- merge linear branch
```shell
git merge name of branch 
```
![merge]()
### delete branch
```shell
git branch -d name of branch 
```
![delete branch]()

## 4- merge nonlinear branch
![non linear 1]()
#
![non linear 2]()
#
![non linear 3]()

# Working with remote

## 3- i initial repo in my physical machine and we assume this is remote repo

![remote]()
![init remote]()

## 5- cloning this remote repo
```shell
git clone link of remote repo
```
![clone]()

## 6- change the remote

![edite remote]()

## 7- fetch 
```shell
git fetch origin
```
![fetch]()

## 8- merge updates 
```shell
git merge
```
![merge fetch]()

## 9- pull =fetch + merge
### remote have change
```shell
git pull origin
```
![pull]()

## 10- push 
### local have change
![local before push]()
```shell
git push -u origin master
```
* -u (--set-upstream) => create branch master and synchronize updates
![after push]()
![remote after]()





