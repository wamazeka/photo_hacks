# photo_hacks
Some little hacks for photos, configs or manuals


## FTPS for Sony A7C 

Proxmox LXC container Alpine with VSFTPD
- create user
- create certificate
- copy config
- setup server in camera

I use NAS mount point in /mnt/nas, you can use something else, or just FTP client

Main part -- ciphers and SSL config lines, because Sony using old and unsecure (but it is better than simple FTP) 

Now, my Sony a7c copying files with 3 MB\s in local network
