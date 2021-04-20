# Some useful linux basic commands
That can help us in the basic management of linux servers

## Files and directories:
- Go to root directory: `cd /`
- Move on level up: `cd ..`
- Join 2 files and store the output in a new file: `cat file1 file2 > file3`
- Move a file to a new location: `mv file directory`
- Rename a file: `mv filename newfilename`
- Delete a file: `rm file`
- Creates a new directory: `mkdir directory`
- Delete a directory and his content: `rm -rf directory`
- List order by date: `ls -ltr`
- List order by extension: `ls -X`
- List including hidden: `ls -a`
- List including complete information: `ls -lh`
- Returns the contents of all subdirectories recursively: `ls -R`
- List sort the results by file size: `ls -S`
- Show the most recent modified file or directory: `ls -ltr | tail -n 1`
- Change owner and group to file or directory: `chown user:group file`
- Change permissions to file or directory: `chmod 644 file`
- 

## Size files and directories, disk space, space available, etc:
- Show disk space usage: `df -h`
- Show the filesystem names, sizes and percentage of the used: `df -h --output=source,size,pcent`
- Show size of a directory: `du -sh directory`
- Show size of directories and first-level subdirectories: `du -shc directory*`
- Show 5 largest directories within the a directory: `du -h directory | sort -rh | head -5`

## Managment and monitoring performance
- Display all the running and active real-time processes in ordered list: `top`
- Like `top` but with a friendly interface: `htop`
- Show statistics of virtual memory, kernel threads, disks, processes, interrupts, CPU activity and more `vmstat`
- Display list of all the open files, processes, disk files, network sockets, pipes, devices, etc: `lsof`
- Like `lsof` but specificing a network port: `lsof -i :80`
- Analize network packagets that received or transferred on a specific interface over a network: `tcpdump -i eth0`
- Monitoring incoming and outgoing network packets statistics as well as interface statistics: `netstat -a | more`
- Show system input and output storage device statistics: `iostat`
- Gives free RAM on the system: `free`
- Gives a list of all past commands typed in the current terminal session: `history`
- Gives information on all logged user: `finger username`
- Create a user: `adduser username`
- Connect to remote server using ssh: `ssh username@ipaddress`
- Show processes of a description given: `ps -aux | grep 'description'`
- Kill a process of a PID given: `Kill -9 PID`
