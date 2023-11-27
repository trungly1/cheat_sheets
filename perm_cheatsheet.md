| Permission | Description | Octal Value | Symbolic Notation |
|---|---|---|---|
| Read (r) | Allows the user to read the contents of a file | 4 | r |
| Write (w) | Allows the user to write to or modify a file | 2 | w |
| Execute (x) | Allows the user to execute a file or enter a directory | 1 | x |

**Examples:**

* To grant the user read and write permissions to a file, use the following command:

```bash
chmod 600 file.txt
```

This command sets the permissions of the file to 600. The first digit (6) represents the permissions for the user, the second digit (0) represents the permissions for the group, and the third digit (0) represents the permissions for others.

* To grant all users read, write, and execute permissions to a file, use the following command:

```bash
chmod 777 file.txt
```

This command sets the permissions of the file to 777. The first digit (7) represents the permissions for the user, the second digit (7) represents the permissions for the group, and the third digit (7) represents the permissions for others.

**Popular chmod commands:**

* `chmod u+rwx filename`: Adds read, write, and execute permissions for the user.
* `chmod g+rx filename`: Adds read and execute permissions for the group.
* `chmod o+r filename`: Adds read permissions for others.
* `chmod u-x filename`: Removes execute permission for the user.
* `chmod g-w filename`: Removes write permission for the group.
* `chmod o-r filename`: Removes read permission for others.

**Chown command:**

The `chown` command is used to change the owner of a file or directory. The syntax of the `chown` command is as follows:

```bash
chown owner[:group] filename
```

**Examples:**

* To change the owner of a file to user1, use the following command:

```bash
chown user1 file.txt
```

* To change the owner of a file to user1 and the group to group2, use the following command:

```bash
chown user1:group2 file.txt
```
