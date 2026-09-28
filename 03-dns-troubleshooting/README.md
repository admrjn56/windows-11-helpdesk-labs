# Lab 03: DNS timeout diagnosis

## Environment

Windows 11 virtual machine in VMware Fusion.

## What I observed

Inspected the original DNS server, then tested a deliberately invalid server (203.0.113.1). IP ping still worked while nslookup timed out. The screenshots show the DNS setting being changed back; the before-and-after sequence demonstrates the distinction between IP reachability and name resolution.

## Screenshots

- [09-17 at 10.11.39](screenshots/09-17-101139.png)
- [09-17 at 10.39.12](screenshots/09-17-103912.png)
- [09-17 at 10.41.02](screenshots/09-17-104102.png)
- [09-17 at 11.07.16](screenshots/09-17-110716.png)
- [09-17 at 11.09.18](screenshots/09-17-110918.png)
