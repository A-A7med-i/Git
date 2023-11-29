# Commands Part 1

## 1- Configuration
```shell
git config --global user.name "User Name"
```
```shell
git config --global user.email "Email"
```
```shell
git config --list
```
![config](https://github.com/A-A7med-i/Git/blob/main/Images/config.jpg?raw=true)

## 2- initial local repo
* First make a directory 
```shell
mkdir name dir
```
* Then move to dir 
```shell
cd name dir
```
* Then i make file.txt to work in it
```shell
echo "Mesg">> name file
```
* Then i initial .git
```shell
git init
```
![init](https://github.com/A-A7med-i/Git/blob/main/Images/init.jpg?raw=true)

## 3- Status 
```shell
git status
```
### we founded the file is untrack 

![status](https://github.com/A-A7med-i/Git/blob/main/Images/status.jpg?raw=true)

## 4- added files to index area
```shell
git add .
```
* (.) Indicates to add all files 

### we founded the file is track 

![added](https://github.com/A-A7med-i/Git/blob/main/Images/added.jpg?raw=true)

## 4- commit file
```shell
git commit -m "message"
```
![commit](https://github.com/A-A7med-i/Git/blob/main/Images/commit.jpg?raw=true)

## 5- Track commit

```shell
git log 
```
```shell
git log --oneline
```
![log oneline](https://github.com/A-A7med-i/Git/blob/main/Images/long%20oneline.jpg?raw=true)

```shell
git cat-file  -t first 7 char of shasum
```

```shell
git cat-file  -p first 7 char of shasum
```
* -t is the type 
* -p show the content 

![log](https://github.com/A-A7med-i/Git/blob/main/Images/log.jpg?raw=true)

## 6- Now i modify the file and make commit

![modify file](https://github.com/A-A7med-i/Git/blob/main/Images/modify%20file.jpg?raw=true)

* from point 3 & 4 :
### (M red) =>  A file not in index area and .git 
### (M green) =>  A file in index area and not in .git

![parent](https://github.com/A-A7med-i/Git/blob/main/Images/parent.jpg?raw=true)

* from above the last commit point to the previous commit

![Flow](https://th.bing.com/th/id/OIP.eExDR06JzW6NMPg7vkG3ngHaET?rs=1&pid=ImgDetMain)

## 7- Difference 

* i modify file then find the difference

```shell
git diff
```

![diff](https://github.com/A-A7med-i/Git/blob/main/Images/diff.jpg?raw=true)


## 8- show 

### track commit

```shell
git show first 7 char of shasum
```

![show](https://github.com/A-A7med-i/Git/blob/main/Images/show.jpg?raw=true)
