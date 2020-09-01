---
layout: post
title:  Read Module
date:   2020-09-01 10:00:00 +0300
image:  02.jpg
---

# Searching in modules

As an example, when loading a module: 

> Connect-ExchangeOnline

PS generates a tmp file with imported commands, sometimes you want to check the option for executing commands.

First check loaded modules:

> Get-Module

You'll see a tmp_randomstuffs.random entry, lets check export the commands.

>  (Get-Module -name tmp_*).ExportedCommands | FT key 

Scrolling in PS is not really preferd, so lets do the following: 

> (Get-Module -name tmp_*).ExportedCommands | out-gridview

Great success, as you can see alot of commands you never even used or knew they excisted.


