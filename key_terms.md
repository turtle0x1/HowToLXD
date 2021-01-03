---
title: Key Terms
page.title: Key Terms
---
## LXD Key Terms
Like all software `LXC` & `LXD` has evolved over time, its important to understand
whats happened!
## LXC - C Program
Originally there was `LXC` program / application wirtten in `C`.

The original `LXC` is the application is responsible for running containers &
virtual machines at a "low level".

The application `LXC` itself is rarely directly interacted with these days,
some operating systems like `Debian` have been slow to package `LXD` and so
as a result you will still some people making reference to commands like;

 - `lxc-ls`
 - `lxc-create`
 - `lxc-console`

These commands wont apply for any documentation found on this site as we
interact with the modern `LXD`!

That being said some projects like [Proxmox](https://proxmox.com/) made the
decision to directly interact with `LXC`, but they are the exception not the
norm!

## LXD

`LXD` in the projects own words is;

> A next generation system container and virtual machine manager.

Its written in `GO` and offeres a REST API built on top on the low level `C`
application `LXC` to offer an easy and convineniat way to manage containers &
virtual machines!

## LXC - GO Program
After `LXD` was written a new command line program was needed to interact
with the `LXD` REST API, a decision was made above the developers head to name
this program `LXC`.

This could cause a significant ammount of confusion as the diffence between
the `C` application `LXC` and the `GO` `LXC` application is vast.

 - `LXC` the `C` application is responsible for running your containers
 - `LXC` the `GO` application issues `HTTP` requests to one or more `LXD` instances (much like searching for google.com in your browser)

Most people using LXC / LXD will be used to running to the modern `GO` `LXC`
application which uses commands like;

 - `lxc list`
 - `lxc create`
 - `lxc storage list`

These commands are thinly veild `HTTP` requests, programs like [LXDMosaic](https://github.com/turtle0x1/LxdMosaic)
are alternatives to the `lxc` command.

*Currently no publicly available graphical interface (LXDMosaic included) is as feature complete as the `LXC` tool!*

### Next
[Lets undestand LXD Architecture!](undestanding_lxd.html)
