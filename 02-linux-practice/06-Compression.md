### zip

Compresses files and folders into a single ZIP archive.

Syntax:

```bash
zip -r archive.zip folder_name
```

Example:

```bash
zip -r project.zip project
```

Options:

- `-r` → Include all files and subfolders recursively.

When to use:

- Backup
- Deployment
- Sharing multiple files
- Project archive

Real World Example:

```bash
zip -r website.zip website
```

### unzip

Extracts files and folders from a ZIP archive.

Syntax:

```bash
unzip archive.zip
```

Example:

```bash
unzip project.zip
```

When to use:

- Extract project files
- Restore backups
- Open ZIP archives

Real World Example:

```bash
unzip backup.zip
```


### tar

Creates an archive of files and folders.

Syntax:

```bash
tar -cvf archive.tar folder_name
```

Example:

```bash
tar -cvf project.tar project
```

Options:

- `-c` → Create archive
- `-v` → Show files while creating
- `-f` → Archive file name

Difference:

- zip → Compress + Archive
- tar → Archive only

When to use:

Create backups and package multiple files.

### gzip

Compresses a file to reduce its size.

Syntax:

```bash
gzip filename
```

Example:

```bash
gzip backup.tar
```

Decompress:

```bash
gunzip backup.tar.gz
```

Difference:

- tar → Creates an archive.
- gzip → Compresses a file.

Real World Example:

```bash
tar -cvf backup.tar website
gzip backup.tar
```

Output:

```text
backup.tar.gz
```


#exract
tar -xzf backup.tar.gz