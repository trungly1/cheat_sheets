| **Command** | **Description** | **Example** |
|---|---|---|
| `git init` | Initializes a new Git repository in the current directory | `git init my-project` |
| `git clone <remote-url>` | Clones an existing Git repository from a remote URL | `git clone https://github.com/username/repository.git` |
| `git add <file>` | Adds a file to the staging area | `git add index.html styles.css` |
| `git add .` | Adds all tracked files to the staging area | `git add .` |
| `git status` | Shows the status of the working directory and staging area | `git status` |
| `git commit -m "<message>"` | Commits the changes in the staging area to the repository | `git commit -m "Updated index.html and styles.css"` |
| `git branch` | Lists all local branches | `git branch` |
| `git checkout <branch-name>` | Switches to the specified branch | `git checkout master` |
| `git merge <branch-name>` | Merges the specified branch into the current branch | `git merge feature-branch` |
| `git push <remote-name> <branch-name>` | Pushes the specified branch to the remote repository | `git push origin master` |
| `git pull <remote-name> <branch-name>` | Fetches and merges the specified branch from the remote repository | `git pull origin master` |
| `git diff <file>` | Shows the differences between the working directory and the specified file in the repository | `git diff index.html` |
| `git diff <branch-name>` | Shows the differences between the current branch and the specified branch | `git diff feature-branch` |
| `git log` | Shows the history of commits | `git log` |
| `git log --oneline` | Shows the history of commits in a single line format | `git log --oneline` |
| `git log --graph` | Shows the history of commits in a graphical format | `git log --graph` |
| `git reset HEAD <file>` | Unstages the specified file from the staging area | `git reset HEAD index.html` |
| `git reset --hard HEAD <commit-hash>` | Resets the working directory and staging area to the specified commit | `git reset --hard HEAD abc123` |
| `git remote add <remote-name> <remote-url>` | Adds a remote repository to the local repository | `git remote add origin https://github.com/username/repository.git` |
| `git remote -v` | Lists all remote repositories | `git remote -v` |
| `git config --global user.name "<name>"` | Sets the Git user name | `git config --global user.name "John Doe"` |
| `git config --global user.email "<email>"` | Sets the Git user email | `git config --global user.email "johndoe@example.com"` |

These are just some of the most common Git commands. For a more comprehensive list of commands and their options, please refer to the official Git documentation: [https://git-scm.com/](https://git-scm.com/)
