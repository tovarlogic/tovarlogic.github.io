---
title: "Linux: Comandos básicos"
date: 2022-04-01
categories:
  - Tecnología
tags:
  - Linux
lastmod: 2022-04-18T13:36:19.208Z
---
|**Purpose** | **Command** | **Description** |
| ---------- | ----------- | --------------- |
| **online man** | [link](https://www.kernel.org/doc/man-pages/) | official page  |
| **online man** | [link](https://man7.org/linux/man-pages/index.html) | official search  |
| **online man** | [link](https://linux.die.net/man/) | die.net|
| **online man** | [link](https://explainshell.com) | explainshell.com |
| **online man** | [link](https://man.cx/) | man.cx |
| **online tutorial** | [link](https://www.geeksforgeeks.org/linux-commands/) | geeksforgeeks.org |
| linux basic | `man <tool>` | Opens man pages for the specified tool. | 
| linux basic | `<tool> -h` | Prints the help page of the tool. | 
| linux basic | `apropos <keyword>` | Searches through man pages' descriptions for instances of a given keyword. | 
| linux basic | `cat` | Concatenate and print files. |
| system info  | `whoami` | Displays current username. | 
| system info  | `id` | Returns users identity. | 
| system info  | `hostname` | Sets or prints the name of the current host system. | 
| system info  | `uname` | Prints operating system name. | 
| system info  | `pwd` | Returns working directory name. | 
| network info  | `ifconfig` | The `ifconfig` utility is used to assign or view an address to a network interface and/or configure network interface parameters. | 
| network info  | `ip` | Ip is a utility to show or manipulate routing, network devices, interfaces, and tunnels. | 
| network info  | `netstat` | Shows network status. | 
| network info  | `ss` | Another utility to investigate sockets. | 
| processes info | `ps` | Shows process status. | 
| system info  | `who` | Displays who is logged in. | 
| system info  | `env` | Prints environment or sets and executes a command. | 
| system info  | `lsblk` | Lists block devices. | 
| system info  | `lsusb` | Lists USB devices. | 
| system info  | `lsof` | Lists opened files. | 
| system info  | `lspci` | Lists PCI devices. | 
| linux users | `sudo` | Execute command as a different user. | 
| linux users | `su` | The `su` utility requests appropriate user credentials via PAM and switches to that user ID (the default user is the superuser).  A shell is then executed. | 
| linux users | `useradd` | Creates a new user or update default new user information. | 
| linux users | `userdel` | Deletes a user account and related files. |
| linux users | `usermod` | Modifies a user account. | 
| linux users | `addgroup` | Adds a group to the system. | 
| linux users | `delgroup` | Removes a group from the system. | 
| linux users | `passwd` | Changes user password. |
| linux users | `chage` | change user password expiry information. |
| linux packages | `dpkg` | Install, remove and configure Debian-based packages. | 
| linux packages | `apt` | High-level package management command-line utility. | 
| linux packages | `aptitude` | Alternative to `apt`. | 
| linux packages | `snap` | Install, remove and configure snap packages. |
| linux packages | `gem` | Standard package manager for Ruby. | 
| linux packages | `pip` | Standard package manager for Python. |  
| system info | `systemctl` | Command-line based service and systemd control manager. |
| processes | `ps` | Prints a snapshot of the current processes. | 
| system info | `journalctl` | Query the systemd journal. | 
| processes | `kill` | Sends a signal to a process. | 
| processes | `bg` | Puts a process into background. |
| processes | `jobs` | Lists all processes that are running in the background. | 
| processes | `fg` | Puts a process into the foreground. | 
| network transfer | `curl` | Command-line utility to transfer data from or to a server. | 
| network transfer | `wget` | An alternative to `curl` that downloads files from FTP or HTTP(s) server. |
| network service | `python3 -m http.server` | Starts a Python3 web server on TCP port 8000. | 
| linux basic | `ls` | Lists directory contents. | 
| linux basic | `cd` | Changes the directory. |
| linux basic | `clear` | Clears the terminal. | 
| linux basic | `touch` | Changes file timestamps or creates an empty file. |
| linux basic | `mkdir` | Creates a directory. | 
| linux basic | `tree` | Lists the contents of a directory recursively. |
| linux basic | `mv` | Move or rename files or directories. | 
| linux basic | `cp` | Copy files or directories. |
| linux basic | `nano` | Terminal based text editor. | 
| linux basic | `which` | Returns the path to a executable file or link. |
| linux basic | `find` | Searches for files in a directory hierarchy. | 
| | `updatedb` | Updates the locale database for existing contents on the system. |
| linux basic | `locate` | Uses the locale database to find contents on the system. | 
| linux basic | `more` | Pager that is used to read STDOUT or files. |
| linux basic | `less` | An alternative to `more` with more features. | 
| linux basic | `head` | Prints the first N lines of STDOUT or a file. |
| linux basic | `tail` | Prints the last N lines of STDOUT or a file. | 
| linux basic | `sort` | Sorts the contents of STDOUT or a file. |
| linux basic | `grep` | Searches for specific results that contain given patterns. | 
| linux basic | `cut` | Removes sections from each line of files. |
| linux basic | `tr` | Replaces certain characters. | 
| linux basic | `column` | Command-line based utility that formats its input into multiple columns. |
| linux basic | `awk` | Pattern scanning and processing language. |
| linux basic | `sed` | A stream editor for filtering and transforming text. | 
| linux basic | `wc` | "word count". Prints newline, word, and byte counts for a given input. |
| premissions | `chmod` | Changes permission of a file or directory. |
| permissions | `chown` | Changes the owner and group of a file or directory. |