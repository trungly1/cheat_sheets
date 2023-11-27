| Command | Description | Example |
|---|---|---|
| ssh user@remote_host | Connects to the remote host remote_host as the user user. | `ssh john@192.168.1.100` |
| ssh-keygen | Generates a new SSH key pair. | `ssh-keygen -t rsa` |
| ssh-copy-id user@remote_host | Copies your public SSH key to the remote host remote_host. | `ssh-copy-id john@192.168.1.100` |
| ssh-keyscan remote_host | Prints the SSH fingerprint of the remote host remote_host. | `ssh-keyscan 192.168.1.100` |
| scp local_file user@remote_host:remote_path | Copies the local file local_file to the remote path remote_path on the remote host remote_host. | `scp my_file.txt john@192.168.1.100:/home/john/my_file.txt` |
| scp user@remote_host:remote_path local_file | Copies the remote file remote_path on the remote host remote_host to the local file local_file. | `scp john@192.168.1.100:/home/john/my_file.txt my_file.txt` |
| sftp | Opens an SFTP session with the remote host remote_host. | `sftp john@192.168.1.100` |
| ssh -L local_port:remote_host:remote_port | Creates a local forward from local_port to remote_port on the remote host remote_host. | `ssh -L 8080:192.168.1.100:22 john@192.168.1.100` |
| ssh -R remote_port:localhost:local_port | Creates a remote forward from remote_port on the remote host remote_host to local_port on the local host. | `ssh -R 2222:localhost:8080 john@192.168.1.100` |

**SSH Options**

| Option | Description |
|---|---|
| -p port | Specifies the port to connect to on the remote host. |
| -i identity_file | Specifies the SSH private key file to use. |
| -v | Verbose mode. |
| -vv | More verbose mode. |
| -q | Quiet mode. |

**Examples**

```
ssh user@remote_host
ssh -p 2222 user@remote_host
ssh -i ~/.ssh/id_rsa user@remote_host
ssh -v user@remote_host
ssh -vv user@remote_host
ssh -q user@remote_host
```

**Commands Relating to Listing Available Keys**

| Command | Description | Example |
|---|---|---|
| ssh-add -l | Lists all available SSH keys in the default key store. | `ssh-add -l` |
| ssh-keyscan | Lists the SSH fingerprints of all available SSH keys in the default key store. | `ssh-keyscan` |
| ssh-agent | Launches the SSH agent and manages SSH keys. | `ssh-agent` |
| ssh-add -K | Adds the private key for the current user to the default key store. | `ssh-add -K` |
