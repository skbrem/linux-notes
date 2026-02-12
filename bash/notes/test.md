The command that is used the most with `if` is `test`. There are two forms of the test command: 

1. `test *expression*`
2. `[ *expression* ]`

The *expression* is the expression that is being evaluated as either true or false. If the expression is true, the test command will return with an exit status of 0, and if it's false, it will return with an exit status of 1. 


## File Expressions Table

| Expression | Is true if: |
| --- | --- |
| *file1* `-ef` *file2* | *file1* and *file2* have the same inode numbers. |
| *file1* `-nt` *file2* | *file1* is newer than *file2*. |
| *file1* `-ot` *file2* | *file1* is older than *file2* |
| `-b` *file* | exists and is a block-special (device) file. |
| `-c` *file* | exists and is a character-special (device) file. |
| `-d` *file* | *file* does exist and is a directory |
| `-e` *file* | file exists |
| `-f` *file* | exists and is a regular file |
| `-g` *file* | exists and is set-group-ID |
| `-G` *file* | file exists and is owned by the effective group ID |
| `-k` *file* | exists and its sticky bit is set. |
| `-L` *file* | exists and is a symbolic link |
| `-O` *file* | exists and is owned by effective user ID |
| `-p` *file* | exists and is a named pipe |
| `-r` *file* | exists and is readable |
| `-s` *file* | exists and has a length greater than zero |
| `-S` *file* | exists and is a network socket |
| `-t` *fd* | this is a descriptor type that is directed to and from the terminal. It's used to determine whether standard input/output/error is being redirected. |
| `-u` *file* | exists and is setuid |
| `-w` *file* | exists and is writable |
| `-x` *file* | exists and is executable |


