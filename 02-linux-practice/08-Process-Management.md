## Process

A running program in Linux is called a Process.

Examples:

- nginx
- mysql
- docker
- nano
- vim

Each process has a unique Process ID (PID).

---

## ps

Shows running processes.

Commands:
ps                    >  Current terminal ke processes
ps -ef                >  Almost saare processes (full format)
ps -u username        >  Sirf ubuntu user ke processes
ps aux                >  Sab users + detailed info + background processes
 a = All users
 u = User-oriented format
 x = Processes without terminal (TTY) bhi dikhao.
Examples:
ps -u ubuntu


Real World:
Used to check which processes are running on a Linux server.


## top

Displays live running processes and system resource usage.



Shows:
- PID
- USER
- CPU Usage
- Memory Usage
- Running Command

Exit:

Press `q`

Difference:

- `ps` → Snapshot
- `top` → Live monitoring

Real World:
Used to monitor CPU, RAM and running processes on production servers.

term
PR → Process priority.
NI → Nice value (CPU scheduling preference).
VIRT → Total virtual memory reserved.
RES → Actual physical RAM being used.
SHR → Shared memory with other processes.


## kill

Stops a running process using its PID.

Syntax: kill PID

Example: kill 1521

Default Signal:

- SIGTERM (15)
- Gracefully stops the process.

Force Stop: kill -9 PID

- SIGKILL (9)
- Immediately terminates the process.

Real World: Used to stop hung or unwanted processes.


## killall

Stops all processes with the same name.

Syntax: killall process_name

Example: killall python


Difference:
- kill → Uses PID
- killall → Uses Process Name

Real World: Used to stop multiple processes with the same name.


## jobs = Background jobs dikhao.

Shows background jobs in the current terminal.

## bg = Pause hui process ko background me chalao.

Continues a stopped process in the background.

## fg = Background process ko foreground me lao.

Brings a background process back to the foreground.


Flow:

Foreground → Ctrl+Z → Stopped → bg → Background → fg → Foreground

uses = 
Ctrl + Z = Pause (Stop) the current foreground process.
Ctrl + C = Process ko terminate (end) kar do.


Real World:

Used to manage long-running commands without opening a new terminal.