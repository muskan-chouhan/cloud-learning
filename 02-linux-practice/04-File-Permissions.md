### whoami

Displays the current logged-in user.

### id

Check complete information about the current user.

Shows:

- User ID (UID)
- Group ID (GID)
- Groups         > Displays the groups of the current user.



### chmod (Symbolic Method)

u = User (Owner)

g = Group

o = Others

a = All

+ = Add permission

- = Remove permission


Add or remove permissions from files and directories.



### chmod (Numeric Method)

Permission Values:

r = 4

w = 2

x = 1

Common Permissions:

777 = rwxrwxrwx

755 = rwxr-xr-x

644 = rw-r--r--

600 = rw-------

700 = rwx------

### chown

Changes the owner and group of a file or directory.

Examples:

sudo chown ubuntu file.txt

sudo chown ubuntu:ubuntu file.txt

When to use:

Change file ownership.

### umask  > user mask > umask future me banne wali files ke liye rule set karta hai.

Displays or sets the default permission mask for new files and directories.

When to use:

Control default permissions of newly created files and directories.

Owner se kuch mat hatao (0)
Group se Write hata do (2)
Others se Write hata do (2)


### sudo  >Temporarily runs ONE command with administrator privileges.

Full Form:

Super User DO

Runs a command with root (administrator) privileges.

Examples:

sudo apt update

sudo apt install nginx

sudo systemctl restart nginx

sudo chown ubuntu:ubuntu file.txt

### groups

Displays the groups of the current user.


Example Output:

```text
ubuntu adm cdrom sudo dip lxd
```

Common Groups:

- ubuntu → Default user group
- adm → System log access
- sudo → Administrator privileges
- dip → Networking related permissions
- lxd → Linux container management

Difference:

- whoami → Shows current username.
- id → Shows username, UID, GID and groups.
- groups → Shows only group names.

When to use:

Check which groups the current user belongs to.


which git
which ssh
which ls

Example Output:
/usr/bin/git


When to use:
Check where a command is installed.

### whereis

Shows the location of a command's executable, source, and manual files.

Syntax:
whereis command_name

Examples:
whereis git
whereis ssh
whereis ls


Difference:

- which → Shows executable path only.
- whereis → Shows executable, source (if available), and manual page.

When to use:

Get more information about a command's location.
