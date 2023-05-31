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
   
2. **Navigating through sessions**
    
    function | shortcut
    ---|---
    before action | ctrl + b  
    create session|ctrl + b + c 
    navigate to next session |ctrl + b + n
    navigate to previous session |ctrl + b + p
    navigate to specific session | ctrl + b + #no.
    detach sessions | ctrl + b + d
    find sessions | ctrl + b + f
    list sessions | tmux list-sessions  
    attach sessions | tmux attach-session -t #no.
    kill all sessions | tmux kill-window -t #no. / ctrl + b + &


3.  **Navigating through panels**
   
   function | shortcut
    ---|---
    split horizontally | ctrl + b + %
    split vertically |ctrl + b + "
    close panel | ctrl + b + x
    navigate to neighbor panels | ctrl + b + #arrow

4. kill tmux
   ```
   pkill -f tmux
   ```