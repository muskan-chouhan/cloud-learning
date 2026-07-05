### grep

Searches for a specific word or pattern inside a file.


### Common grep Options

grep -i word file - Ignore case while searching.

grep -n word file - Show line numbers.

grep -v word file - Show lines that do NOT match.

grep -r word folder - Search recursively inside folders.


### find

Searches files and directories.

Syntax:

find . -name "notes.txt"

Root directory:
find / -name "nginx.conf"


Search all .txt files:
find . -name "*.txt"


Search only files:
find . -type f


Search only directories:
find . -type d


Search .conf files:
find /etc -type f -name "*.conf"


Explanation:

- `.` → Current directory
- `/` → Root directory
- `-name` → Search by name
- `*` → Wildcard (anything)
- `-type f` → Files only
- `-type d` → Directories only

Real World Example:

```bash
find /etc -type f -name "*.conf"
```

Used to find configuration files.


### locate

Searches files using a database.

Syntax:

locate filename


Difference:

- find → Real-time search
- locate → Database search (Fast)

When to use:

Quickly find files by name.


### which

Shows the location of an executable command.

Syntax:
which command_name

Examples:
