# Some useful linux commands
That can help us in the basic management of linux servers

## Show files and directories within the current directory:
- Order by date: `ls -ltr`
- Order by extension: `ls -X`
- Including hidden: `ls -a`
- Including complete information: `ls -lh`
- Returns the contents of all subdirectories recursively: `ls -R`
- Sort the results by file size: `ls -S`
- Show the most recent modified file or directory: `ls -ltr | tail -n 1`

## Show Size files and directories, disk space, space available, etc:
- Show disk space usage: `df -h`
- Show the filesystem names, sizes and percentage of the used: `df -h --output=source,size,pcent`
- Show size of a directory: `du -sh /var`
- Show size of directories and first-level subdirectories: `du -shc /var/*`
- Show 5 largest directories within the a directory: `du -h /var/ | sort -rh | head -5`

## Monitoring performance

- Display all the running and active real-time processes in ordered list: `top`
- Like `top` but with a friendly interface: `htop`
- Show statistics of virtual memory, kernel threads, disks, processes, interrupts, CPU activity and more `vmstat`
- Display list of all the open files, processes, disk files, network sockets, pipes, devices, etc: `lsof`
- Like `lsof` but specificing a network port: `lsof -i :80`
- Analize network packagets that received or transferred on a specific interface over a network: `tcpdump -i eth0`
- Monitoring incoming and outgoing network packets statistics as well as interface statistics: `netstat -a | more`
- Show system input and output storage device statistics: `iostat`
