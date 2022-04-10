## Week 2 Lab Report
A totorial for incoming 15L students, or future me, about how to log into a course-specific account on `ieng6`.
1. Installing VScode

    * Download install package [for Mac](https://code.visualstudio.com/sha/download?build=stable&os=darwin-universal) or [for Windows](https://code.visualstudio.com/sha/download?build=stable&os=win32-user).
    What you should get:
    <img src="VScode setup.png"
     alt="VScode setup"
     style="float: left; margin-right: 10px;" /> 
    * install OpenSSH, following [instructions](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse).<br>
<br>
2. Remotely Connecting
    * open terminal
    * enter command `ssh cs15lsp22__@ieng6.ucsd.edu`, put your identical characters on the underline.
    * Then they should ask you for your password, enter your password.
    * After aforementioned process, you should get: <img src="SSHenter.png"
     alt="SSHenter"
     style="float: left; margin-right: 10px;" /> 
<br>
3. Trying Some Commands
    | Commands  | Description |
    | :----:      | :---      |
    | mkdir | Make directory     |
    | pwd | Print work directory     |
    | cd   | Change directory       |
    | \~  | represents `home` directory       |
    | ls  | List files        |
    | ls -l   | List files, inlong listing format        |
    | ls -a  | List files, including files starting with dot `.`       |
    | ls -t | List files, with time   |
    | cat | concatenate, output file content |
    | exit | logout |

    An example of trying commands: 
<img src="trycommands.png"
     alt="VScode setup"
     style="float: left; margin-right: 10px;" /> 

4. Moving Files with scp
5. Setting an SSH Key
6. Optimizing Remote Running


