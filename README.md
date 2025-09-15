# [EspoCRM Build Guide CVE-2025-32390]

## Status

| Firewall      | On/Off |
| ------------- | ------ |
| Updates       | On/Off |
| ICMP          | On/Off |
| IPV6          | On/Off |
| AV / Security | On/Off |

## Overview

| OS                 | [e.g., Ubuntu 22.04 LTS] |
| ------------------ | ------------------------ |
| HOSTNAME           | [espocrm]                |
| CTF_ROOT_USERNAME  | [espouser]               |
| CTF_ROOT_USERPASS  | [espopass]               |
| CTF_ROOT_FLAGNAME  | [proof.txt]              |
| CTF_ROOT_FLAGTEXT  | [5d41402abc4b2a76b9719d911017c592]|
| CTF_SSH_USERNAME   | [user]|
| CTF_SSH_USERPASS   | [SshUserPass123]|

## Requirements

| CPU     | [1]     |
| ------- | ------------- |
| Memory  | [2 GB]  |
| Storage | [25 GB] |

## Build

1. Install `[Ubuntu 24.0.X]`.
2. Upload `build.sh` to `/root`.
3. Run `build.sh` as `root`.
4. Wait for the build it will prompt with creation of the Admin page.
5. Open `http://localhost:8082` in your browser and follow the setup steps:
    - **Database name**: `espocrm`
    - **Database user**: `espouser`
    - **Database password**: `espopass`
6. Test the connection and proceed with installation.
    - **Username**: `admin`
    - **Password**: `admin123`
7. Once installed:
    - Click **Enter** in the terminal.
    - Create a user by clicking the three-dot menu in the top-right corner and selecting **Administrator**.
8. Go to **Users** and click **Create User** in the top-right corner:
    - **Username**: `user`
    - **Password**: `SshUserPass123`
    - **Email**: `user@example.com`
9. Click **Enter** again in the terminal the script will set up the bot.
10. Done.
