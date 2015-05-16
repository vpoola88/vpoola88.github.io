---
layout: posts
title: Enumerable Power
subtitle: #Maps
categories:	blogs
---

Computers are intelligent. Theres no getting around that fact. Computers can do amazing things, and have only served to make what we can do as humans even better. However, much like I've alluded to before, computers are pretty awesome for doing more than flappy bird. Programming is an incredible feat to the tech world. As we go through this journey in DBC, I feel we are going to witness to just how incredible that feat gets.

We all know programming can be difficult, and differ as much from what speaking English is like, to what speaking Choctaw is like (apparently only 10,000 people speak and understand it). The cool thing about English that has been recently brought to my attention is just how versatile it is. You can take some basic foreign words and englishify it, which helps make it a cross cultural language. I can go on and on about English, but I'll save that for another day. Let just focus on how English relates to what we do.

Much link English, Ruby is a very readable and mixable language. There are so many different ways we can write our algorithms, and with so many spins. Ruby has an amazing list of methods, each of which relates to the other to help modify what its interested in. Even better, Ruby has Enumerables. Don't get lost now - its actually not that bad. Enumerables provide a set of methods to help manipulate collections - AKA you can do some cool shit with them and do it quicker.

Lets focus on one enumerable that may make the most sense going into this world. Assuming we all understand arrays in ruby, we should then know that there are multiple ways to iterate through them. Perhaps the most used one would be our friendly Array#Each method. However, each will not return our appended array value unless specified.

In comes MAP. The Enumerable#Map method will take our data set and iterate through the block, but now included the new values for the appended data. This is crucial when modifying larger data sets and having a desired return value.

<pre>
#Map Example!

array = ["Hello", "Goodbye"]

array.map { |n| n + " World!" }

=> ["Hello World", "Goodbye World"]
</pre>

Ma-a-a-a-ps, wait! They don't love you like i love you... -- YEAH YEAH YEAHS