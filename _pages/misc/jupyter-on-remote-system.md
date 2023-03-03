---
layout: archive
title: Jupyter on remote system
permalink: /misc/jupyter-on-remote-system
author_profile: true
---

### Configureration of ssh on local

Edit ssh config at `~/.ssh/config` as follows.

```
Host YOUR_SERVER_NAME
HostName IP_ADDRESS
User YOUR_USER_NAME
IdentityFile ~/.ssh/YOUR_SSH_KEY
Port 22
LocalForward 9999 localhost:9999
ServerAliveInterval 60
```

In this example, you login to the server at `IP_ADDRESS` with user name `YOUR_USER_NAME` using the ssh key of `~/.ssh/YOUR_SSH_KEY`.
You can login the server by

```
ssh YOUR_SERVER_NAME
```

### Setting on the remote server

```
c = get_config()

c.IPKernelApp.pylab = 'inline'
c.ServerApp.ip                  = 'localhost'
c.ServerApp.port                = 9999
c.ServerApp.allow_remote_access = True
c.ServerApp.password            = 'HASHED_PASSWORD'
c.ServerApp.open_browser        = False
```

Here, you need to specify your hased password of jupyter.
You can obtain the hased password by running,

```
python -c 'from notebook.auth import passwd;print(passwd())'
```

and entering your jupyter password.
