---
title: "Data science virtual machine"
date: 2018-04-20T15:30:30-04:00
categories:
  - projects
tags:
  - DevOps
---

## A self-configuring virtual machine for data-science projects

For many development projects, a lot of dependencies need to be installed on the machine, often requiring root privilidges. As the project evolves, those dependencies change, and with constant re- and re-re-installations, conficts arise, and the system (or some of it's components) breaks down.

What if you could destroy you current configuration and roll it back to an earlier date, or start over from scratch, without suffering from making constant backups of data unrelated to the project.

Vagrant, combined with Ansible, is the perfect tool for developing and testing complex software with constantly evolving dependencies. With just a few commands, you can set up a virtual machine, modify it, or destroy it... without worrying about any side effects on other, unrelated projects.

Checkout my repo for a [datasciencevm](https://github.com/theonlyid/datasciencevm).