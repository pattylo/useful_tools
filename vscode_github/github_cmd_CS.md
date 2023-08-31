# GitHub CMD Cheat Sheet

1. **Init**
   
   Create a repo on your GitHub, named ```{lala}```. Then, in your directory that you want to push, do the following:
   ```
   git config --global user.name {name}
   git config --global user.email {email}
   git config --global --unset user.name
   git config --global --unset user.email

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
   git remote set-url origin https://github.com/pattylo/gan.git  # ||
   git remote add origin https://github.com/pattylo/gan.git
   git remote -v

   git pull origin main --allow-unrelated-histories
   git config pull.rebase false # if neccessary
   # resolve conflict if needed
   git push -u origin main
   
   # Note that do set the default main (master in legacy)
   git remote set-head origin {branch-name} # 
   
   ```
   
4. **Branching and Tagging**
    
    Branching
    ```
    git branch {new branch-name}
    git checkout -b {new branch-name} {off which branch}

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

   View what has been change without doing anything on the locals; ```git pull``` will really modifiy the local files.
   ```
   git fetch
   ```

   Note that
   ```
   git pull = git fetch + git merge
   ```


