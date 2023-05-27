---
title: Variables
description: let, var, const etc.
weight: 1
lastmod: 2023-05-20T10:23:30-09:00
draft: false
vimeo: 773633416
emoji: 🚆
video_length: 1:33
chapter_start: 
free: true
---


Variables are a place to store data. 

Ways of declaring a variable: 

1. let
2. var
3. const
4. (nothing)

var is the legacy way of declaring variables. 

var is function scoped. 

what is a scope

can redeclare a variable in var

let is block scoped.

Got added in ES6

cannot redeclare

const is block scoped

Got added in ES6

must be assigned

cannot redeclare

Const doesnt allow you to change the value of reference. const doesn’t say that it’ll always have the constant value. which means, you cannot reassign rather, you can change the properties or elements of the const value.

Few Rules before naming your variable: 

1. cannot be reserved words
2. can start with letters or  $ or _
3. names are case sensitive

Data Types, 

Hoisting: Is a weird behaviour of moving all the variable declartions to the top.

When I say declaration, it only means declations, not initializations.