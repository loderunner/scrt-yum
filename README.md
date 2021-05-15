# This is the YUM repository for [`scrt`](https://github.com/loderunner/scrt).

See https://github.com/loderunner/scrt for details.

## Install instructions

To install `scrt` using `yum`,

Add `scrt` repository by creating the following file at `/etc/yum.repos.d/scrt.repo`:

```conf
[scrt]
name=scrt
baseurl=https://loderunner.github.io/scrt-yum/main
repo_gpgcheck=1
gpgcheck=0
enabled=1
gpgkey=https://loderunner.github.io/scrt-yum/key.gpg
sslverify=1
metadata_expire=300
```

Install `scrt`:

```sh
sudo yum update
sudo yum install scrt
```
