# Initial Setup

## Create a User
`adduser YOURNAMEHERE`

## Add to Sudoers
`sudo vim /etc/sudoers`

Add this line:
`YOURNAMEHERE ALL=(ALL) ALL`

## Add SSH Key

```
sudo -u YOURNAMEHERE -i
mkdir .ssh
chmod 700 .ssh
vim .ssh/authorized_keys
<paste pubkey and write>
chmod 600 authorized_keys
```

## Access Your Account

At this point, you should be able to ssh in as your new user and run a command as sudo. If that works, you’re ready for the next step.

## Disable Password-based Authentication and Root Access

`sudo vim /etc/ssh/sshd_config`
set `PasswordAuthentication` to `no`
set `PermitRootLogin` to `no`

`sudo /etc/init.d/ssh reload`

Now you are ready to start setting up!