## To start with, download VScode,open the terminal and connect to AutoDL
1.How to delete extension extensively: delete extension in C:/..../.vscode  

2.if error pops up: "Failed to connect to the remote extension host server (Error: Cannot read properties of undefined (reading 'after'))",check if you deleted the config file, you should fill in the correct stuff.Maybe use another editor or computer to connect the server and log them.

3. New terminal， ls， to check current file.

4.cd +file. go to the file
   
5.cd .. %go back the last directory

6.cd ../../../ %go back to 3 times 

## Open tmux, to protect your process from your pc operations (try everything under this premise)
%download tmux in terminal<br>
apt-get update && apt-get install -y tmux   <br>
% new session<br>
tmux new-session -s maoamo<br>
% reenter session<br>
tmux attach -t maomao<br>
%delete session<br>
tmux kill-session -t maomao<br>
%detach session<br>
tmux detach<br>
%to be efficient,create multiple screens under one session or create multiple session using: bash(+)<br>

## git clone
 if it doesnt work, try replace github.com to githubfast.com(help the server inside China,its a mirror website)

 ## 下载数据集
直接从huggingface、hf-mirror 下载： <br>
#export HF_ENDPOINT=https://hf-mirror.com <br>
huggingface-cli download --repo-type dataset --resume-download 数据集名（../..） --local-dir /root/autodl-tmp/.. <br>

## 删除隐藏.cache等缓存文件
 ls -la /root/autodl-tmp  <br>
 rm -rf /root/autodl-tmp/.*  <br>

 

## file move and download
%move file to another directory<br>
 mv A B % move A to B<br>
 mv A ../  %move A to previous directory    <br>

%file/directory delete    <br>
rm -r directoryname    <br>

%copy and download directory    <br>
cp -r A B % copy directory A to path/to/B(can be a new name)    <br>

%zip    <br>
zip -r newname.zip path/to/file    <br>

%download zip file using xftp,its slow to dorectly download from vscode ide    <br>


## vim,:q
 vim to open the file in the terminal    <br>
 :q means leave without anything changed    <br>
 :wq means keep the change and leave    <br>
 
## check the envs
 cd /root/miniconda3/envs/    <br>
 
## check the terminal history
 ctrl+ B then [
 
