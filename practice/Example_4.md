## Removes a file from git 

`git rm hello.txt`  
`git commit -m "Remove hello.txt"`  


### what it does:

`git rm hello.txt`  
- Deletes the file from your working directory and stages that deletion for the next commit.
    - The file `hello.txt` is removed from the present working directory 
    - Git marks it as "deleted" in the staging area


`git commit -m "Remove hello.txt"`  
- It creates a commit that records that `hello.txt` was deleted.