# Recruitment 

## 1- Track Everything:

### Git allows you to track every change made to your source code or any other files in your project. Every modification, addition, or deletion is recorded and can be traced back through the commit history.

## 2- OS Independent:

### Git is platform-independent, meaning it works seamlessly across various operating systems, including Windows, macOS, and Linux. This ensures that team members using different operating systems can collaborate without compatibility issues.

## 3- Unique ID:

### Each commit in Git is identified by a unique hash (SHA-1) that serves as a unique identifier. This ensures that every change made to the project is uniquely identified and can be referenced using this hash.

* Example:
```shell
echo "Hello Git" | git hash-object --stdin
```

* Output : 
```
0dec2239efc0bbfabe4078f5357705ca93b5475e
```

* how can git see the pervious command 
```
echo "blob 10\0Hello Git" | git hash-object --stdin
```

* blob is the type and 10 is the size and added a null character \0

* If we pass it to shasum algorithm 
```shell
echo -e"blob 10\0Hello Git" | shasum
```

* We get the same output 


## 4- Track History:

### Git maintains a comprehensive history of your project. You can easily navigate through the commit history, view changes introduced in each commit, and understand the evolution of the project over time.



## 5- No Content Change:

### In Git, once a commit is made, its content is immutable. The unique identifier (hash) of the commit is based on the content of the commit, and changing the content would result in a new commit with a new hash. This ensures the integrity of the project history.

# Git object 

## 1- Blob (File) :

### A blob (binary large object) in Git represents the content of a file at a specific point in time. It is essentially the raw data of a file without any metadata. Blobs store the contents of files, and each blob is uniquely identified by a hash based on its content.


## 2-Tree (Working Directory) :

### A tree object in Git represents a directory or a snapshot of the project's directory structure at a specific commit. It contains references to blobs (file content) and other subtrees, forming a hierarchical structure that mirrors the layout of files and directories in the project.


## 3- Commit:

### A commit object in Git represents a specific state of the project at a given point in time. It includes a reference to a tree object that captures the project's directory structure and the associated blobs representing file contents. Commits also include metadata such as the author, committer, commit message, and a pointer to the parent commit(s), forming a commit history.


## 4-Tag (Tagged):

### A tag object in Git is used to create a human-readable reference to a specific commit. It allows you to assign a meaningful name to a commit, making it easier to refer to important points in your project's history, such as releases or milestones. Tags are typically used to mark specific commit versions as stable or significant. Tags are immutable and do not change as the repository evolves.

# Git uses a three-tree architecture

## 1- Working Directory:

### The working directory is where you have your project files. It's essentially your local file system. When you modify files in your working directory, Git recognizes the changes, but they are not automatically committed.


## 2- Index (Staging Area):

### The index, also known as the staging area, is an intermediate area where you prepare changes before committing them to the repository. It acts as a bridge between the working directory and the repository. When you make changes to files in your working directory, you use commands like git add to stage those changes in the index.


## 2- Repository (HEAD):

### The repository is where Git permanently stores the committed versions of your files, along with their complete history. The repository contains a series of commits, each representing a snapshot of the project at a specific point in time. The latest commit is referred to as HEAD.

#

![3-tree](https://media.geeksforgeeks.org/wp-content/uploads/20191122182103/staging_process.jpg)














