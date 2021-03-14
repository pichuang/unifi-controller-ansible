# Unifi Controller Day 2 Operation

## Prerequisite
1. Edit variables in `hosts`
2. Replace ssh private/public key

## Features
- [x] Fetch Unifi Controller config - `ansible-playbook backup-config.yml`

![](/img/backup.png)


## Information
- Ansible 2.10.5
- macOS Catalina 10.15.7

## Appendix
### SSH Key Generate
```bash
ssh-keygen -t rsa -b 4096

...omit...

ssh-copy-id -i ubi_rsa.pub root@<controller ip>
```