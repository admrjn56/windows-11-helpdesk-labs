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
