## Track a new file and commit it

`echo "Hello Git" > hello.txt`  
`git status`  
`git add hello.txt`  
`git commit -m "Add hello.txt"`  


### what it does:
`echo "Hello Git" > hello.txt`  
It creates a new file named `hello.txt`  
writes the next "Hello Git" into that file 


`git status`  
- It shows you what have changed in your working directory:
    - which files are untracked
    - which files are staged
    - which files have chnaged not committed
- Here, `hello.txt` is not tracked by git and it is a new file 


`git add hello.txt`  
- It stages the file for commit.
- That means, "Git, I want to include this file in my next commit"


`git commit -m "Add hello.txt"`  
- It commits the staged file to the repo with a message:
    - "Add hello.txt" becomes the commit message
    - Git saves a snapshot of the file in its current state





