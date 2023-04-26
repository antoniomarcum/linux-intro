## Linux directory structure

Linux uses an "upside-down" tree directory structure. The filesystem
always starts at root, denoted "/" (forward-slash).

Under root, there are many other directories and files which are separated by
"/"s (forward-slashes).

e.g.
```
/users/project/username
```

```
/
|_ users/
  |_ <project>/
    |_ <user1>/
    |_ <user2>/
```

### Home directory

Each user is granted their own home directory path which they can use to store
files. This is where a user will be by default when starting a session.


## Hands-on CLI

Visit [OSC ondemand](https://ondemand.osc.edu) and login with your OSC username
and password.

After logging in, use the top navigation bar to select **Clusters**, then click
**Pitzer shell**. This will open a new tab showing a command line interface (CLI)
and a bash shell will start.

### ls and mkdir

Use ls command to 'list' the contents of a directory.

Use mkdir to 'make directory'. This command takes and argument of the new
directory name.

```
$ ls
# displays contents
$ mkdir my-new-dir
# creates a new directory
```

### pwd and cd commands

The first two commands to try are pwd and cd.

Use pwd to 'print working directory'. The working directory is the directory you
are currently in.

Use cd to 'change directory'. This command takes an argument of the directory
name to change to.

```
$ pwd
# print current directory
$ cd <dir-name>
# change directory to <dir-name>
```

### Directory absolute/relative paths and shorthands

Directories can be identified by an **absolute** path, meaning that the entire
path from root down is written.

e.g. `/fs/ess/PZS1132`

Another way to navigate the directory structure is using **relative** paths. A
relative path prepends the current working directory (cwd) to the path entered.

e.g. (Assume cwd is `/users/PZS1132`)
```
$ cd <username>
# will be interpreted as "cd /users/PZS1132/<username>"
```

If there is no leading forward-slash, then the directory is interpreted as
**relative**. If there is, then the directory path is starting a root, and needs
to be **absoulte**.

Finally, there are some shorthands that can be useful.

* `cd` command with no arguments sets cwd to home directory.
* `$HOME` or `~` is shorthand for the current user's home directory

## Commands list

* ls
* mkdir
* pwd
* cd
