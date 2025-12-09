# Activity: Use Linux commands to manage file permissions

*This activity is based on a fictional scenario.*

**References**

* **file-permissions-in-linux.docx:** Activity template
* **current-file-permissions.docx:** Demonstrates how the file structure is built and provides permissions for each file and directory
* **instructions-for-including-linux-commands.docx:** Provides instructions and best practices for including samples of Linux commands
* **file-permissions-in-linux-exemplar.docx:** Sample solution

## Scenario

You are a security professional at a large organization. You mainly work with their research team. Part of your job is to ensure users on this team are authorized with the appropriate permissions. This helps keep the system secure.

Your task is to examine existing permissions on the file system. You'll need to determine if the permissions match the authorization that should be given. If they do not match, you'll need to modify the permissions to authorize the appropriate users and remove any unauthorised access.

## Use Linux commands to manage file permissions

### Project description

The task is to examine existing permissions on the file system to determine if the permissions match the authorization that should be given. If the permissions do not match they need to be modified to authorize the appropriate users and remove any unauthorised access. Checking and updating these permissions will help keep the system secure. To complete this task, I performed the following tasks:

### Check file and directory details

The `ls -al` command was used to confirm that the file permissions match the current file permissions listed in **current-file-permissions.docx:**.

![file-permissions-1.png](file-permissions-1.png)


### Describe the permissions string

A permission string is a 10-character code that describes a file's type and its read/write/execute permissions:

| Pos | Meaning            | Examples                                  |
|-----|--------------------|-------------------------------------------|
| 1   | File type          | `-`, `d`, `l`, `c`, `b`, `s`, `p`         |
| 2–4 | Owner permissions  | `rwx`, `rw-`, `r--`                       |
| 5–7 | Group permissions  | same as owner                             |
| 8–10| Others permissions | same as owner; may include `t` or `T`     |
| —   | Special bits       | `s/S` (setuid/setgid), `t/T` (sticky bit) |

**Example:** File permissions `-rw-rw-r--` (**project_r.txt**) represents a file where the owner and group can read and write, while others can read only, and no one has execute permission.

### Change file permissions

The organization does not allow others to have write access to any files.

The following command was run to remove write permissions for others for **project_k.txt**.

```
chmod o-w project_k.txt
```

### Change file permissions on a hidden file

The research team has archived **.project_x.txt**, which is why it's a hidden file. This file should not have write permissions for anyone, but the user and group should be able to read the file.

```
chmod u-w,g-w,g+r .project_x.txt
```

### Change directory permissions

The files and directories in the projects directory belong to the **researcher2** user. Only **researcher2** should be allowed to access the **drafts** directory and its contents.

```
chmod g-x drafts
```

### Summary

* The `chmod` command was used to change permissions on files and directories.
* The `ls -al` command was used to check the permissions were updated correctly.

Here are the final permissions:

![file-permissions-final.png](file-permissions-final.png)
