| Command | Description | Note | Version | Docs |
|:--- |:--- |:--- |:--- |:--- |
| `!!` | repeat the last entered bash command | | | |
| `!$` | repeat the last argument from the last bash command | | | |
| `&><file_name>` | redirect stdout and stderr to the given file by overriding it's previous content | | | |
| `&>><file_name>` | redirect stdout and stderr to the given file by appending to the file's end | | | |
| `1><file_name>` | redirect stdout to the given file by overriding it's previous content | | | |
| `2>dev/null` | discard all data sent to the stderr | | | |
| `<<file_name>` | redirect content of the given file to the stdin | | | |
| `<program_name> &>/dev/null &disown` | start program, detach stdin, stdout and stderr from the console and continue using terminal | | | |
| `<shell_variable_name>=<value>` | create shell variable in this session | | | |
| `>>word 2>&1` | redirect stdin and stderr to the given file by appending to the file's end | | | |
| `>word 2>&1` | redirect stdin and stderr to the given file by overriding it's content | | | |
| `[ -d /<directory_name> ] && echo 'Exist' \|\| echo 'Doesn't exist'` | test whether a directory exists | blank spaces around square brackets are mandatory | | |
| `[ -f <file_name> ] && echo 'Exist' \|\| echo 'Doesn't exist'` | test whether a file exists | blank spaces around square brackets are mandatory | | |
| `adduser <user_name>` | create a user | needs `sudo` | | |
| `apt autoremove` | remove all unused packages | needs `sudo` | | |
| `apt dist-upgrade` | upgrade packages by handling changes in the package dependencies | | | |
| `apt install -f` | install missing dependencies | needs `sudo` | | |
| `apt install <package_name>` | install package | needs `sudo` | | |
| `apt list --installed` | list packages installed with apt-get tool | | | [link](https://manpages.ubuntu.com/manpages/kinetic/man8/apt.8.html) |
| `apt list --upgradable` | list packages which update is available | | | [link](https://manpages.ubuntu.com/manpages/kinetic/man8/apt.8.html) |
| `apt policy` | list all available package repositories on the system | | | |
| `apt policy <package_name>` | show the package version and repository from where it was installed | | | |
| `apt purge <package_name>` | remove package and its configuration files | needs `sudo` | | |
| `apt show <package_name> -a` | show information about all available versions of the package in the repository | | | |
| `apt update` | update packages definitions | needs `sudo` | | |
| `apt upgrade` | upgrade the system by installing/upgrading packages | needs `sudo` | | |
| `apt-cache depends <package_name>` | show package dependencies | | | |
| `apt-cache pkgnames` | list all the packages in the cache | | | |
| `apt-cache policy \| grep http \| awk '{print $2" "$3}' \| sort -u` | list all repositories | | | |
| `apt-cache search <term>` | search of packages | | | |
| `apt-get install --reinstall <package_name>` | reinstall the package | needs `sudo` | | |
| `apt-get install ./<package_name>` | install the deb package | needs `sudo` | | |
| `apt-mark auto <package_name>` | mark package as automatically installed | package is marked as manually installed when it was installed with `apt install <package_name>` | | |
| `apt-mark showmanual` | list all of the manually installed packages from distribution packages | | | |
| `awk -F ':' '{print $1}' /etc/passwd` | list all of the users | | | |
| `cat /etc/environment` | list system-wide environment variables | | | |
| `cat /etc/group` | list all groups of the users | | | |
| `cat /etc/os-release` | display information about the operating system | | | |
| `cat /etc/passwd` | list all users with some additional information | | | |
| `cat /proc/meminfo` | information about the RAM memory | | | |
| `cd -` | go to the previously visited directory | | | |
| `chgrp group <file_name>` | change group ownership of the given file | | | |
| `chmod [ugoa][+-=][rwxXst] <file_name>` | change file permissions of the given file | | | |
| `chown <group_name>:<user_name> <file_name>` | change group and user permision of the given file | | | |
| `chown <user_name> <file_name>` | change the user owner of the file | | | |
| `compgen -g` | list all the groups of the users | | | |
| `compgen -v` | list all environment variables | | | |
| `cp <source> <destination>` | copy the file | | | |
| `date -d "<date_string> +<time>"` | calculate resulting date by adding specified time to a date | i.e. `date -d "18:48:00 2022-12-12 +1 hour 38 minutes"` gives us `20:26:00 2022-12-12` with default date formatting | | | 
| `declare -p` | list all shell variables | | | |
| `deluser --remove-home <user_name>` | needs `sudo`| deletes user with its home directory | | |
| `df -h` | display disk partition usage in human readable form | | | |
| `dmidecode -t 17 ` | hardware specification of the RAM chips | needs `sudo` | | |
| `do-release-upgrade` | update Ubuntu | | | |
| `dpkg -L <package_name>` | list where application puts its files | | | |
| `dpkg-deb -x <package_name>.deb <directory_name>` | unpack the package file | | | |
| `du -hs *` | display disk usage of the files and subdirectories in the current directory | | | |
| `echo $(($(getconf _PHYS_PAGES)* $(getconf PAGE_SIZE)/(1024*1024)))` | RAM size | | | |
| `echo $<variable_name>` | print shell variable's value | | | |
| `echo $?` | display return code of the last executed shell command | | | |
| `env` | list all shell variables with their values | | | |
| `export -p` | list all environment variables | | | |
| `export <variable_name>` | export shell variable so it can be used by the child processes | | | |
| `export <variable_name>=<value>` | export shell variable while setting its value so it can be used by the child processes | | | |
| `find . ! -name "<file_name>" -type f -delete` | delete all files from the current directory except the given file | | | |
| `find . -name <pattern> -delete` | delete all files which name matches a given pattern | | | |
| `find / -iname <pattern>` | list all files on the system which name matches the regular expression in a given pattern | search is case insensitive | | |
| `free -m` | display information about total, used and free RAM in MB | | | |
| `getconf -a` | list all configuration variables with their values | | | |
| `getent group` | list all groups of users | | | |
| `getent group <group_name>` | list all users of the given group | | | |
| `grep ^[^#] /etc/apt/sources.list /etc/apt/sources.list.d` | list all package repositories on the system | | | |
| `groupadd <group_name>` | create new group of users | needs `sudo` | | |
| `groupdel <group_name>` | delete a group of users | needs `sudo` | | |
| `groupmod --new-name <new_group_name> <old_group_name>` | rename a group of users | needs `sudo` | | |
| `groups <user_name>` | show all the groups that belongs a user with the given name | | | |
| `gsettings get <schema_name> <key>` | get a value for a given key of the given gnome settings schema | | | |
| `gsettings get org.gnome.shell favorite-apps` | list pinned program shorcuts in the gnome taskbar | | | |
| `gsettings list-keys <schema_name>` | list all the keys of the given gnome settings schema | | | |
| `gsettings list-recursively` | list all key-value pairs having the term | | | |
| `gsettings set <schema_name> <key> "['<value>]"` | set a value for a gnome setting key | | | |
| `gzip -dk <file_name>` | decompress a file while keep original compressed file | | | |
| `head -<n> <file_path>` | print the first n lines of the given file to the standard output | | | |
| `head <file_path>` | print the first 10 lines of the given file to the standard output | | | |
| `history` | list of previously used bash commands | | | |
| `history -d <number>` | delete the line from a history denoted with `<number>` | reenumerates the history after line deletion | | |
| `hostname -I` | display private IP address | | | |
| `ip add` | list IP adresses associated on all network interfaces | | | |
| `la -la \| grep "^d" && ls -la \| grep "^-" && ls -la \| grep "^l"` | display all the directories, files and links in that order | | | |
| `ldd <file_name>` | display shared library dependencies of the executable file or shared library | | | |
| `ln -s <file_path> <symbolic_link_path>` | create symbolic link | needs `sudo` | | |
| `ln <file1_name> <file2_name>` | create hard link `file2_name` that points to `file1_name` | changes in one file are reflected in the other | | |
| `ls -d1 */` | display list of subdirectories of the current directory | | | |
| `ls -ld .??*` | display hidden files in the current directory | | | |
| `ls -p \| grep -v /` | display files only in the current directory | | | |
| `ls /sys/class/net` | show the names of network interfaces | | | |
| `ls \| grep -v "<file_name>" \| xargs rm` | delete all files from the current directory except the given file | fails if the filename contains a space character | | |
| `lsb_release -a` | show information about Linux installation | | | 
| `lsblk` | list all disk and disk partitions | | | |
| `lsblk -o NAME,FSTYPE,SIZE,MOUNTPOINT,LABEL` | show information about hard disk partitions | needs `sudo` | | |
| `lscpu` | display information about the CPU architecture | | | |
| `lshw` | show system information | needs `sudo` | | |
| `lshw -c <class_name>` | show information about the hardware class | needs `sudo` | | |
| `mount` | show all mounted volumes | | | |
| `mv <file1_name> <file2_name> <destination_directory>` | move multiple files at once to the destination directory | | | 
| `mv <file1_path> <file2_path>` | move and/or rename a file | | | |
| `netstat -tulpn` | list all open ports; when used with `sudo` it displays programs listening on those ports | | | |
| `printenv` | list all environment variables | | | |
| `printenv <variable_name>` | print variable's value | | | |
| `printf %s "$(pwd)" \| xclip` | copy current directory path string to X clipboard without a new line at the end | needs `xclip` to be installed | | |
| `ps aux` | show status of every process on the system using BSD syntax | | | |
| `ps xf` | show status of the processes owned by the current user with the full format listing | | | |
| `pwd` | print current working directory | | | [link](https://www.gnu.org/software/bash/manual/bash.html#Bourne-Shell-Builtins) |
| `pwd \| xclip` | copy current directory path string to X clipboard with a new line at the end | needs `xclip` to be installed | | |
| `reboot` | restart the system | needs `sudo` | | |
| `rm -i <file_path>` | delete a file with prompting before a removal | | | |
| `rm -rf ~/.local/share/Trash/*` | empty the trash | | | |
| `sed -i '/s/<term1>/<term2>/g' <file_name>` | replace every occurence of the `<term1>` with the `<term2>` inside the given file | | | |
| `sed -i -re 's/([a-z]{2}\.)?archive.ubuntu.com\|security.ubuntu.com/old-releases.ubuntu.com/g' /etc/apt/sources.list` | change urls of the old Ubuntu repositories so packages can be updated | needs `sudo` | | [link](https://askubuntu.com/a/91821) |
| `set` | print all environment variables, shell variables and shell functions | | | |
| `set -o emacs` | use emacs keybindings | this is the default bash behavior | | | 
| `set -o posix ; set` | list all shell variables | | | |
| `set -o vi` | use vim keybindings | | | |
| `shutdown` | Schedule shut down event in one minute | needs `sudo` | | |
| `shutdown now` | Immediately shut down the system | needs `sudo` | | |
| `snap find <string>` | search snap packages | | | |
| `snap install <package_name>` | install a snap package | | | |
| `snap install <package_name>` | install a snap package | needs `sudo` | | |
| `snap list` | list installed snap packages | | | |
| `snap refresh` | update all snap packages | needs `sudo` | | |
| `snap remove <package_name>` | uninstall snap package | needs `sudo` | | |
| `source <file_name>` | execute shell script | file have to be executable shell file | | |
| `su` | switch to the `root` user | needs `sudo` | | |
| `su - <user_name>` | switch the user | | | |
| `su <user_name>` | switch the user while keeping the environment of the current one | | | |
| `sudo -i` | switch to the `root` user | by switching to the `root` user this way, one does not have to know the `root` account password | | |
| `sudo -s` | switch to the `root` user while keeping the environment of the current one | | | |
| `sudo <command>` | temporally grant the administrative rights of the `root` account | needs to be used only on restricted commands | | | 
| `systemctl disable <service_name>.service` | disable service from starting on the next boot | needs `sudo` | | |
| `systemctl enable <service_name>.service` | enable service to start on the next boot | needs `sudo` | | |
| `systemctl hibernate` | hibernate the system | | | |
| `systemctl list-dependencies <service_name>.service` | list dependencies of the service | | | |
| `systemctl list-unit-files --type service --state enabled` | list services starting on the next boot | | | |
| `systemctl list-units --type service --state running` | list services currently running | | | |
| `systemctl reload <service_name>.service` | restart the service without reloading its configuration | | | |
| `systemctl restart <service_name>.service` | restart the service with reloading its configuration | | | |
| `systemctl show <service_name>.service` | show properties of the the service | | | |
| `systemctl start <service.name>.service` | start the service | needs `sudo` | | |
| `systemctl start <service_name>.service` | activate the service | | | |
| `systemctl status <service_name>.service` | service status | | | |
| `systemctl stop <service_name>.service` | deactivate the service | | | |
| `systemctl suspend` | suspend the system | | | |
| `tail <file_path>` | print the last 10 lines of the given file to the standard output | | | |
| `tail <file_path>` | print the last 10 lines of the given file to the standard output | | | |
| `tar xjf <file_name>` | decompress a `tar.bz2` archive file | | | |
| `tar xzf <file_name>` | decompress a `tar.gz` archive file | | | |
| `test -f <file_name> && echo 'Exist' \|\| echo 'Doesn't exist'` | test whether a file exists | blank spaces around square brackets are mandatory | | |
| `time <bash_command>` | show time needed for the execution of the given bash command | | | |
| `touch <file_name>` | create empty file with the given name | | | |
| `uname -a` | Linux kernel version with some more system information | | | |
| `uname -r` | Linux kernel version | | | |
| `unset <variable_name>` | delete environment variable | | | |
| `update-alternatives --config <command>` | choose alternative program to be run by the command | needs `sudo` | | |
| `update-alternatives --install <link> <command> <path> <priority>` | install alternative program designated by the `<path>` to be run by the executable designated by `<link>` giving it a priority rank among all the alternatives | needs `sudo` | | |
| `useradd -s /bin/false -g <group_name> -m <user_name>` | create user that cannot be logged from the terminal | needs `sudo` | | |
| `userdel -u <user_name>` | delete user and their home directory | needs `sudo` | | |
| `usermod -aG <group_name> <user_name>` | add a user to a group | needs `sudo` | | |
| `usermod -l <new_user_name> <old_user_name>` | change the username of a user | | | |
| `vmstat -s` | display info about virtual memory, interrupts and CPU activity | | | |
| `whereis <command>` | display paths of the program | | | |
| `which <file_path>` | show executable file's path | | | |
| `xkill` | kill chosen program by mouse click | useful when program is not responding; after entering command, the `x` mouse pointer is shown with which one chooses program to close | | |
