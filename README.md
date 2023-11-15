# internCTL

`internctl` is a command-line tool designed to perform various system operations. It provides functionalities related to CPU information, memory information, user management, and file information retrieval.

## Table of Contents
- [internctl](#internctl)
  - [Table of Contents](#table-of-contents)
  - [Installation](#installation)
    - [Options:](#options)
      - [Subcommands](#subcommands)
    - [Examples](#examples)
  - [Contributing](#contributing)
  - [License](#license)

## Installation

To use `internctl`, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/internctl.git
   
```bash
cd internctl
``````
```bash 
chmod +x internctl
```
```bash
sudo mv internctl /usr/local/bin/

```
```bash
internctl [options] subcommand [arguments]

```

### Options:
- --help: Display help information.
- --version: Display the version of internctl.
#### Subcommands
- cpu getinfo: Get CPU information (similar to lscpu).
- memory getinfo: Get memory information (similar to free).
- user create <username>: Create a new user with the given username.
- user list: List all regular users.
- user list --sudo-only: List users with sudo permissions.
- file getinfo [options] <file-name>: Get information about a file.
Options:
 --size, -s: Print file size.
 --permissions, -p: Print file permissions.
 --owner, -o: Print file owner.
 --last-modified, -m: Print last modified time of the file.

 ### Examples

 ```bash
 # Get CPU information
internctl cpu getinfo

# Get memory information
internctl memory getinfo

# Create a new user
internctl user create newuser

# List all regular users
internctl user list

# List users with sudo permissions
internctl user list --sudo-only

# Get file size
internctl file getinfo --size sample.txt

# Get file permissions
internctl file getinfo --permissions sample.txt

# Get file owner
internctl file getinfo --owner sample.txt

# Get last modified time of the file
internctl file getinfo --last-modified sample.txt
```
