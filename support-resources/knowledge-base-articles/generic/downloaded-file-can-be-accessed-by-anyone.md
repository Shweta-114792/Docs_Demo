# Downloaded File can be Accessed by Anyone

**Summary**: This article explains the behaviour of the Find File Path action when accessing files from the local download directory and clarifies file accessibility limitations for multiple users

### Error behavior

When this issue occurs, you may observe the following behavior:

* The file located in the local download directory is not accessible to other users.
* When attempting to access the file path from another user session, the file cannot be found or accessed.
* No direct error may appear in Avo, but access fails due to system-level restrictions.

### **Possible Reasons**

This issue may occur due to one or more of the following reasons:

* Files downloaded locally are stored under user-specific system directories.
* Local file systems restrict access to the user profile that downloaded the file.
* Lack of shared storage location for the file.

### Resolution/Solution

To resolve this issue and ensure successful execution, perform the following actions:

1. If a file is saved locally, only the individual user who downloaded it can access it.
2. To make the file accessible to multiple users, it needs to be stored in a shared location.   \
   A network‑shared folder is an example of such a shared location.

###
