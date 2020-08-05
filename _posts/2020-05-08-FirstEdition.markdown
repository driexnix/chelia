---
layout: post
title:  First Edition
date:   2020-08-05 10:10:00 +0300
image:  02.jpg
---

# PowerShell
Let's try to make a fast script that wil "WoW" your online fans....

## Open PowerShell ISE

Copy & Past below highlighted area in PS ISE and click run.
Windows might uninstall if done right.

{% highlight js %} 
#Show current connected Wi-Fi name (SSID).
$CurrentWifi= (Get-NetConnectionProfile).name  

#Execute Order 66 plus show current wifi password.
netsh wlan show profile name="$CurrentWifi" key=clear | findstr Key

{% endhighlight %}

> Hacker man, you are.