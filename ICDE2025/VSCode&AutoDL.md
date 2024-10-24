# To start with, download VScode 
1.How to delete extension extensively: delete extension in C:/..../.vscode  

2.if error pops up: "Failed to connect to the remote extension host server (Error: Cannot read properties of undefined (reading 'after'))",check if you deleted the config file, you should fill in the correct stuff.Maybe use another editor or computer to connect the server and log them.

3. New terminal， ls， to check current file.

4.cd +file. go to the file
   
5.cd .. %go back the last directory

6.cd ../../../ %go back to 3 times 

# Open tmux, protect your process (try everything under this premise)
%download tmux in terminal
apt-get update && apt-get install -y tmux   
% new session
tmux new-session -s maoamo
% reenter session
tmux attach -t maomao
%delete session
tmux kill-session -t maomao
%detach session
tmux detach

%to be efficient,create multiple screens under one session or create multiple session using: bash(+)

# git clone
 if it doesnt work, try replace github.com to githubfast.com(help the server inside China,its a mirror website)

 ## move file to another directory
 mv A B % move A to B
 mv A ../  %move A to previous directory

 ## vim,:q
 vim to open the file in the terminal
 :q means leave without anything changed
 
 ## check the envs
 cd /root/miniconda3/envs/
 
