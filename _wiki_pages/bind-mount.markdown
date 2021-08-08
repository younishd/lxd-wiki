---
layout: wiki-page
title: Bind Mounting
---

Bind mounting...

## Disk

The recommended way of implementing bind mounting with LXD is to attach a device of type `disk` to the target container.

Example:

```
lxc config device add <container> mydisk disk \
        source=/home/alice \
        path=/mnt
```

## UID/GID mapping

WIP…
