# Day 3 - Linux File System Hierarchy

## Linux File System Hierarchy

Linux organizes files and directories in a hierarchical structure starting from the root directory (/).

---

## /

The root directory.

All files and directories in Linux start from this location.

---

## /home

Home directories for normal users.

Example:

/home/nikita

---

## /root

Home directory of the root (administrator) user.

Example:

/root

---

## /boot

Contains boot-related files required to start the Linux operating system.

Examples:
- Kernel files
- Bootloader files

---

## /etc

Contains system configuration files.

Examples:
- Network configuration
- User configuration
- Service configuration

---

## /usr

Contains user applications and software installed on the system.

Many programs are stored here.

---

## /bin

Contains essential commands used by all users.

Examples:

- ls
- pwd
- cp
- mv

---

## /sbin

Contains system administration commands.

Generally used by the root user.

Examples:

- reboot
- shutdown
- fdisk

---

## /opt

Used for optional third-party software packages.

Example:

- Google Chrome
- Custom applications

---

## /dev

Contains device files.

Examples:

- Hard disks
- USB devices
- Terminal devices

In Linux, hardware devices are represented as files.

---

## Key Learning

Linux follows a hierarchical file system structure.

Important directories:

- /home → User home directories
- /root → Root user's home directory
- /boot → Boot files
- /etc → Configuration files
- /usr → Installed software
- /bin → Common commands
- /sbin → Administrative commands
- /opt → Optional software
- /dev → Device files