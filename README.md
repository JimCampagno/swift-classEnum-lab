# Enums Dinosaurs Lab 

![Dino](http://i.imgur.com/ukpn5w3.jpg)

> Let your heart guide you. It whispers so listen closely. -[Littlefoot's Mother](http://www.imdb.com/title/tt0095489/?ref_=ttqt_qt_tt)

## Overview

In this lab, you'll implement a few simple classes using enums. 

## Instructions

This lab is all about classes and enums! In this lab, you'll implement a few simple classes using enums. As usual, a set of tests have been written for you. If you follow the directions in this lab correctly, the tests will pass.

Get started by opening up `ClassesNenums.xcworkspace` in Xcode. Go ahead and run the tests by **Test** from the **Product** menu, or pressing <kbd>Command</kbd>+<kbd>U</kbd>. Right now, you'll see that the tests fail, but if you finish this lab, the tests should pass.

Let's go!

1. First, open up `Bird.swift` in Xcode's code editor. You'll be making a lot of changes in this file.
2. To complete this lab, you'll need to implement three enums. The first one should be called `Speed`. This enum is used for comparison and has _raw values_, so it should inherit from `Int`. It should have three cases: `Slow`, `Medium`, and `Fast`. Create this enum now, in `Bird.swift`.
3. Implement a method for your `Speed` enum called `isFaster(thanSpeed:)`. This enum should take a `Speed` paramater and return true if the enum value that `isFaster(thanSpeed:)` is called on is faster than the parameter. For example:
	* `Speed.Slow.isFaster(thanSpeed: Speed.Medium)` should return `false`.
	* `Speed.Faster.isFaster(thanSpeed: Speed.Medium` should return `true`.
	* In the case of a tie, the value that `isFather(thanSpeed:)` is called on should be considered "faster" (i.e., the method should return `true`). So `Speed.Faster.isFaster(thanSpeed: Speed.Faster)` should return `true`.
4. Next, create an enum called `Diet`. (This enum does not need to do any comparisons, so it does not need to have any raw values associated with it.) The cases for `Diet` should be `MeatEater` and `Vegetarian`.
5. Then create an enum called `Sex`. The cases of this enum should be `Male` and `Female`.
6. Now it's time to create a new _class_ called `Trex`. Declare that class in `Bird.swift`.
7. Add a property called `speed` to your `Trex` class. This property should be of type `Speed` and should initially be set to `Speed.Fast`.
8. Add a property called `diet` to your `Trex` class. This property should be of type `Diet` and should be set to `Diet.MeatEater`.
9. Add a property called `name` of type `String` to `Trex`.
10. Add a property called `sex` of type `Sex` to `Trex`.
11. Add a property called `isAlive` of type `Bool` to `Trex`. This should initially be set to `true`.
12. Create an initializer for `Trex`. This initializer should take two parameters, `name` and `sex`, and assign those parameters to the corresponding properties.
13. Create a method called `speak()`. This method should return the string ""ROAAAWWWWRRRRR!!!!!!".
14. Create a method called `isFaster(thanTrex:)`. This method should take one parameter of type `Trex`. It should return `true` if the object the method is called on is faster than the parameter.
15. Create a method called `eat(otherTrex:)`. This method should take one parameter of type `Trex`. If the object the method is called on is faster than the parameter, it should "eat" the other `Trex` (by setting the other `Trex`'s `isAlive` property to `false`).

That's it! Try running the tests again. This time, they should pass. If they don't, take a look at these directions again and make sure you implemented everything properly, and keeping hammering away until the tests _do_ pass!

<a href='https://learn.co/lessons/ClassesEnums' data-visibility='hidden'>View this lesson on Learn.co</a>
