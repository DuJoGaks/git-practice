# [OSS] CLI_2 Week5_Lab5  
#### 202234880 Kimtaewoo  
---
### I/O Redirection : Standard Output  
- Default : Standard output is screen.  
- Using ">" after command, save output to file.  
- Using ">>" to append output to text file.  
- Using "cat" to display text file in CLI  
```sh
$ ls -lh > file.txt //output to file
$ ps >> file.txt //append
$ cat file.txt //read text file
```

### I/O Redirection : Standard Input  
- Default : Standard input is keyboard.   
- Using "<" after command, read input from text file.  
- You can mix "<" and ">" in same line.  
```sh
$ sort < in.txt > file.txt //input from in.txt and output to file.txt
$ cat file.txt //read text file
```
---
## Shell Things  
### Pipeline "|"  
- feeds output of previous command to input of next command  
- command1 | command2 | command3 | ...  
```sh
$ ls -lh | less
$ ls | wc -l //file counter of current directory
```
### Expansion  
- "echo" like print(), just print.
- "echo *" : wildcard! display EVERYTHING
- "echo ~" : ~ means /home/usrname
- backslash \ : to operate like "enter"
- "history > file" to see previous commands history

---
## Permission (!!important!!)  
- Linux is a multi-user sys.
- File/directory have permission assigned differently "owner/group/others"
```sh
$ ls -l /bin/bash
-rwxr-xr-x 1 root root ...
  rwx / r-x / r-x
-owner/group/others permission
```
 **CHANGE PERMISSION**
 ```sh
 $ chmod NNN filename
 ```
 - 6 = 110(bin) = rw- for owner
 - 0 = 000(bin) = --- for group
 - 0 = 000(bin) = --- for others
 - value : 777, 755, 700, 666, 644, 600, ...
 
---

## Superuser
- superuser has all sys administation authority!
- Some commands need SU's authority.
- Use "sudo" run command to SU.
```sh
$ sudo apt-get update
$ sudo apt-get upgrade
```
---
### Shell Script
- in linux, can choose CLI-Based / GUI-Based text editors.
- vi/vim , nano, Emacs, gedit(gui) ...
```sh
$ nano script.sh
```
