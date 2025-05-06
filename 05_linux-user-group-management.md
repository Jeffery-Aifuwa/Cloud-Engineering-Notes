# Managing Users and Groups in Linux

Linux allows multiple users to share the same system. Each user has specific permissions and access rights.

## Viewing Users
```bash
cat /etc/passwd  # Displays a list of all system users
```

## Adding a User
```bash
sudo su                # Switch to root user (required for user management)
useradd username       # Creates a new user
passwd username        # Sets a password for the user
useradd -m username    # Creates a user along with a home directory
useradd -g groupname username  # Adds a user to a specific group
id username            # Displays the user’s ID and group ID
useradd -s /usr/bin/zsh username  # Assigns a specific shell (e.g., Zsh) to the user
```

### Example:
```bash
sudo su
useradd john
passwd john  # Set password
```
Now, 'john' is a new user on the system!

## Viewing Groups
```bash
cat /etc/group  # Displays a list of all system groups
```

## Managing Groups
```bash
groupadd [groupname]             # Creates a new group
groupmod -n [newname] [oldname]  # Renames a group
groupdel [groupname]             # Deletes a group
cat /etc/group                   # Displays all groups
cat /etc/group | grep [username]  # Searches for a specific user in group records
```

## File Permissions and Ownership
```bash
ls -l   # Lists files with permissions
ls -al  # Lists all files, including hidden ones, with permissions
```

### Permission Values
- Read (r) = 4  
- Write (w) = 2  
- Execute (x) = 1  

## Changing Ownership
```bash
chown [new_owner] [file]           # Changes file owner
chown [owner]:[group] [file]       # Changes both owner and group
```

## Changing Permissions
```bash
chmod [number] [file]              # Changes permissions using numeric mode
chmod u+x myfile.txt               # Adds execute permission for the user
chmod g-w myfile.txt               # Removes write permission for the group
chmod o=r myfile.txt               # Sets others' permissions to read-only
chmod a+x myfile.txt               # Gives execute permission to all (user, group, others)
```

### Example:
```bash
chmod 755 myfile.txt  # Owner can read, write, execute; others can read & execute
```
