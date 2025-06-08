## Task 5: Practicing More Linux Commands

This task was about getting more comfortable with Linux commands by using them practically. I didn’t just memorize them — I tried them out, understood what they do, and how they might be useful while working on a real system. Here's a detailed list of what I practiced and how I understood each command:


### `uname -a`

This command shows a bunch of system details — the kernel name, version, machine type, and OS info all in one go. It's like asking “what exactly am I running right now?” Good for knowing the environment you're working in.


### `hostname`

This just tells me the name of the computer I'm on. If I’m connected to multiple systems or doing networking stuff, it helps identify which system I’m currently inside.


### `uptime`

Shows how long the system has been turned on. Also shows the load average — how busy the system has been. I used it to just get an idea of how long my virtual machine has been running.


### `whoami`

Literally tells “who am I” — shows which user I'm logged in as. Helpful when working in a system with multiple users or switching accounts using `sudo su`.


### `df -h`

This one shows the disk space usage of all partitions, but with `-h`, it gives sizes in MBs and GBs (human-readable), which is easier to understand. I used it to check how full my disk is.


### `du -sh <directory>`

Tells me how much space a particular folder is taking. I used this to check how heavy a directory was — the `-s` gives summary, and `-h` again makes it readable.


### `file <filename>`

It tells me what kind of file it is — plain text, binary, image, or something else. Useful when the file doesn’t have a clear extension or I’m unsure about its contents.


### `stat <filename>`

Shows more info about a file — like size, who owns it, when it was last modified or accessed. I used it to see timestamps and permission info in detail.


### `tree <directory>`

This one's cool — it shows a folder structure in the form of a tree. So instead of just `ls`, which lists files, this one shows nested folders and files clearly. Makes it easier to visualize a big project directory.


### `find <path> -name "<filename>"`

Used to search for files by name. Super helpful when I didn’t remember where a file was. You just give a path and the file name, and it finds all matches in subfolders too.

### `grep "word" <file>`

Searches for a word or line inside a file. For example, I used it to find if a specific config or value exists inside a file without opening it manually.

### `grep -r "word" <directory>`

Same as above, but works recursively — so it looks for that word in *all* files inside a folder. I used it when I didn’t know exactly where the text was saved.


### `top`

Live-updating version of `ps aux`. It shows the processes and refreshes every few seconds — kind of like Task Manager in Windows. I kept it open for a while to watch real-time CPU and RAM usage.

### `kill <PID>`

This is how I ended a program that was stuck. First, I used `ps aux` or `top` to get the PID (process ID), then used this to stop that specific process.


### `ping <hostname>`

Checks if a machine is reachable — like if the internet or a server is working. I used it to ping google.com and check my VM’s connectivity.


### `ifconfig`

Shows all network interfaces and their IP addresses. It's a bit old, but still found on some systems. Helped me check if my network was properly configured.


### `ip addr show`

This is the newer version of `ifconfig`. Shows the same kind of IP and interface details, but in a more modern format. I used both to compare the outputs.


### `unzip <archive.zip>`

This is only for `.zip` files. When I had a `.zip`, I used this to unpack it. It’s simple and worked without needing extra flags.


### `echo "text" > file.txt`

A quick way to create a file and write some text into it. I used it to make test files while checking other commands.


### `cat file.txt`

Displays what’s inside the file in one shot. Useful for small files, configs, or test outputs.

### `sort file.txt`

Arranges all the lines in the file alphabetically. I used it to sort some random data I had written using `echo`.



### `chmod 644 file.txt`

This changes the permissions of a file. 644 means the owner can read/write, and others can only read. I played with this to understand how file access is controlled.

### `chown user:group file.txt`

Changes the owner of the file. I tried this to understand how ownership works — for example, switching a file to another user or group.

### `history`

Shows all the commands I’ve typed before. Super helpful when I forgot a command I used earlier or wanted to repeat something quickly.

### `date`

Gives the current date and time from the system. I used it mostly to check if my VM’s clock was in sync.

