| Command | Description | Note | Version | Docs |
|:--- |:--- |:--- |:--- |:--- |
| `&><file_name>` | redirect stdout and stderr to the given file by overriding it's previous content | | 5.0.3 | |
| `&>><file_name>` | redirect stdout and stderr to the given file by appending to the file's end | | 5.0.3 | |
| `1><file_name>` | redirect stdout to the given file by overriding it's previous content | | 5.0.3 | |
| `2>dev/null` | discard all data sent to the stderr | | 5.0.3 | |
| `<<file_name>` | redirect content of the given file to the stdin | | 5.0.3 | |
| `<program_name> &>/dev/null &disown` | start program, detach stdin, stdout and stderr from the console and continue using terminal | | 5.0.3 | |
| `<shell_variable_name>=<value>` | create shell variable in this session | | 5.0.3 | |
| `>>word 2>&1` | redirect stdin and stderr to the given file by appending to the file's end | | 5.0.3 | |
| `>word 2>&1` | redirect stdin and stderr to the given file by overriding it's content | | 5.0.3 | |
| `[ -d /<directory_name> ] && echo 'Exist' \|\| echo 'Doesn't exist'` | test whether a directory exists | blank spaces around square brackets are mandatory | 5.0.3 | |
| `[ -f <file_name> ] && echo 'Exist' \|\| echo 'Doesn't exist'` | test whether a file exists | blank spaces around square brackets are mandatory | 5.0.3 | |
| `adduser <user_name>` | create a user | needs `sudo` | 5.0.3 | |
| `apt autoremove` | remove all unused packages | needs `sudo` | 5.0.3 | |
| `apt dist-upgrade` | upgrade packages by handling changes in the package dependencies | | 5.0.3 | |
| `apt install -f` | install missing dependencies | needs `sudo` | 5.0.3 | |
| `apt install <package_name>` | install package | needs `sudo` | 5.0.3 | |
| `apt list --installed` | list packages installed with apt-get tool | | 5.0.3 | [link](https://manpages.ubuntu.com/manpages/kinetic/man8/apt.8.html) |
| `apt list --upgradable` | list packages which update is available | | 5.0.3 | [link](https://manpages.ubuntu.com/manpages/kinetic/man8/apt.8.html) |
| `apt policy` | list all available package repositories on the system | | 5.0.3 | |
| `apt policy <package_name>` | show the package version and repository from where it was installed | | 5.0.3 | |
| `apt purge <package_name>` | remove package and its configuration files | needs `sudo` | 5.0.3 | |
| `apt update` | update packages definitions | needs `sudo` | 5.0.3 | |
| `apt upgrade` | upgrade the system by installing/upgrading packages | needs `sudo` | 5.0.3 | |
| `apt-cache depends <package_name>` | show package dependencies | | 5.0.3 | |
| `apt-cache pkgnames` | list all the packages in the cache | | 5.0.3 | |
| `apt-cache policy \| grep http \| awk '{print $2" "$3}' \| sort -u` | list all repositories | | 5.0.3 | |
| `apt-cache search <term>` | search of packages | | 5.0.3 | |
| `apt-get install --reinstall <package_name>` | reistall the package | needs `sudo` | 5.0.3 | |
| `apt-get install ./<package_name>` | install the deb package | needs `sudo` | 5.0.3 | |
| `apt-mark showmanual` | list all of the manually installed packages from distibution packages | | 5.0.3 | |
| `awk -F ':' '{print $1}' /etc/passwd` | list all of the users | | 5.0.3 | |
| `cat /etc/environment` | list system-wide enviroment variables | 5.0.3 | |
| `cat /etc/group` | list all groups of the users | | 5.0.3 | |
| `cat /etc/os-release` | display information about the operating system  | | 5.0.3 | |
| `cat /etc/passwd` | list all users int the format `user_name:encrypetd_pswd:UID:GID:full_name:home_directory:login_shell` | | 5.0.3 | |
| `cat /proc/meminfo` | information about the RAM memory | | 5.0.3 | |
| `cd -` | go to the previously visited directory | | 5.0.3 | |
| `chgrp group <file_name>` | change group ownership of the given file | | 5.0.3 | |
| `chmod [ugoa][+-=][rwxXst] <file_name>` | change file permissions of the given file | | 5.0.3 | |
| `chown <group_name>:<user_name> <file_name>` | change group and user permmision of the given file | | 5.0.3 | |
| `chown <user_name> <file_name>` | change the user owner of the file | | 5.0.3 | |
| `compgen -g` | list all the groups of the users | | 5.0.3 | |
| `compgen -v` | list all enviroment variables | | 5.0.3 | |
| `cp <source> <destionation>` | copy the file | | 5.0.3 | |
| `declare -p` | list all shell variables | 5.0.3 | |
| `deluser --remove-home <user_name>` | needs `sudo`; delete user with its home directory | 5.0.3 | |
| `df -h` | display disk partition usage in human readable form | | 5.0.3 | |
| `dmidecode -t 17 ` | hardware specification of the RAM chips | needs `sudo` | 5.0.3 | |
| `do-release-upgrade` | update Ubuntu | | 5.0.3 | |
| `dpkg -L <package_name>` | list where application puts its files | | 5.0.3 | |
| `dpkg-deb -x <package_name>.deb <directory_name>` | unpack the package file | | 5.0.3 | |
| `du -hs *` | display disk usage of the subdirectories in the current directory  | | 5.0.3 | |
| `echo $(($(getconf _PHYS_PAGES)* $(getconf PAGE_SIZE)/(1024*1024)))` | RAM size | | 5.0.3 | |
| `echo $<variable_name>` | print shell variable's value | 5.0.3 | |
| `echo $?` | display return code of the last executed shell command | | 5.0.3 | |
| `env` | list all shell variables with their values | | 5.0.3 | |
| `export -p` | list all enviroment variables | | 5.0.3 | |
| `export <variable_name>` | export shell variable so it can be used by the child proccesses | 5.0.3 | |
| `export <variable_name>=<value>` | export shell variable while setting its value so it can be used by the child proccesses | 5.0.3 | |
| `find . ! -name "<file_name>" -type f -delete` | delete all files from the current directory except the given file | | 5.0.3 | |
| `find . -name <pattern> -delete` | delete all files which name matches a given pattern | | 5.0.3 | |
| `find / -iname <pattern>` | list all files on the system which name mathes the regular expression in a given pattern | search is case insensitive | 5.0.3 | |
| `free -m` | display information about total, used and free RAM in MB | | 5.0.3 | |
| `getconf -a` | list all configuration variables with their values | | 5.0.3 | |
| `getent group` | list all groups of users | | 5.0.3 | |
| `getent group <group_name>` | list all users of the given group | | 5.0.3 | |
| `groupadd <group_name>` | create new group of users | needs `sudo` | 5.0.3 | |
| `groupdel <group_name>` | delete a group of users | needs `sudo` | 5.0.3 | |
| `groupmod --new-name <new_group_name> <old_group_name>` | rename a group of users | needs `sudo` | 5.0.3 | |
| `groups <user_name>` | show all the groups that belongs a user with the given name | | 5.0.3 | |
| `gsettings get <schema_name> <key>` | get a value for a given key of the given gnome settings schema | | 5.0.3 | |
| `gsettings get org.gnome.shell favorite-apps` | list pinned program shorcuts in the gnome taskbar | | 5.0.3 | |
| `gsettings list-keys <schema_name>` | list all the keys of the given gnome settings schema | | 5.0.3 | |
| `gsettings list-recursively` | list all key-value pairs having the term | | 5.0.3 | |
| `gsettings set <schema_name> <key> "['<value>]"` | set a value for a gnome setting key | | 5.0.3 | |
| `gzip -dk <file_name>` | decompress a file while keep original compressed file | | 5.0.3 | |
| `head -<n> <file_path>` | print the first n lines of the given file to the standard output | | 5.0.3 | |
| `head <file_path>` | print the first 10 lines of the given file to the standard output | | 5.0.3 | |
| `history` | list of previously used bash commands | | 5.0.3 | |
| `history -d <number>` | delete the line from a history denoted with <number> | renumerates the history after line deletion | 5.0.3 | |
| `hostname -I` | display private IP address | | 5.0.3 | |
| `ip add` | list IP adresses associated on all network interfaces | | 5.0.3 | |
| `la -la \| grep "^d" && ls -la \| grep "^-" && ls -la \| grep "^l"` | display all the directories, files and links in that order | | 5.0.3 | |
| `ldd <file_name>` | display shared library dependencies of the executable file or shared library | | 5.0.3 | |
| `ln -s <file_path> <symbolic_link_path>` | create symbolic link | needs `sudo` | 5.0.3 | |
| `ln <file1_name> <file2_name>` | create hard link `file2_name` that points to 'file1_name' | changes in one file are reflected in the other | 5.0.3 | |
| `ls -d1 */` | display list of directories int the current directory | | 5.0.3 | |
| `ls -ld .??*` | display hidden files in the current directory | | 5.0.3 | |
| `ls -p \| grep -v /` | display files only in the current directory | | 5.0.3 | |
| `ls \| grep -v "<file_name>" \| xargs rm` | delete all files from the current directory except the given file | fails if the filename contains a space character | 5.0.3 | |
| `lsb_release -a` | show information about Linux installation | | 5.0.3 | 
| `lsblk` | list all disk and disk partitions | | 5.0.3 | |
| `lsblk -o NAME,FSTYPE,SIZE,MOUNTPOINT,LABEL` | show infromation about hard disk partitions | needs `sudo` | 5.0.3 | |
| `lscpu` | display information about the CPU architecture | | 5.0.3 | |
| `lshw` | show system information | needs `sudo` | 5.0.3 | |
| `lshw -c <class_name>` | show information about the hardware class | needs `sudo` | 5.0.3 | |
| `mv <file1_name> <file2_name> <destination_directory>` | move multiple files at once to the destination directory | | 5.0.3 | 
| `mv <file1_path> <file2_path>` | move and/or rename a file | | 5.0.3 | |
| `printenv` | list all enviroment variables | 5.0.3 | |
| `printenv <variable_name>` | print variable's value | 5.0.3 | |
| `printf %s "$(pwd)" \| xclip` | copy current directory path string to X clipboard without a new line at the end | needs xclip to be installed | 5.0.3 | |
| `ps aux` | show status of every process on the system using BSDD syntax  | | 5.0.3 | |
| `ps xf` | show status of the processes owned by the current user with the full format listing  | | 5.0.3 | |
| `pwd` | print current working directory | | 5.0.3. | [link](https://www.gnu.org/software/bash/manual/bash.html#Bourne-Shell-Builtins) |
| `pwd \| xclip` | copy current directory path string to X clipboard with a new line at the end | needs xclip to be installed | 5.0.3 | |
| `reboot` | restatt the system | needs `sudo` | 5.0.3 | |
| `rm -i <file_path>` | delete a file with prompting before a removal | | 5.0.3 | |
| `rm -rf ~/.local/share/Trash/*` | empty the trash | | 5.0.3 | |
| `sed -i '/s/<term1>/<term2>/g' <file_name>` | replace every occurence of the term1 with the term2 inside the given file | | 5.0.3 | |
| `sed -i -re 's/([a-z]{2}\.)?archive.ubuntu.com\|security.ubuntu.com/old-releases.ubuntu.com/g' /etc/apt/sources.list` | change urls of the old Ubuntu repositories so packages can be updated | needs `sudo` | 5.0.3 | [link](https://askubuntu.com/a/91821) |
| `set` | print all enviroment variables, shell variables and shell functions | 5.0.3 | |
| `set -o posix ; set` | list all shell variables | 5.0.3 | |
| `snap find <string>` | search snap packages | | 5.0.3 | |
| `snap install <package_name>` | install a snap package | | 5.0.3 | |
| `snap install <package_name>` | install a snap package | needs `sudo` | 5.0.3 | |
| `snap list` | list installed snap packages | | 5.0.3 | |
| `snap refresh` | update all snap packages | needs `sudo` | 5.0.3 | |
| `snap remove <package_name>` | uninstall snap package | needs `sudo` | 5.0.3 | |
| `source <file_name>` | execute shell script | file have to be executable shell file | 5.0.3 | |
| `su` | switch to the root user | needs `sudo` | 5.0.3 | |
| `su - <user_name>` | swith the user | 5.0.3 | |
| `su <user_name>` | switch the user while keeping the environment of the current one | | 5.0.3 | |
| `sudo <command>` | temporaraly grant the administrative rights of the `root` account | needs to be used only on restricted commands | 5.0.3 | | 
| `systemctl disable <service_name>.service` | disable service from starting on the next boot | needs `sudo` | 5.0.3 | |
| `systemctl enable <service_name>.service` | enable service to start on the next boot | needs `sudo` | 5.0.3 | |
| `systemctl hibernate` | hibernate the system | | 5.0.3 | |
| `systemctl list-dependencies <service_name>.service` | list dependencies of the service | | 5.0.3 | |
| `systemctl list-unit-files --type service --state enabled` | list services starting on the next boot | | 6.0.3 | |
| `systemctl list-units --type service --state running` | list services currently running | | 5.0.3 | |
| `systemctl reload <service_name>.service` | restart the searvice without reloading its configuration | | 5.0.3 | |
| `systemctl restart <service_name>.service` | restart the service with reloading its configuration | | 5.0.3 | |
| `systemctl show <service_name>.service` | show properties of the the service | | 5.0.3 | |
| `systemctl start <service.name>.service` | start the service | needs `sudo` | 5.0.3 | |
| `systemctl start <service_name>.service` | activate the service | | 5.0.3 | |
| `systemctl status <service_name>.service` | service status | | 5.0.3 | |
| `systemctl stop <service_name>.service` | deactivate the service | | 5.0.3 | |
| `systemctl suspend` | suspend the system | | 5.0.3 | |
| `tail <file_path>` | print the last 10 lines of the given file to the standard output | | 5.0.3 | |
| `tail <file_path>` | print the last 10 lines of the given file to the standard output | | 5.0.3 | |
| `tar xjf <file_name>` | decompress a `tar.bz2` archive file | | 5.0.3 | |
| `tar xzf <file_name>` | decompress a `tar.gz` archive file | | 5.0.3 | |
| `test -f <file_name> && echo 'Exist' \|\| echo 'Doesn't exist'` | test whether a file exists | blank spaces around square brackets are mandatory | 5.0.3 | |
| `touch <file_name>` | create empty file with the given name | | 5.0.3 | |
| `uname -a` | Linux kernel version with some more system information | | 5.0.3 | |
| `uname -r` | Linux kernel version | | 5.0.3 | |
| `unset <variable_name>` | delete enviroment variable | | 5.0.3 | |
| `update-alternatives --config <command>` | choose alternative program to be run by the command | needs `sudo` | 5.0.3 | |
| `update-alternatives --install <link> <command> <path> <priority>` | install alternative programm designated by the `<path>` to be run by the executable designated by `<link>` giving it a priority rank among all the alternatives | needs `sudo` | 5.0.3 | |
| `useradd -s /bin/false -g <group_name> -m <user_name>` | create user that cannot be logged from the terminal | needs `sudo` | 5.0.3 | |
| `userdel -u <user_name>` | delete user and their home directory | needs `sudo` | 5.0.3 | |
| `usermod -aG <group_name> <user_name>` | add a user to a group | needs `sudo` | 5.0.3 | |
| `usermod -l <new_user_name> <old_user_name>` | change the username of a user | | 5.0.3 | |
| `vmstat -s` | dispay info about virtual memory, inerrupts and CPU activity | | 5.0.3 | |
| `whereis <command>` | display paths of the program | | 5.0.3 | |
| `which <file_path>` | show executable file's path | | 5.0.3 | |
