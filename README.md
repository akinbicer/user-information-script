# User Information Script

This script collects information about users on the system and displays it in a formatted manner. It is written in Bash.

## Prerequisites

- Linux operating system (CentOS, Red Hat, or similar)
- Bash shell

## Usage

1. Open a terminal.
2. Navigate to the directory where the script is located.
3. Make the script executable, if needed, by running the following command:
   ```
   chmod +x script.sh
   ```
4. Run the script by executing the following command:
   ```
   ./script.sh
   ```

## Functionality

- The script first collects information about the "root" user and displays it.
- For Linux systems (CentOS, Red Hat), the script then iterates over all the users in the "/home" directory.
  - It collects information such as creation time, password change time, last login time, user status, UID, GID, password existence, and sudo access.
  - The collected information is displayed for each user.
- For non-Linux systems, the script follows a similar process but with different log files.
- The script uses various commands such as `sudo`, `passwd`, `id`, `last`, and `grep` to collect the required information.

## Output

The script displays the following information for each user:

- Username
- Creation time
- Password last changed
- Last login time
- User status (enabled or disabled)
- UID (User ID)
- GID (Group ID)
- Password existence (True or False)
- Sudo access information
- Entry in /etc/passwd file

## Issues, Feature Requests or Support
Please use the [New Issue](https://github.com/akinbicer/docker-dnsmasq/issues/new) button to submit issues, feature requests or support issues directly to me. You can also send an e-mail to akin.bicer@outlook.com.tr.
