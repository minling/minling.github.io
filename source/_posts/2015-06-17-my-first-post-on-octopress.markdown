---
layout: post
title: "My First Post On Octopress"
date: 2015-06-17 20:50:57 -0400
comments: true
categories: Flatiron School
---
#1. Introduction

#2. .tap for Ruby 
scroll to the end to read about .tap for Ruby
 

## Why am I at Flatiron?

Hi there! My name is Minling and I just graduated with a bachelors in Biomolecular Sciences. Although I love biology and its cute little microorganisms, I was always into technology. More often times than not have I said "wow wouldn't it be cool if I built this...", "oh wait nevermind, I don't even know how to get code." 

**Time is a limited resource, and if lost, it will never be found.**

With a finite number of heartbeats in a lifetime, and a finite amount of hours in a day, there is just absolutely no time to waste. People ponder for a long time whether they have taken that risk, but that is just too much time spent being indecisive. 
![Nike just do it](http://brandchannel.com/wp-content/uploads/2013/07/Nike-JustDoIt-560.jpg)

What if you just did it?

If you fail, it'll be a great lesson to learn, but if you don't, you win.

>**“Any chance not taken is an opportunity missed.”
― Ken Petti**

Of course it is said easier than done. You can sit there all day looking at motivational quotes but until you make that first step, you aren't actually listening to any of it.

Some people have lateness issues but it isn't because they don't care enough to change, or respect other people's time. They may have other issues in their life that prevents them from realizing the importance of being on time. No matter how much they are told to be on time, they will never be on time, because they have't gotten to that realization yet. People can't be progammed to change, it is up to their own will.

There are people who are creators and others who just want to experience the creations. I want to be a creator of beautiful things. I want to build meaningful, memorable apps that would make someone's life easier or something cool that people would use. I want to make a dent in this world with my creations. 

Sometimes when times get hard, I fall back to pondering whether I have made the right decision, because I made a drastic change in my life to learn to code. I could have stayed in biology and tried to go forward in my career, but I wouldn't be able to bring my crazy ideas to reality. I guess I'll never know until it all happens.


>“You can’t connect the dots looking forward; you can only connect them looking backwards. So you have to trust that the dots will somehow connect in your future. You have to trust in something — your gut, destiny, life, karma, whatever. This approach has never let me down, and it has made all the difference in my life.”
>
~ Steve Jobs

## #tap dat ...

A few times I encountered the usage of #tap in Ruby. 
> tap{|x|...} → obj
> 
> Yields self to the block, and then returns self. The primary purpose of this method is to “tap into” a method chain, in order to perform operations on intermediate results within the chain.

Although that is the definition of the Ruby Doc, it isn't quite clear on how to use it, at least it wasn't clear to me.

Essentially, this is what .tap does
```ruby
class Object
  def tap
    yield self
    self
  end
end
```

```ruby 
def cats
  array = ['paws', 'furry', 'cute']
  array.reverse!
  array
end
#=> ["cute", "furry", "paws"] 
```
Using .tap will achieve the same in one line.

You can use the object to do something, and then it wil return itself at the end. 

```ruby 
def cats
  ['paws', 'furry', 'cute'].tap(&:reverse!)
end
#=> ["cute", "furry", "paws"] 
```

![cats](https://igcdn-photos-c-a.akamaihd.net/hphotos-ak-xaf1/t51.2885-15/11335852_1441788479455650_419649704_n.jpg)
Kitty: "Smells like a good method." 