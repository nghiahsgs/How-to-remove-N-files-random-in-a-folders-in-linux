# How-to-remove-N-files-random-in-a-folders-in-linux
How to remove N files random in a folders in linux


To remove a random selection of N files in a folder in Linux, you can use the ls and head commands in combination with the rm command.

Here's an example command that will remove N random files from a folder:
```
ls | shuf -n N | xargs rm
```
Here's what each part of the command does:

```
ls: Lists all files in the current directory.
shuf -n N: Randomly selects N files from the list of files output by ls.
xargs rm: Passes the randomly selected files to the rm command to delete them.
```
For example, to remove 5 random files from the current directory, you would run the following command:

```
ls | shuf -n 5 | xargs rm
```
Note that this command will permanently delete the selected files, so be sure to use it with caution and double-check that you have selected the correct number of files before running it. Also, make sure that you have appropriate permissions to delete the files in the directory.



