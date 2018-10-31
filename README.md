# EasyEngine-SFTP
Easily assign secure and robust SFTP-only access to users for single EasyEngine sites

## Inspired by:

http://blog.netgusto.com/solving-web-file-permissions-problem-once-and-for-all/

## Install [or update / re-install] [tested on Ubuntu 16]

```
[log in as root on your EasyEngine linux server]
cd
```

```
apt update
apt -y install git
```
```
git clone https://github.com/Delgesh/sftpengine
bash sftpengine/setup
```


## Set up

### Adding an SFTP user

```
bash delgesh/ee-sftp/add-user username
```

### Assigning a website to an SFTP user

```
bash delgesh/ee-sftp/add-site-to-user
```


## Logging in

### via command line

```
sftp username@server.hostname.tld
[password you specified during setup]
```

### via any SFTP graphical client

```
server: server.hostname.tld
port: [SSH port - usually 22]
[username and password you specified during setup]
```
