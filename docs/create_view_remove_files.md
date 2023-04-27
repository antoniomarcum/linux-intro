## Working with files

### Create file with touch and nano

The `touch` command is used to create a new empty file. It takes a single
argument of the new file's name.

The `nano` command is used to edit a new or existing file. It takes the filename
as an argument. (Keep in mind absolute and relative paths)

While in the nano editor, use <ctrl-o> to write changes, and <ctrl-x> to quit
the editor.

Avoid using spaces or special characters when choosing a filename. Separate words
with hyphens or underscores. In Linux, a dot extension is chosen by the user.

e.g.
```
$ touch my_new_file.txt
# added .txt extension to convey it is a text file
```
Note that the dot extension is to make files more readable, but the extension
could be anything while the file contents are still only text.

### copy move, and remove

Use `cp` command to copy a file. This command takes two arguments, first the
name of file to be copied, second the name of new file.

Use `mv` command to move a file to a new location or rename a file, or both.
This command takes two arguments, the original filename and the new filename.
As with all these commands, both absolute and relative path options can be used.

Use `rm` command to remove a file. This command takes the filename as an argument.
This command will not usually ask for confirmation before deleting a file, so be
careful using it.

Use `rmdir` command to remove an **empty** directory. The command takes a single
argument of the directory. If there are files/directories inside the directory
to be deleted, then it fails.

## View permissions

Previously brought up the `ls` command. There are more uses than showing the
names of contents within a directory.

* `ls -l` provides a **long** listing of the files/directories.
