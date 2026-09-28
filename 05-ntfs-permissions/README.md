# Lab 05: HR folder and NTFS permissions

## Environment

Windows 11 virtual machine in VMware Fusion.

## What I observed

Created the HR-Readers local group and added jsmith. whoami /groups confirms membership; icacls later shows read/execute on C:\CompanyData\HR. Access attempts also produced permission errors. Folder ACLs and child-file permissions must be checked separately; this evidence does not establish that every file was readable.

## Screenshots

- [09-22 at 4.32.50](screenshots/09-22-43250.png)
- [09-22 at 4.35.48](screenshots/09-22-43548.png)
- [09-22 at 4.42.00](screenshots/09-22-44200.png)
- [09-22 at 4.45.42](screenshots/09-22-44542.png)
- [09-28 at 11.23.44](screenshots/09-28-112344.png)
- [09-28 at 11.26.08](screenshots/09-28-112608.png)
