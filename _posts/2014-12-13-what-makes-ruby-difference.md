---
layout: post
title: "What makes ruby difference ?"
modified:
categories: 
excerpt: "A dynamic, open source programming language with a focus on simplicity and productivity. It has an elegant syntax that is natural to read and easy to write."
tags: [ruby,ruby-lang]
image:
  feature: logo-ruby-intro.png
date: 2014-12-13T15:18:27+07:00
---


A dynamic, open source programming language with a focus on simplicity and productivity. It has an elegant syntax that is natural to read and easy to write.


{% highlight yaml %}
# Output "I love Ruby"
say = "I love Ruby"
puts say

# Output "I *LOVE* RUBY"

say['love'] = "*love*"
puts say.upcase

# Output "I *love* Ruby"
# five times
5.times { puts say }
{% endhighlight %}

#### Overview

Ruby language was designed and developed in the mid-1990s by Yukihiro "Matz" Matsumoto in Japan.

on Oct 08 2014, the lastest version is 2.1.3. This release contains a change of full GC timing to reduce memory consumption, and many bugfixes.

#### Ruby is considered as a slowly language

Yes, it's the truth. But when you choose a language, you are not only care about speed or performance, it depends on kind of application you going to develop.

If it have a realtime features or high complexity algorithms, you really need speed. In otherwise, you haven't any features really need speed, you should think about stability, flexibility, simplicity ... and the community to help you.

<div class="full zoomable"><img src="/images/ruby-benchmark_comparison.png"></div>
#### Ruby is a open source programming language

Ruby have a large community contribution because it's a open source language, any time you need help you can ask them or finding yourself in the very big questions library asked by another ones.

#### Ruby have brief and nature syntax but it can do alot of things

{% highlight yaml %}
 "1 + 2 = #{1 + 2}"    #=> "1 + 2 = 3"

"" << 197 # add decimal value 304 to a string

if a.nil? then puts "Nothing here" else "Something here" end

{% endhighlight %}

Ruby is high object-oriented programing language, almost everything is object. And as you know, object have the attributes and methods so we can call it in simple way and pretty look, eg:

{% highlight yaml %}

moment = Time.zone.new # Create new Time with zone
moment.hour # Get current hour
moment.min # Get current minute
moment.sec # Get current second

{% endhighlight %}

#### Ruby Procs And Lambdas

As you know, almost everything in ruby is an object. So, blocks are not objects, but you can turn them into objects without too much trouble. We do this by wrapping our block in an instance of the Proc class ( or Lambda )

Proc is the standard way to create any object, you simply need to pass in a block and you will get back a Proc object which will run the code in the block when you invoke its call method.

{% highlight yaml %}

proc_object = Proc.new {puts "I am a proc object"}
proc_object.call

{% endhighlight %}

Lambda is likely Proc, but a bit of difference. With blocks and lambdas you can make everything you need

{% highlight yaml %}

block_var = my_method {puts "hello block"}
block_var.call

{% endhighlight %}

**So**
> “I think ruby is a bit of strange, but so interesting and awesome !”
