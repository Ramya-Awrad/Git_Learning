## Edit a file and see changes

`echo "Another line" >> hello.txt`  
`git diff`  
`git add hello.txt`  
`git commit -m "Update hello.txt"`  


### What it does:

`echo "Another line" >> hello.txt`  
- It appends the text `"Another line"` to the end of the file `hello.txt`
- The `>>` means append, not overwrite.
- here, `hello.txt` already tracked, Git will notice that it has changed.


`git diff`  
- It shows the difference between:
    - The last committed verion of the file
    - The current version(modified but not yet staged)
- This tells you what new content was added since the last commit


`git add hello.txt`  
- It stages the modified file so it can be committed


`git commit -m "Update hello.txt"`  
- It create a new commit with the latest version of the file
