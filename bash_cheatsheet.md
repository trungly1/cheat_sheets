| Command | Description | Example |
|---|---|---|
| pwd | Prints the working directory | pwd |
| ls | Lists the contents of the current directory | ls |
| mkdir | Creates a directory | mkdir new_directory |
| cd | Changes the current directory | cd new_directory |
| rm | Removes a file or directory | rm file.txt |
| cp | Copies a file or directory | cp file.txt new_directory |
| mv | Moves a file or directory | mv file.txt new_directory |
| touch | Creates an empty file | touch new_file.txt |
| cat | Concatenates and displays files | cat file1.txt file2.txt |
| grep | Searches for text in files | grep "search_term" file.txt |
| sort | Sorts lines of text | sort file.txt |
| uniq | Prints only unique lines | uniq file.txt |
| cut | Cuts text from files | cut -d ":" -f 2 file.txt |
| awk | Performs pattern matching and data processing | awk '{print $1,$2}' file.txt |

**mkdir**

| Argument | Description | Example |
|---|---|---|
| -p | Creates any parent directories that do not exist | mkdir -p documents/projects/new_project |
| -m | Sets the permissions of the new directory | mkdir -m 755 new_directory |

**grep**

| Argument | Description | Example |
|---|---|---|
| -i | Case-insensitive search | grep -i "search_term" file.txt |
| -r | Searches recursively through directories | grep -r "search_term" directory |
| -v | Prints lines that do not contain the search term | grep -v "search_term" file.txt |
| -n | Prints line numbers with the matched lines | grep -n "search_term" file.txt |

**cp**

| Argument | Description | Example |
|---|---|---|
| -r | Copies recursively, including subdirectories | cp -r directory1 directory2 |
| -v | Verbose output, showing each file being copied | cp -v file1.txt file2.txt |
| -f | Forces the copy, even if the destination file exists | cp -f file1.txt file2.txt |
| -p | Preserves file permissions and ownership | cp -p file1.txt file2.txt |

**mv**

| Argument | Description | Example |
|---|---|---|
| -f | Forces the move, even if the destination file exists | mv -f file1.txt file2.txt |
| -n | Renames the file, but does not move it | mv file1.txt file2.txt |
| -i | Prompts for confirmation before moving each file | mv -i file1.txt file2.txt |

**rm**

| Argument | Description | Example |
|---|---|---|
| -r | Removes recursively, including subdirectories | rm -r directory |
| -f | Forces the deletion, even if the file is write-protected | rm -f file.txt |
| -v | Verbose output, showing each file being deleted | rm -v file1.txt file2.txt |

**ls**

| Argument | Description | Example |
|---|---|---|
| -l | Lists files with detailed information | ls -l |
| -a | Lists all files, including hidden files | ls -a |
| -d | Lists directories as entries, not as symbolic links | ls -d directory |
| -F | Adds a slash (/) to the end of directory names | ls -F |

**awk**

| Argument | Description | Example |
|---|---|---|
| '{print $1,$2}' | Prints the first two fields of each line | awk '{print $1,$2}' file.txt |
| '$2 > 10' | Prints lines where the second field is greater than 10 | awk '$2 > 10' file.txt |
| '^search_term' | Prints lines that start with the search term | awk '^search_term' file.txt |
| 'search_term$ | Prints lines that end with the search term | awk 'search_term$' file.txt |
