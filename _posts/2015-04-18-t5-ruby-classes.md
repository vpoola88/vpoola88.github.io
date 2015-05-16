---
layout: posts
title: A Dogs Tricks
subtitle: The Ruby Class
categories:	blogs
---
From my previous posts, we all know how and why programming in Ruby is awesome. Ruby is an object oriented language by design, meaning that everything is an object. What does this mean, and why does that matter?

Objects are unique in ruby, and can be manipulated by using methods. The Ruby class is a blueprint for an object that we can create. Underneath that class, we have our variables and our methods. Gibberish? Not really.

I hope you all love dogs, because I sure do. Lets talk about classes in Ruby, and how its going to help teach my dog some tricks.

World, meet Jax:

Jax is my best friend, and most loyal compadre, but he also does some pretty cool things to. Jax, of course, is a Dog (class), and has certain attributes (name, breed, color). Jax can also learn and do some pretty neat tricks (speak). Let see what all this looks like in our Ruby Class.

<pre>
	class Dog

                attr_accessor :name, :breed, :color


                def initialize (name, email, password)
                    @name, @breed, @color = name, breed, color
                end

                def meet
                    p "Meet my dog #{name}. He is a #{color} #{breed}."
                end

                def speak
                    "Ruff"
                end

            end

            jax = Dog.new("Jaxson", "Labrador", "Chocolate")

            p jax.meet
            p jax.speak
</pre>

As we can see, Classes are great way to organize a blueprint for our methods, and anything that exists within that class. The code above is very simple. It creates a blueprint for any dog, that will have a name, breed, and color. By calling jax = Dog.new("","",""), I have simply stated that Jax has these 3 characters that are common among all dogs. "jax.meet" is the class's method to introduce you to him, and "jax.speak" returns "Ruff", which is his favorite trick.

Pretty straight forward right? Ruby classes are a great way to work within the object oriented world.