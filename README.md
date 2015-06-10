# Truthiness

##Objectives
1. Understand the concept of truthiness in Ruby
2. Understand why the concept of truthiness is significant in programming
3. Learn what is truthy and what is falsey in Ruby

## Introduction

![Truthiness](http://upload.wikimedia.org/wikipedia/en/thumb/8/85/Truthiness.png/300px-Truthiness.png)

Many programming languages, including Ruby, have native boolean (true and false) data types.  In Ruby they're called `true` and `false`. 

These boolean values come in handy in programming when we want to implement flow control. We're going to learn more about this later, but for now, just understand the flow control is the idea that we can tell our program to execute certain lines of code based on certain conditions. 

###Booleans and Flow Control

For example, *if* I am tired, I will take a nap. Otherwise, I will keep reading this insightful and informative readme. You could also think of this example in the following way: 

If it is *true* that I am tried, then I will take a nape. If it is *false* that I am tired, then I won't take a nap. 

Flow control is predicated on boolean, or true and false, values. 

What this example amounts to is this: we want to be able to use non-boolean values (like strings or integers) in a boolean context. We want to be able to say: if a certain statement *evaluates* to true, or is "truthy", execute certain lines of code. 

Consequently, Ruby must have a way of determining what counts as true, or what is "truthy" and what counts as false, or "falsey". 

Remember, don't worry about understanding flow control and implementing it right now. This is just to provide some background on why we care about the conecpt of truthiness in Ruby. 

## What's truthy and falsey in Ruby?
Programming languages are software, too! That means the people who built Ruby had to decide what is truthy and what is falsey. Different languages make different decisions.

**In Ruby only false and nil are falsey.  Everything else is truthy (yes, even 0 is truthy).** 

Become familiar with the following chart:

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

###Bonus: Determining Truthiness
If you forget to memorize this handy chart, there is a trick you can use to determine if a value is truthy or falsey. 

**The double bang operator:** We've already seen that a single bang operator, `!`, will negate value. A double bang operator, `!!`, will return `true` or `false` based on whether a value is truthy or falsey to begin with. 

For example: 

```ruby 
!!"hello"
  => true
!!nil
  => false
```

## Resources
* [JFarmer's Gists](https://gist.github.com/jfarmer/) - [Truthy and Falsey in Ruby](https://gist.github.com/jfarmer/2647362)
