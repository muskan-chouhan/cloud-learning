### nano

Simple terminal text editor.

Syntax:
nano filename


Example:
nano notes.txt


Shortcuts:

- Ctrl + O → Save
- Enter → Confirm filename
- Ctrl + X → Exit

When to use:

Create or edit files directly from the terminal.

Real World Example:

```bash
sudo nano /etc/nginx/nginx.conf
```


Shortcut	Work
Ctrl + O	Save
Enter	Confirm filename
Ctrl + X	Exit
Ctrl + K	Cut line
Ctrl + U	Paste line
Ctrl + W	Search inside file



### vim

Powerful terminal text editor.

Syntax:
vim filename


Modes:

- Normal Mode → Default mode
- Insert Mode → Press `i` to type
- Command Mode → Press `Esc`, then use commands

Common Commands:

- `i` → Insert Mode
- `Esc` → Normal Mode
- `:w` → Save
- `:q` → Quit
- `:wq` → Save and Quit
- `:q!` → Quit without saving

Real World Example:

```bash
sudo vim /etc/nginx/nginx.conf
```

Used to edit server configuration files. 