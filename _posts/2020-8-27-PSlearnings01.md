---
layout: post
title:  PS Learnings 
date:   2020-08-27 10:10:00 +0300
image:  02.jpg
---
## Learned 

# Setting a global variable.
If you create a Function in PS, the commands are executed within the function run-space. But sometimes you want to have the outcome running outside
that function. To do so you have to work with $global / $local: variable. 

Example in PS


> Function auth{$global:cred = "test"}
> auth
>$cred



You made a function called Auth, within this function you created a global out of scope variable named Cred with Test as output.
If you run your function and run $cred, normally it shouldn't show any output because it keeps it withing the function. But now its 
outside of your function so you can use it. 

You don't have to use the word global, it can be local or something that references to out-of-scope. 

# Join path

Sometimes you have a few variable that together make a FullyQualifiedName path towards an item, but you need a way to merge them together.
Here is where Join Path comes into play.



# Multi Search / Select and purge

Within Visual Studio when you select a string and Press <strong>  CONTROL + F </strong>  you'll notice you select the word you highlighted.
If you press <strong> Alt + Enter </strong> you get a way to manipulate all the same name fields/strings. 
Also handy to purge a C:/user-name blab-la sting that's in the way :> 


# MS Teams sharing Code
Within MS Teams you have the following option to share code in proper format. 
> Opmaak -> Meer Opties -> CodeFragment -> Select Code style preferably Powershell Grote glimlach
​​​​​​​ 
This way you are able to share your code in perfect state to colleges to gloat over the awesomeness you've created.
