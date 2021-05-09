# Linux Commands
The basic linux commands to be known to work on the linux platform.
### 1. pwd command
The `pwd` command is for knowing the present working directory. It returns the absolute path starting from forward slash(/).  

*Example:*
 ```
 $ pwd
 /home/usr/mydirectory
 ```
  
 ### 2. cd command
 The `cd` command helps in changing the directory.It requires the full path or the name of the directory.Suppose you are in /home/usr/mydirectory you can switch to new directory 'projects'
 under my directory by:  
 
 *Example:*
  ```
  $ cd projects
  $ cd /home/usr/Documents
  ```
 **Some shortcuts to cd:**
 1. cd .. => helps in moving to one previous directory
 2. cd ~ => move directly to home directory

### 3. ls command
The `ls` command helps helps in listing the contents under a directory.  

*Example:*
```
$ ls /home/usr/mydirectory
```
**some basic options to be used with `ls`:**
1. ls -a => listing the hidden files
2. ls -al => lists contents with permissions,owner,size
3. ls -ltr => lists contents in reverse sorted order by modification time

### 4. cat command
The `cat` command helps in displaying the contents of file in a terminal. Sometimes the `cat` command can be used to create the file.  

*Example:*
```
$ cat /home/usr/mydirectory/myfile.txt
$ cat>filename (creates new file)
```

### 5. mv command
The `mv` command helps in moving the file or renaming the file.    

*Example:*
```
$ mv oldfile.txt newfile.txt (renaming the file, make sure you dont have the same new name file existing else it will overwrite the file) 
$ mv oldfile.txt /home/usr/mydirectory/myfile.txt (moving file contents to the required destination)
```

### 6. cp command
The `cp` command helps in copying of files.  

*Example:*
```
$ cp oldfile.txt newfile.txt (create new file newfile.txt before copying)
```

### 7. mkdir and rmdir command
The `mkdir` command helps in making the new directories.  
The 'rmdir` command helps to remove the empty directories.  

*Example:*
```
$ mkdir <path where the directory is to be created>
$ rmdir newdirectory
```

### 8. rm command
The `rm` command helps in removing of files.  

*Example:*
```
$ rm oldfile.txt 
$ rm -rf <directoryname>  (to delete the recursive subdirectories and files)
```

### 9. clear command
The `clear` command helps in clearing the terminal/command line.  

*Example:*
```
$ clear
```

### 10. vi/vim/gedit command
The `vi/vim/gedit` command helps in creating the new file and entering the contents.Once the command is given it creates new file and a editor is opened to write. Simply click `insert`
button to start editing the file. To quit the file use, `esc`+ `:wq`

*Example:*
```
$ vi myfile.txt
```

### 11. ps command
The `ps` command shows the number of processes running with the pid.  

*Example:*
```
$ ps
$ ps -ef (displays all processes with detailed info)
```

### 12. kill command
The `kill` command is used to kill the process with pid .  

*Example:*
```
$ kill -l (lists all available signals)
$ kill -9 <pid> (kills the process with the given pid)
```

### 13. grep command
The `grep` command helps in searching the text in a given file.  

*Example:*
```
$ grep python newfile.txt (searches for python word in newfile.txt)
$ grep -nr <pattern> /home/usr/mydirectory (searches recursively in all files in a directory and gives the line number)
$ grep -nr Test.123.sdf.* /home/usr/mydirectory (searches for the pattern which matches Test.123.sdf.*, * indicates anything of that pattern.)
$ ps -ef | grep vnc (finds all the process and then match vnc in the processes. | indicates the pipe operator used to run multiple commands by providing the output of one command to the next one) 
```

### 14. chmod command
The `chmod` command allows to provide read,write,execute permissions to the file.
Read(r) = 4
write(w) = 2
execute(x) = 1
*Example:*
```
$ chmod 777 dirname (gives the r,w,x permissions to all i.e owner(u), group(g), others(o) 
```


