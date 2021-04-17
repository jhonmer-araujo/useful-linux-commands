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
