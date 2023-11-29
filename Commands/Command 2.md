# Command Part 2

# Undoing Things

## 1- Untrack file

```shell
git rm --cached file.txt
```

![untrack]()

## 2- restor file

### I modify file 

![edite file]()

```shell
git restor file.txt
```

![restor]()

### After restor
![After restore]()

## 3- unstaged file

### if we added file and become in index area we can unstaged file and modifications that do not change now i modify the file

![edite unstaged]()

```shell
git restor --staged file.txt
```

![unstaged]()

### After unstaged
![edite unstaged]()

## 4- Head

### Head is pointer You can control it and control the commits

```shell
git reset  HEAD~1
```
### 1 refer to back one commit


![HEAD]()

### but change the head witout --hard it has no effect on working tree 

![HEAD WITOUT --HARD]()

### to fast forward 
```shell
git reset  HEAD@{1}
```
![fast forward]()


## 5- HEAD --hard

### --hard effect on the WT

### back pointer
```shell
git reset --hard HEAD~1
```
### forward pointer
```shell
git reset --hard HEAD@{1}
```

![--hard]()

## 6- tagged
### tags in Git are references to specific commits in the repository's history. They are used to mark significant versions

### There are two types of tags in Git: lightweight tags and annotated tags.

#### 1- Lightweight tags: A lightweight tag is simply a name or label assigned to a specific commit. It is created by running the command git tag <tag-name>. Lightweight tags are similar to branch names and do not contain any additional metadata. They are easy to create and do not require much disk space.

#### 2-Annotated tags: An annotated tag, on the other hand, contains additional information such as a tagger's name, email, date, and an optional message. Annotated tags are created using the git tag -a <tag-name> command. This type of tag is recommended when you need to store extra information about the tag, such as release notes or important details.

```shell
git tage -a version -m "message"
```
![tagged]()