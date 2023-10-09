# Linux_Basics


> Linux basic for every DevOps Engineer

## File Manipulation

- **sudo**

  > it runs your command with administrative or root permissions.

  `sudo (command)`

  ![Image](images/Screenshot_1.png)

- **pwd**

  > displays the current working directory

  `pwd [option]`
  ![Image](images/Screenshot_2.png)

- **cd**

  > changes the curent directory to the specified path

  `cd [Filename]` or `cd /home/ubuntu/Filename`
  ![Image](images/Screenshot_3.png)
  
- **ls**

  > list files and directories
    - **ls -R** : lists subdirectories recursively
    - **ls a** : shows all files and directories including hidden files
    - **ls -lh** : displays file sizes in a human-readable format
    
  `ls /home/ubuntu`
  `ls -R`
  `ls a`
  `ls -lh`

  ![Image](images/Screenshot_4.png)

- **cat**

  > this command lists, combines and writes file content to the standard output.
    - `cat > filename` : creates a new file
    - `cat filename.txt filename2.txt > filename3.txt` : merges the first two files and stores the output in **filename3*.txt*
    - `tac filename` : displays content in reverse order

  `cat filename`
  `cat filename filename2 > filename3`
  `tac filename`
  
  ![Image](images/Screenshot_5.png)
  ![Image](images/Screenshot_6.png)

- **cp**

   > this command is to copy files or directories, including their content form your current directory to another.
     - `cp -R` : Duplicating an entire directory, pass the **-R** flag followed by the source and destination directory

  `cp file1 file2 /home/username/Directory`
  `cp filename filename`
  `cp -R /home/username/Directory /home/username/Directory_backup`
  
  ![Image](images/Screenshot_7.png)
  ![Image](images/Screenshot_8.png)
  ![Image](images/Screenshot_9.png)

- **mv**

  > use this command to move or rename files and directories. This command can also be use to **renamea file**

  `mv filename /home/username/Directory`
  `mv filename newfile`
  
  ![Image](images/Screenshot_10.png)

- **mkdir**

  > command to create one or multiple directories and set their permissions. Ensure you are authorized to make a new folder in the parent directory. 
  
  `mkdir [option] directory_name`
  `mkdir Directory/File` 
  
  ![Image](images/Screenshot_11.png)

- **rmdir**

  > command to delete an **empty directory**. The user must have sudo privileges in the parent directory.

  `rmdir -p Directory/File`
  
  ![Image](images/Screenshot_12.png)

- **rm**

   > use this command to permanently delete files within a directory.

  `rm filename`
  `rm filename1 filename2 filename3`
  
  ![Image](images/Screenshot_13.png)

- **touch**

  > the touch command lets you create an empty file in a specified directory path

  `touch filename`
  
  ![Image](images/Screenshot_14.png)

- **locate**

  > lets you find a file in the database system.
  `locate -i filename`
  
  ![Image](images/Screenshot_15.png)

- **find**

  > use this command to search for files within a specific directory

  `find [option] [path] [expression]`
  
  ![Image](images/Screenshot_16.png)

- **grep**

  > lets you find a word by searching the content of a file. The command prints all lines containing the matching strings, this is useful of for filtering.

  `grep [option] filename`
  
  ![Image](images/Screenshot_17.png)

- **df**

  `df [options] [file]`
  `df -h`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_18.png)

- **du**

  `du /home`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_19.png)

- **head**

   > prints the first ten lines of a text file

  `head [option] [file]`
  
  ![Image](images/Screenshot_21.png)

- **tail**

   > displays the last ten lines of a file

  `tail [option] [file]`
   `tail -n [file]`
  
  ![Image](images/Screenshot_22.png) 
  ![Image](images/Screenshot_23.png)

- **diff**

  > compares two files' content and outputs the differences.

  `diff [option] file1 file2`
  
  ![Image](images/Screenshot_24.png)

- **tar**

  > The tar command archives multiple items into a **TAR** file
  
  `tar [options] [archive_file] [file or directory]`
  
  ![Image](images/Screenshot_25.png)

## File Permissions and Ownership

- **chmod**

  `chmod [option] [permission] [file_name]`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_26.png)

- **chwon**

  `chwon [option] owner[:group] file(s)`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_27.png)

- **jobs**
  `jobs [options] jobID`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_28.png)

- **kill**

  `ps ux`
  `kill [signal_option] pid`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_29.png)

- **ping**

  `ping [option] [hostname_or_IP_address]`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_30.png)

- **wget**

  `wget [option] [url]`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_31.png)

- **uname**

  uname [option]
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_32.png)

- **top**

  `top`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_33.png)

- **history**

  `history [option]`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_34.png)
  ![Image](images/Screenshot_35.png)

- **man**

  `man [command_name]`
   `man [option] [section_number] [command_name]`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_36.png)

- **echo**

  `echo [option] [string]`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_37.png)

- **zip, unzip**

  > **zip** command lets you compress items into a **ZIP** file.
  > **unzip** this command will extract the compressed file.

   `zip [options] zipfile file1 file2`
   `unzip [option] file_name.zip`
  
  ![Image](images/Screenshot_38.png)
  ![Image](images/Screenshot_39.png)

- **hostname**

  `hostname [option]`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_40.png)

- **useradd, userdel**

  `useradd [option] username`
  `userdel username`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_41.png)
  ![Image](images/Screenshot_42.png)

- **apt-get**

  `apt-get [options] (command)`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_43.png)

- **nano, vi, jed**

   > editing text editors for Linux. If the target file does not exist, these editors will create one.
 
  `vi [filename]`
  `nano [filename]`
  `jed [filename]`
  
  ![Image](images/Screenshot_44.png)

- **alias, unalias**

   `alias Name=String`
   `unalias [alias_name]`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_45.png)

- **su**

  `su [options] [username [argument]]`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_46.png)

- **htop**

  `htop [options]`
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_47.png)

- **ps**
  > provides root priviledges to the user
  
  ![Image](images/Screenshot_48.png)







