---
layout: archive
title: Cisco from CLI
permalink: /misc/cisco-from-cli
author_profile: true
---

### Cisco AnyConnect

Cisco AnyConnect is a virtual private network (VPN) software that allows users to remotely access a network from anywhere in the world, securely and with ease. It is commonly used in enterprise and corporate settings to provide employees with access to company resources, such as servers, databases, and applications, without compromising security.

### Connecting VPN from CLI

Usually, people connect to VPN server with the Desktop Cisco AnyConnect application. Cisco AnyConnect also has command line interface, so we can easily connect to VPN server from command line interface (CLI).

Cisco CLI is available at

```console
ls /opt/cisco/anyconnect/bin/
```

To connect the VPN server "XXX", do as

```console
/opt/cisco/anyconnect/bin/vpn -s connect XXX
```

Then, you can connect to the server XXX after giving your username and password.

### Automating Cisco AnyConnect from CLI

This step can be automated using with an executable script (name this file as `cisco2xxx`)

```bash
#!/usr/bin/expect
# Conenct to VPN server with vpn by Cisco
# Here we assume server name "XXX",  your username "yourusername", and your password "yourpassword"

spawn /opt/cisco/anyconnect/bin/vpn -s connect XXX

expect "Group: \\\[Remote_User\\\]" {send "\r" }
expect "Username: " { send "yourusename\r" }
expect "Password: " { send "yourpassword\r" }
expect "accept? \\\[y/n\\\]:" { send "y\r" }

set timeout 60
expect "VPN>"
```

Put this script to the directory where the PATH is setted, then you can connect to the server XXX by executing

```
cisco2xxx
```

### Disconnecting Cisco AnyConnect

```console
vpn -s disconnect
```

### Checking the status of VPN connection

```console
vpn -s stats
```

If you just want to see whether the VPN is connected or not, do as

```
vpn -s state | grep "notice: Connected"
```
