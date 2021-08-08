---
layout: wiki-page
title: Port Forwarding
---

Port forwarding or port mapping in the context of LXD is the technique of directing traffic from one network (typically the host) to the appropriate container.

## Proxy

The recommended way of implementing port forwarding with LXD is to attach a device of type `proxy` to the target container.

### PROXY protocol

The default way of using a proxy device looks as follows:

```
lxc config device add <container> tcp1337 proxy \
        listen=tcp:0.0.0.0:1337 \
        connect=tcp:127.0.0.1:1337
```

### NAT mode

## iptables
