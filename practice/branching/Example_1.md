### Reproduce a Merge Conflict Step-by-Step:

Step 1: Create a repo and add a file

`git init merge-conflict-demo`  
`cd merge-conflict-demo`  
`echo "Hello Git" > hello.txt`  
`git add hello.txt`  
`git commit -m "Initial commit"`  

Step 2: Create and Switch to a new branch 

`git checkout -b feature-1`  
`echo "This is Feature 1" > hello.txt`  
`git commit -am "Edit hello.txt in feature-1"`  

Step 3: Switch to main and edit same line 

`git checkout main`  
`echo "This is Main branch" > hello.txt`  
`git commit -am "Edit hello.txt in main"`  

Step 4: Try to merge feature-1 into main

`git merge feature-1`  

Now, Git will say,

Auto-merging hello.txt
CONFLICT (content): Merge conflict in hello.txt
Automatic merge failed; fix conflicts and then commit the result.






