# tmux Cheat Sheet

## **tmux** is basically a more powerful terminal that allows users to fire up multi-session. It is particularly usefull when doing multi-session-required tasks such as ssh to a remote server. This Markdown file serves as a cheat sheet for operating tmux.

1. **tmux installation**
   ```
   # Ubuntu
   sudo apt-get install tmux

   # mac
   brew install tmux

   # Fuck windows
   ```
   ```
   #start
   tmux
   ```
   
2. **Navigating through sessions and windows**

    First note that server >> session >> window >> pane
    
    function | shortcut
    ---|---
    before action | ctrl + b
    ---|---
    detach sessions | ctrl + b + d
    kill all sessions (kill tmux server) | tmux kill-server 
    list sessions | tmux ls 
    attach sessions | tmux attach -t #no.
    tmux kill-session -t #no
    ---|---
    create window | ctrl + b + c 
    navigate to next window |ctrl + b + n
    navigate to previous window |ctrl + b + p
    navigate to specific window | ctrl + b + #no.
    find window | ctrl + b + f
    rename window | ctrl + b + ,

3.  **Navigating through panes**
    function | shortcut
    ---|---
    split horizontally | ctrl + b + %
    split vertically |ctrl + b + "
    close pane | ctrl + b + x
    navigate to neighbor panes | ctrl + b + #arrow
    scroll up lines | ctrl + b + [

4. kill tmux
   ```
   pkill -f tmux
   ```