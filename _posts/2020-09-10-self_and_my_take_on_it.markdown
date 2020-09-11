---
layout: post
title:      " SELF AND MY TAKE ON IT"."
date:       2020-09-10 23:39:37 -0400
permalink:  self_and_my_take_on_it
---



Self is has being one of the topics tha was not as easy to learn as others while learning Ruby, the word self in ruby is pretty much a conductor that will give you  back information about the object "itself" and the object that is receiving the message. This is clearly a little confusing and if you are new in thee coding world it will require some extra thinking. The first time you will see self (at least for me ) it was while creating a class method, like the next one;

#### Class method:

```
class Human 
  
def self.test 
  print "Hi, "
  puts "#{self}"
  
end 
end

puts Human.test
puts self

-> Hi, Human
->
->Main
```

In the context of a class, `self` refers to the current class, which in this case is `Human`  but using self outside the context of the class will retunr you the higher level of the program( `main` )

To explain this a bit more clearly or at least to try when you use `self` in Ruby you are calling into a comunication process where there will be 2 parts: the sender and receiver( I know super redundant names ), these both parts will try to comunicate in acordance with the circunstances/contexts they are, the most common context would be 
inside or outside of a `class`/`module`/`method` and learning what is the return or the behavior of self on each case is the key to understand a bit better its function and behavior. 

						
		context 				
class	->	inside				
						
module	->	inside	->	self 	->	class/module
						
method	->	outside				
						
		context 				
class	->	outside				
						
module	->	outside	->	self 	->	main
						
method	->	outside				
						
		context 				
class	->	outside/inside				
						
module	->	outside/inside	->	self 	->	object
						
method	->	inside				


This is my understanding if this. Hope it helped you a bit understand or learn a bit more about Ruby/self.





