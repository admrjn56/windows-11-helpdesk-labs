# Lab 15: 7-Zip installation blocked by DNS

## Environment

Windows 11 virtual machine in VMware Fusion.

## What I observed

Confirmed 7-Zip was absent, then winget install 7zip.7zip failed with InternetOpenUrl() and 0x80072ee7. Ping to 8.8.8.8 succeeded while the configured DNS server timed out. A query through 8.8.8.8 resolved www.7-zip.org. After changing DNS and flushing its cache, the install succeeded. The original DNS configuration was restored after the test.

## Screenshots

- [09-28 at 10.25.50](screenshots/09-28-102550.png)
- [09-28 at 10.28.16](screenshots/09-28-102816.png)
- [09-28 at 10.30.36](screenshots/09-28-103036.png)
- [09-28 at 10.31.43](screenshots/09-28-103143.png)
- [09-28 at 10.34.08](screenshots/09-28-103408.png)
- [09-28 at 10.34.13](screenshots/09-28-103413.png)
- [09-28 at 10.36.49](screenshots/09-28-103649.png)
- [09-28 at 11.34.39](screenshots/09-28-113439.png)
