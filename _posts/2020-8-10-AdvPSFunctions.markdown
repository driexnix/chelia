---
layout: post
title:  Advanced PS Functions
date:   2020-08-10 10:10:00 +0300
image:  01.jpg
---
# Input methodes voor functies 

* Begin - Beschikt over alle benodigde code
* Process - main functions
* End - 

> net localgroup administrators | select -skip 6 | ? {$_ -and $_ -notmatch 'Taak Voltooid.|^administrator$|^admin$'}


Namespace 

> $test = New-WebServiceProxy -Namespace -Uri "http://www.dneonline.com/calculator.asmx?wsdl"
> $test | Get-Member 
> $test | Get-Member -MemberType method
> $test.Multiply(6,7)
