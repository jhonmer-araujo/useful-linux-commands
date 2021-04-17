# useful-linux-commands
Some useful linux commands that can help us in the basic management of linux servers

## Size files, directories, disk space, space availables, etc:
- Show disk space usage: `df -h`
- Show the filesystem names, sizes and percentage of the used: `df -h --output=source,size,pcent`
- Show size of a directory: `du -sh /var`
- Show size of directories and first-level subdirectories: `du -shc /var/*`
- Show 5 largest directories within the a directory: `du -h /var/ | sort -rh | head -5`
