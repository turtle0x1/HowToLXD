---
title: Undestanding Projects
page.title: Undestanding Projects
---
# Understanding Projects

`LXD` projecs are very similar to Google's!

You can have containers, virtual machines, storage, networks ETC segragated by `project/s`.

This segragation is what enables `LXD` & `LXDMosaic` to limit `user/s` access.

**Other limits** like CPU & memory can be defined here, but only in very recent versions of `LXD`

*[The `LXD` server you initilazed in the last step](undestanding_lxd.html) gives you one server with one project `default`.*

*This project is where everthing is created if the user is not using / assigned to another project*

*Both `LXD` & `LXDMosaic` both support segragrating an `LXD` server by project/s.*

## Projects

Lets imagine we have 2 teams, `dev` & `pod`

We have two options to create the projects for the teams here;

 1. Use `lxc` (CLI)
   -  (TODO link to create projects with `lxc`)
 2. Use `LXDMosaic` (WEBB UI)
  - (TODO link to create projects with `LXDMosaic`)
