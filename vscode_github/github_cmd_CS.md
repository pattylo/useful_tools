# GitHub CMD Cheat Sheet

1. **Init**
   
   Create a repo on your GitHub, named ```{lala}```. Then, in your directory that you want to push, do the following:
   ```
   git init
   git remote add origin https://github.com/{username}/{lala}.git
   git branch -M main
   git add .
   git commit -m "initial commit"
   git push -u origin main

   ```
2. **General Commit**
   ```
   git status
   git add .
   git commit -a || git commit -m "{message}" # (quit vim: esc + ":wq")
   git push -u origin main

   ```
3. **Merge Local Repo with Remote Repo**
   
   Do this to set remote (origin)
   ```
   git remote set-url origin https://github.com/pattylo/gan.git
   git remote add origin https://github.com/pattylo/gan.git
   git remote -v
   git pull origin main --allow-unrelated-histories
   # resolve conflict if needed
   git push -u origin main
   ```
   
4. **Branching and Tagging**
    
    Branching
    ```
    git branch {new branch-name}
    git branch # check all branches
    git switch {branch-name} || git checkout {branch-name}
    git push -u origin {branch-name}
    ```
    
5. **Pull Request**
   
6. **Others**
   
   Undo last commit 
   ```
   git reset --soft HEAD~
   ```

