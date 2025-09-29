1. Create a branch 

`git checkout -b add-greeting`  

What it does:  
    - creates a new branch called add-greeting 
    - switches to that branch 

2. Make some changes:

make changes into that new branch

Stage and commit the changes

`git add .`  
`git commit -m "msg"`  

3. Switch back to main branch 

`git checkout main`  

4. Merge the new branch into main

`git merge new-branch`  
 Note: if no conflicts, then the changes are now part of main

5. Push to Remote

`git push origin main`  

6. Delete the new branch

`git branch -d new-branch`  

7. Delete remotely

`git push origin --delete new-branch`  
