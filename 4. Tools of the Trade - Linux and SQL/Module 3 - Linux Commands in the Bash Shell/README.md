# Module 3: Linux Commands in the Bash Shell

## Overview

* The command line
* Navigating and managing the file system
* Authenticating and authorising users
* Accessing resources

## Navigating and managing the file system

The command line can be used to navigate, manage, and analyze files remotely via a Linux shell without a graphical user interface.

Simple Linux Bash shell commands can be used to:

* navigate directory structures with the **cd** command,
* display the current working directory with the **pwd** command,
* list the contents of a directory with the **ls** command, and
* display the contents of files with the **cat** and **head** commands.

Filtering for information using Linux commands is an important skill for security analysts so that they can customise data to fit their needs. Three key Linux commands for this are **grep**, **piping (|)**, and **find**. These commands can be used to navigate and filter for information in the file system.

Knowing how to manage the file system in Linux is an important skill for security analysts. Useful commands for this include: **mkdir**, **rmdir**, **touch**, **rm**, **mv**, and **cp**. When security analysts need to write to files, they can use the **nano** text editor, or the **>** and **>>** operators.

## Authenticating and authorising users

Authorization is the concept of granting access to specific resources in a system. It's important because without authorization any user could access and modify all files belonging to other users or system files. This would certainly be a security risk.

Permissions are represented with a 10-character string. Permissions include:

* **read:** for files, this is the ability to read the file contents; for directories, this is the ability to read all contents in the directory including both files and subdirectories
* **write:** for files, this is the ability to make modifications on the file contents; for directories, this is the ability to create new files in the directory
* **execute:** for files, this is the ability to execute the file if it's a program; for directories, this is the ability to enter the directory and access its files

These permissions are given to these types of owners:

* **user:** the owner of the file
* **group:** a larger group that the owner is a part of
* **other:** all other users on the system

Using **ls** with the **-l** and **-al** options allows you to investigate directory and file permissions. Using **chmod** allows you to change user permissions and ensure they are aligned with the principle of least privilege.

### Responsible use of sudo

To manage authorization and authentication, you need to be a root user, or a user with elevated privileges to modify the system. However, running commands as the root user is not recommended because it can create security risks if malicious actors compromise that account. It's also easy to make irreversible mistakes, and the system can't track who ran a command. For these reasons, rather than logging in as the root user, it's recommended you use sudo in Linux when you need elevated privileges.

The sudo command can be used to to temporarily run commands with elevated privileges to complete authentication and authorization management tasks. Specifically, **useradd**, **userdel**, **usermod**, and **chown** can be used to manage users and file ownership.

## Accessing resources

There are many resources available for troubleshooting issues or getting support for Linux. Linux has a large global community of users who ask and answer questions on online resources. You can also use integrated support commands in Linux, such as **man**, **apropos**, and **whatis**.

## Glossary: Linux Commands in the Bash Shell

**Absolute file path:** The full file path, which starts from the root

**Argument (Linux):** Specific information needed by a command

**Authentication:** The process of verifying who someone is

**Authorization:** The concept of granting access to specific resources in a system

**Bash:** The default shell in most Linux distributions

**Command:** An instruction telling the computer to do something

**File path:** The location of a file or directory

**Filesystem Hierarchy Standard (FHS):** The component of the Linux OS that organises data

**Filtering:** Selecting data that match a certain condition

**nano:** A command-line file editor that is available by default in many Linux distributions

**Options:** Input that modifies the behaviour of a command

**Permissions:** The type of access granted for a file or directory

**Principle of least privilege:** The concept of granting only the minimal access and authorization required to complete a task or function

**Relative file path:** A file path that starts from the user's current directory

**Root directory:** The highest-level directory in Linux

**Root user (or superuser):** A user with elevated privileges to modify the system

**Standard input:** Information received by the OS via the command line

**Standard output:** Information returned by the OS through the shell
