---
layout: posts
title: Ruby Classes and Modules
subtitle: Sorta The Same, But Not
categories:	blogs
---
Modules and Classes are both vital parts of the Ruby language. We've learned how to require relative files, include methods in ohter classes, and access variables across our program architecture. Knowing all of the above, what and why are Modules useful?

We know that Ruby classes are specific to their methods, each of which step the Class to achieve a singular goal. Modules can also hold classes, but are considered more as a "Library" of classes to reference during coding a class. Modules also work with the concept of inheritance, where classes can inherit from super classes. Sounds confusing? Not really, but lets look at some code and feel it out:

<pre>
class Vehicle
                attr_accessor :type, :make, :model, :miles
            end

            class Car < Vehicle
                def initialize(make, model)
                    @make = make
                    @model = model
                end

                def describe
                    puts "This car is a #{@make}, #{@model}."
                end
            end

            module New
                def describe
                    puts "This car is a #{@make}, #{@model}."
                    puts "This car has 0 miles, and is new!"
                end
            end

            class New_Car < Car
                include New
            end


            used_ferrari = Car.new("Ferrari", "125 S")

            new_ferrari = New_Car.new("Ferrari", "458")


            p used_ferrari.describe

            p new_ferrari.describe
        

            # This car is a Ferrari, 125 S.

            # This car is a Ferrari, 458.
            # This car has 0 miles, and is new!
</pre>
In the code above, we can see that classes and modules are very similar, and work with each other. Classes are specific, and need to do specific things. Modules extend the power of simplicity by allowing other code to be included, giving the class more versatility but keeping it clean. Again, we can think of modules as "libraries", that will house code to be called in our later classes. The module is a collection of related methods and classes and can be refereed to sort of like using an include.

Though Object Oriented Programming can get quite deep, the tools, design, and tactics we can use using it can truly help our "better design" development move forward.

Lets make pretty code, and keep it that way.