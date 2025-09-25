## Ignore unwanted files

`echo "node_modules/" > .gitignore`  
`git add .gitignore`  
`git commit -m "Add .gitignore"`  

### What it will do:

`echo "node_modules/" > .gitignore`  
- It creates a file names `.gitignore` 
- writes the text 'node_modules/' into it 
- `.gitignore` is like do not track list for git


`git add .gitignore`  
- Adds the `.gitignore` file itself to the staging area

`git commit -m "Add .gitignore"`  
- creates a commit 

