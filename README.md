# 1410-Assignment-9
Problem One.  Fun With Mobiles

The project contains a package called "mobiles".  Run the main method in the class MobileExamples.  You should see this:

Mobile1-Default.JPG

This is a rendering of a mobile.  Imagine that the vertical lines are wires, and that the upper wire is attached to the ceiling.  The horizontal lines are unbendable massless rods, and the circles are weights (also called bobs).  The weight of each bob is shown, as is the distance from the ends of each rod to the supporting wire.  We'll call the distance from the left end to the wire the "left distance", and similarly for "right distance".

A rod is balanced when the product of its left distance and the weight hanging from its left end equals the product of its right distance and the weight hanging from its right end.  Every rod in the mobile shown above is balanced, so we say that the mobile as a whole is balanced.

Notice the seven labeled values in the upper left corner of the window.  These values were calculated by the program we have given you.  They have all been calculated incorrectly because the methods that do the calculation are implemented by stubs.  Your job is to replace those stubs with correct implementations.

A correct version of the program would display this view of the mobile above:

Mobile1-Correct.JPG

The illustration is the same, but the seven labeled values are correct.  Here's one more visualization of a slightly different mobile, created by a correct implementation:

Mobile2-Correct.JPG

The only difference is that the bottommost rod has been attached to its wire in a slightly different position.  As a result the rod is unbalanced, and this is shown in the illustration.

Here are the steps you should follow to create a correct implementation of the Mobiles program.

Study the Mobile class, which is used to represent mobiles.  Notice that there are two very different constructors, one for creating bobs and one for creating rods.  

Mobile contains eight methods: display, which draws illustrations like the one above, and seven more, which provide the values that appear in the upper left of the window.  I have provided an implementation of display; your job is to provide implementations of the other seven methods.

A Mobile is a recursive data structure.  So, when you implement the methods, think recursively!  

A Mobile is either a rod or a bob.  A rod contains two simpler Mobiles.  A Bob does not contain any mobiles.

When you implement a method on Mobiles, you will need to have a case for bobs and a case for rods.  In the rod case you will be coding a recursive case that makes two recursive calls.  You will need to figure out how, for example, to define the weight of a rod in terms of the weights of the two Mobiles it supports.  In the bob case, you will be coding a base case with no recursion.

Believe it or not, the seven bob cases and the seven rod cases can each be written with a single return statement and nothing else.  None of the methods is complicated.

You should not modify anything except the bodies of the seven methods that you are implementing in Mobile.  Do not change anything else about this class. 

Have fun with this.  I think you'll be amazed by how much just a little bit of code can accomplish.  And do try to understand why your code works.
 

Problem Two.  File System Methods

The project contains a package called "files" that contains a class called FileSystem.  FileSystem contains correct implementations of three methods from lecture.  It also contains three method stubs.  Those are the ones that you need to implement for the assignment.

FileSystem has a main method that calls the three implemented and the three unimplemented stubs.  There are comments that give the correct result for each call.
 
