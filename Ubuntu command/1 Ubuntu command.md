
### File and Directory Management

- `ls` – List directory contents
- `cd` – Change directory
    - Example: `cd /home/user/Documents`
- `pwd` – Print working directory (shows the current directory path)
- `mkdir` – Create a directory
    - Example: `mkdir new_folder`
- `rmdir` – Remove empty directory
    - Example: `rmdir old_folder`
- `rm` – Remove files or directories
    - Example: `rm file.txt` (removes file)
    - Example: `rm -r folder_name` (removes folder recursively)
- `cp` – Copy files or directories
    - Example: `cp file1.txt file2.txt`
    - Example: `cp -r source_folder/ destination_folder/` (copy directories)
- `mv` – Move or rename files and directories
    - Example: `mv oldname.txt newname.txt`
    - Example: `mv file.txt /path/to/destination/`
- `touch` – Create a new empty file
    - Example: `touch newfile.txt`

### File Viewing and Editing

- `cat` – Display the contents of a file
    - Example: `cat file.txt`
- `less` – View content of a file with scrollable pages
    - Example: `less file.txt`
- `nano` – Open a file in the Nano text editor
    - Example: `nano file.txt`
- `vim` – Open a file in the Vim text editor
    - Example: `vim file.txt`
- `head` – Display the first few lines of a file
    - Example: `head file.txt`
- `tail` – Display the last few lines of a file
    - Example: `tail -n 20 file.txt` (last 20 lines)

### Process Management

- `ps` – Display currently running processes
    - Example: `ps aux` (shows all processes)
- `top` – Monitor system resources and processes interactively
- `kill` – Kill a process by PID
    - Example: `kill 1234` (where 1234 is the process ID)
- `killall` – Kill processes by name
    - Example: `killall firefox`
- `htop` – Interactive process viewer (must be installed first)

### System Information

- `df` – Display disk space usage
    - Example: `df -h` (human-readable format)
- `du` – Display disk usage of files and directories
    - Example: `du -sh directory_name` (summary in human-readable format)
- `free` – Display memory usage
    - Example: `free -h`
- `uname -a` – Show system information (kernel version, OS, etc.)
- `uptime` – Show how long the system has been running
- `top` – View system resource usage (CPU, memory, etc.)

### Package Management (using APT for Ubuntu)

- `apt update` – Update package list from repositories
- `apt upgrade` – Upgrade all upgradable packages
- `apt install <package>` – Install a package
    - Example: `apt install vim`
- `apt remove <package>` – Remove a package
    - Example: `apt remove vim`
- `apt purge <package>` – Remove a package and its configuration files
    - Example: `apt purge vim`
- `apt search <package>` – Search for a package
- `dpkg -l` – List installed packages

### User Management

- `adduser` – Add a new user
    - Example: `adduser newuser`
- `passwd` – Change user password
    - Example: `passwd username`
- `userdel` – Delete a user
    - Example: `userdel username`
- `usermod` – Modify a user's properties (e.g., change user group)
    - Example: `usermod -aG sudo username` (adds a user to the sudo group)

### Network Commands

- `ping` – Send ICMP packets to test connectivity
    - Example: `ping google.com`
- `ifconfig` – Display network interfaces and configurations
    - Example: `ifconfig`
- `ip a` – Show all IP addresses and network interfaces
- `netstat` – Display network connections and statistics
    - Example: `netstat -tuln`
- `curl` – Transfer data from or to a server (useful for downloading files)
    - Example: `curl -O http://example.com/file.txt`
- `wget` – Download files from the internet
    - Example: `wget http://example.com/file.txt`

### File Permissions

- `chmod` – Change file permissions
    - Example: `chmod 755 file.txt` (gives execute permission to owner)
- `chown` – Change file owner or group
    - Example: `chown user:group file.txt`
- `chgrp` – Change group ownership of a file
    - Example: `chgrp groupname file.txt`

### Disk Management

- `mount` – Mount a filesystem or device
    - Example: `mount /dev/sdb1 /mnt/usb`
- `umount` – Unmount a filesystem or device
    - Example: `umount /mnt/usb`
- `fdisk` – Disk partitioning tool
    - Example: `fdisk -l` (list all partitions)