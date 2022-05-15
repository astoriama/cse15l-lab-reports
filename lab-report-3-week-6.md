# Lab report 3
## Streamlining ssh Configuration
### Showing and editing my .ssh/config file
- I accessed my `.ssh/config` file by using:
```
% cd ~ .\ssh
% cat config
```
- Which gives:
<img src="showSSHfile.jpeg"
     alt="showSSHfile"/> 

- I edited the file using:
```
% chmod +x config
% vim config
```
- Which opens up the file in my terminal for me to edit, then I pressed `i` to enter insert mode. Where I changed my original host name to my alias `nini`:
<img src="changeAlias.png"
     alt="changeAlias"/> 


### Show the ssh command logging you into your account using just the alias you chose:

- Since I chose `nini` as my alias I used command
`$ SSH nini`:

<img src="SSHnini.jpeg"
     alt="SSH nini" /> 


### Show an scp command copying a file to your account using just the alias you chose.

- I created a file named HereIam.java, then:
```
(base) astoria@Astorias-MacBook-Pro markdown-parser % scp HereIam.java nini:~/
HereIam.java                                                  100%  303    12.5KB/s   00:00  
```
- Comparing the list of files before and after the command, we can see the file has been successfully copied:
     - Before:
<img src="beforeSCP.png"
     alt="beforeSCP"
     style="float: left; margin-right: 10px;" /> 

     - After:
<img src="afterSCP.png"
     alt="afterSCP"
     style="float: left; margin-right: 10px;" /> 

## Setup Github Access from ieng6

### Public key and private key
- Public key on my user account is stored in id_rsa.pub file in .ssh directory, while private key is stored in id_rsa file:
<img src="lsSSH.png" 
     alt="lsSSH"
     style="float: left; margin-right: 10px;" /> 

- As I open id_rsa.pub file, I get my public key:
<img src="catid_rsa.pub.png" 
     alt="catid_rsa.pub"
     style="float: left; margin-right: 10px;" /> 

- As I open id_rsa file, I get my private key (content not included):
<img src="catprivatekey.png" 
     alt="catprivatekey"
     style="float: left; margin-right: 10px;" /> 

- Public Key on github is stored in setting:

<img src="publicKeyOnGithub.jpeg" 
     alt="PublicKeyOnGithub"
     style="float: left; margin-right: 10px;" /> 

## Running git commands to commit and push a change to Github while logged into your ieng6 account:
- I modified my `MarkdownParseTest.java` file and commited my change:
<img src="gitCommit.png" 
     alt="gitCommit"
     style="float: left; margin-right: 10px;"
     width="500" /> 

- Then, I pushed:
<img src="gitPush.png" 
     alt="gitPush"
     style="float: left; margin-right: 10px;" /> 

- A link to my commit is [here](https://github.com/astoriama/markdown-parser/commit/e62f94fa4cf0a7cbd3102f8f9bed7c6b896809fa).

## Copy whole directories
- Using `scp -r` I copied all my files recursively into my user account:
<img src="scp-r.png" 
     alt="scp -r"
     style="float: left; margin-right: 10px;" /> 

- Running file on server:
<img src="runFileOnServer.png" 
     alt="runFileOnServer"
     style="float: left; margin-right: 10px;" /> 

- Combination of commands:
<img src="manyCommands.png" 
     alt="manyCommands"
     style="float: left; margin-right: 10px;" /> 

