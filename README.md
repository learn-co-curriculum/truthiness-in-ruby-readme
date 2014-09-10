---
tags: readme
language: ruby
resources: 0
track: web development
topic: ruby
unit: control flow
lesson: truthiness
---

# Truthiness

## Introduction

Many programming languages, including Ruby, have native boolean (true and false) data types.  In Ruby they're called `true` and `false`. 

But oftentimes we want to use a non-boolean value (integers, strings, arrays, etc.) in a boolean context (if statement, &&, ||, etc.).  So someone designing a language has to decide what values count as "true" and what count as "false."  A non-boolean value that counts as true is called "truthy," and a non-boolean value that counts as false is called "falsey."

*Remember*: only true and false are booleans.  nil is not a boolean.  0 is not a boolean.  [1,2,3] is not a boolean.  The string "apple" is not a boolean.  When used in a context where a boolean is expected, Ruby evaluates them as boolean.

## What's truthy and falsey in Ruby?
Programming languages are software, too! That means the people who built Ruby had to decide what is truthy and what is falsey. Different languages make different decisions.

In Ruby only false and nil are falsey.  Everything else is truthy (yes, even 0 is truthy).

| Value        | Truthy? |
|:------------:|:-------:|
|0             | yes     |
|"hello"       | yes     |
|nil           | no      |
|6.7           | yes     |
|true          | yes     |
|false         | no      |
|[1,2]         | yes     |
|{:hi=>"there"}| yes     |

You get the idea!
