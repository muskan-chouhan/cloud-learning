# Day 4 - File System Navigation

## Navigation Commands

### pwd - Print Working Directory

Shows the current directory path.

### ls

Lists files and directories.

Useful options:

* ls -a → Show hidden files.
* ls -l → Long listing format.
* ls -la → Hidden + Long listing.
* ls -lh → Human readable file size.

### cd

Change directory.

Move one level up.

## Path Types

### Absolute Path

Starts from Root (/).

Example:

/home/ubuntu/project

### Relative Path

Starts from the current directory.

Examples:

cd project

cd ..

cd ../..

---

## Directory Management

### mkdir

Create a directory.

### mkdir -p

Create nested directories.

Example:

mkdir -p dir1/dir2/dir3

---


## File Creation

### touch

Create an empty file.

Example:

touch file1.txt

Can also update file timestamps.

### cat

Displays the contents of a file.

Examples:

cat notes.txt   - read files

cat > notes.txt - add content

cat >> notes.txt - add more content

cat file1.txt file2.txt > output.txt          -also combine multiple files.


When to use:

View, create, or append content to a file.



### cp

Copy files and directories.

Example:

cp file1.txt file2.txt

Copy directory:

cp -r project backup

When to use:

Create a backup or duplicate files/folders.

### mv

Move or rename files and directories.

Examples:

mv file1.txt file2.txt

mv notes.txt backup/

When to use:

Move or rename files and folders.


## File Viewing Commands
### head

### head  -n 

Display first 10 lines.

### less

View large files page by page.
Navigation:

Space → Next page

b → Previous page

q → Quit


### tail

Display last 10 lines.

tail -f = fall (continue update lines show)
Ctrl + C -exit

### more

View content page by page.

## Delete Operations

### rm

Delete files.

### rm -r     >folder ke ander folder delete

Delete directories recursively. 

### rm -f

Force delete


## rm -rf  > dangerous 


### rmdir

Remove empty directory.

### rmdir -p

Remove parent and child empty directories.



# echo
Displays text on the terminal.

# clear
Clears the terminal screen.

# history
Shows previously executed commands.

# man  >manual
Shows the manual (documentation) of a command.
---



