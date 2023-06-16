# Migrating Files

## Special Copy

Copy a file from your local machine to a server directory:

```scp ~/Documents/file.txt user@ip.add.re.ss:/var/www/file.txt```

Copy a file from a server to your local machine:

```scp user@ip.add.re.ss:/var/www/file.txt ~/Documents/files.txt```

## RYSNC

If you want to copy entire directories, then it is better to use rysnc as if there is an error during the process you don’t need to restart from the beginning like you do with scp.

Copy a folder (and all files and folders it contains) from a server to your local machine:

```rsync -chavzP --stats user@ip.add.re.ss:/path/to/copy /path/to/local/storage```

Copy a folder (and all files and folders it contains) from your local machine to a server:

```rsync -chavzP --stats /path/to/local/storage user@ip.add.re.ss:/path/to/copy```
