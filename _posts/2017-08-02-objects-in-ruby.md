---
layout: post
---
## Objects in Ruby
You've probably heard somewhere before that everything in Ruby is an object. This is is indeed true. Anytime you create a variable type in Ruby, it is in fact an object of some class. If you want to see what class an object you're working with belongs to, simply try the `#class` method. It will return to you the class of the object you called the method on, for example `"string".class` will return `String` and `5.class` will return `Fixnum`.

## What is a class?
A Class is pretty much a blueprint for the objects you create in Ruby. It will hold instance variables and instance methods that are unique to that class. You see, when you create an object, you "instantiate" it. In other word, the object you created will be unique, that instance of the class will only hold data that you assign to only that instance. This is where the instance variables come into play, they will hold data unique to that instance of your class, and the instance methods are the methods you can call on those variables. This may sound a little confusing in theory, but it makes a lot of sense. In object oriented laguages such as Ruby, you can use Classes to emulate real life objects. But, enough of theory, let's see a class in action.

```ruby
class Fridge
     def initialize(food)
          @food = food
     end
     def change_food(new_food)
          @food = new_food
     end
end
```

In the above code, I've created a new class called Fridge. It has an initialize method, which runs right when the object is created. In my case, I've decided to initalize my class by setting an instance variable `@food`, an instance variable is distinguished by the @ sign. So now I can create a new instance of fridge `my_fridge = Fridge.new('chicken')`. I've assigned a food to the `@food` instance variable with my initialize method. Now this instance variable will hold the food variable I assigned until I call the instance method #change_food. This can be done like: `my_fridge.change_food('potato')`, now the instance variable changed its value to 'potato'.

## Here comes the cool part:
I can create a second instance of Fridge, `my_other_fridge = Fridge.new('apple')`. This new instance will hold its own unique instance variable `@food` which is now set to 'apple'. This leaves the other Fridge object completely untouched, meaning I can create as much Fridge's as my heart desires, just like in real life where you can have many fridges that have different foods, but the fridges all work the same way!

## Go make some Classes!
I really hope this gave you a basic idea of what classes are. Of course the above was a very small example of what the powers of classes are. If you want to get more used to them, I say you practice by writing some classes and get instantiating! Happy coding!
