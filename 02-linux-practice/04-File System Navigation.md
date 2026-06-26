# Day 4 - File System Navigation

## Navigation Commands

### pwd

Print Working Directory

Shows the current directory path.

### ls

Lists files and directories.

Useful options:

* ls -a → show hidden files
* ls -l → long listing format
* ls -al → hidden + long listing

### cd

Change directory.

Examples:

cd foldername

cd ..

Move one level up.

---

## Directory Management

### mkdir

Create a directory.

Example:

mkdir project

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

Create, view and combine files.

Examples:

cat file1.txt

cat > file1.txt

cat >> file1.txt

### tac

Display file contents in reverse order.

Example:

tac file1.txt

---

## Text Editors

### vi

Open file in vi editor.

Commands:

i → insert mode

:wq → save and quit

### nano

Simple text editor.

Save and exit:

Ctrl + X

Y

Enter

---

## Copy, Move and Rename

### cp

Copy files.

Example:

cp file1 file2

### mv

Move files or rename files.

Examples:

mv file1 folder/

mv old.txt new.txt

---

## Delete Operations

### rm

Delete files.

Example:

rm file1.txt

### rm -r

Delete directories recursively.

### rm -f

Force delete.

### rmdir

Remove empty directory.

### rmdir -p

Remove parent and child empty directories.

---

## File Viewing Commands

### less

View large files page by page.

### head

Display first 10 lines.

### tail

Display last 10 lines.

### more

View content page by page.

---

## Key Learning

Linux file system navigation involves moving between directories, creating files and folders, viewing content, copying, moving and deleting resources using terminal commands.


-----


## Path Types

### Absolute Path

Starts from Root (/).

Example

/home/ubuntu/project

### Relative Path

Starts from current directory.

Examples

cd project

cd ..

cd ../..