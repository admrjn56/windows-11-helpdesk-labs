# Lab 01 – Password Reset & Local User Troubleshooting

## Objective

Practice troubleshooting a Windows user who is unable to access their account and perform a password reset using administrative tools.

## Scenario

A user reports that they are unable to sign in to their Windows account.

As the Help Desk technician, I need to verify the account exists, reset the password, and confirm that the user can successfully authenticate.

## Environment

- Windows 11
- VMware Fusion
- PowerShell
- Local Windows user accounts

## Tools Used

- PowerShell
- Command Prompt
- `net user`

## Troubleshooting Process

### 1. Verified the local user account

```powershell
net user
```

This command displays the local user accounts configured on the Windows workstation.

### 2. Attempted the administrative action

When attempting to modify the account without sufficient privileges, Windows returned an Access Denied error.

This showed that password and account-management tasks require administrative privileges.

### 3. Opened PowerShell as Administrator

I reopened PowerShell using elevated administrative privileges.

### 4. Reset the user's password

```powershell
net user USERNAME *
```

This command allows an administrator to assign a new password to a local Windows user account.

### 5. Verified the resolution

I confirmed that the account remained enabled and that the new credentials could be used successfully.

## Resolution

The local user's password was successfully reset using an elevated administrative terminal.

The account was then tested to confirm that the new credentials worked.

## What I Learned

- How to identify local Windows users
- How administrative permissions affect account management
- How to reset a local user's password
- How to recognize an Access Denied error
- Why a Help Desk technician should verify a fix before closing a ticket

## Real-World Help Desk Relevance

Password resets and account-access issues are common Tier 1 Help Desk requests.

In a real organization, a technician should verify the user's identity according to company policy before resetting credentials and confirm that the user can successfully authenticate afterward.

## Evidence

Screenshots documenting the troubleshooting process are stored in the `screenshots` folder.
