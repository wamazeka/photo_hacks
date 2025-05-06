# photo_hacks
Some little hacks for photos, configs or manuals


## FTPS for Sony A7C 

Proxmox LXC container Alpine with VSFTPD

- raw template Alpine container
- `apk add vsftpd`
- `adduser USERNAME`
- create certificate with openssl
- copy my config
- `rc-update add vsftpd default`
- setup server in camera

can use `vsftpd /etc/vsftpd/vsftpd.conf` for checking errors in config. Maybe you have to clean from spaces or other symbols


I use NAS mount point in /mnt/nas, you can use something else, or just FTP client

Main part -- ciphers and SSL config lines, because Sony using old and unsecure (but it is better than simple FTP) 

Now, my Sony a7c copying files with 3 MB\s in local network
