# [OSS] CLI_1 Week4_Lab4  
#### 202234880 Kimtaewoo  
---
### Linux  
- Open-source Unix-like Operating systems and kernels  
- First released by Linus Torvalds in 1991  
- Runs on CLI, but support GUIs  


### Kernel and Shell  
- Kernel : Core of OS, control/communicates with hardware  
- Shell : Interface that allows users to communicate with kernel  

---
### Shell commands  

```sh
$ pwd
```
pwd : shows the current path in a hierarchical directory  
```sh
$ cd (directory)
$ ls
```
cd : change directory  
ls : list files and directories  
- -l : show detailed info
- -lh : same as above, but size in units

```sh
$ clear
```
clear : same 'cls' in windows cmd  
```sh
$ cp -i (file1) (file2)|(dir2)
$ cp -R (dir1) (dir2)
```
- cp : copy files/directories, if file2 exists, overwrite it.
- -i : if file2 exists, user is prompted before it is overwritten.
- -R : copy contents of the dir1 to dir2

```sh
$ mv file1 file2 //rename file1 to file2
$ mv file1 dir1 //move file1 to dir1
$ mv file1 file2 dir1 //file1 and file2 are moved to dir1
```
mv : move file or rename it  
```sh
$ rm -i|-r file1
```
- rm : delete files/directories
- -r : delete directories option
- -i : user interactive option
```sh
$ mkdir (dir)
```
mkdir : make directory  

```sh
$ exit
```
---