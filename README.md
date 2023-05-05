Download Link: https://assignmentchef.com/product/solved-cse271-lab-6-one-exercise-pertaining-to-interfaces
<br>
For today’s lab you will be doing one exercise pertaining to interfaces.   It is just one exercise, and small so you can focus and finish your project, which is due this week!

<ul>

 <li>Lab Requirements</li>

</ul>

Suppose that we have a set of objects with some common behaviors: they could move up, down, left or right. The exact behaviors/implementations (such as how to move and how far to move) depends on the objects themselves. One common way to model these common behaviors is to define an <em>interface. </em>In this case, an you will define an interface called Movable,

with interface methods moveUp(), moveDown(), moveLeft(), and moveRight(), all of which return void. (5 points)




Write two concrete classes – MovablePoint and MovableCircle – that implement the Movable interface. These classes that implement the Movable interface will provide actual implementation to the (abstract) interface methods.

<h2>MovablePoint Class (10 points)</h2>




For the MovablePoint class, declare the instance variables x, y, xSpeed and ySpeed; which represent the x location, y location, speed in the x direction, and speed in the y direction. Make getters and setters for the speed variables only, and one constructor that sets all the (4) instance variables.  XSpeed and YSpeed can be positive numbers only, so make sure you program them accordingly (smart setters). Override toString() to an appropriate representation.  Implement the movable interface with “logical” implementations that utilize these instance variables.

For the MovablePoint, you should be using your ySpeed and xSpeed values for the moveUp/Down and moveLeft/Right methods, respectively. And, you shouldn’t be changing your speed in those methods either (we are ignoring friction and momentum here).  So, for example.  If I have a MoveablePoint with the values

y = 4;  yspeed = 8;

Then, moveUp() would cause y to 12, and moveDown() would change y to -4.

MovableCircle Class (10 points)

For the MovableCircle class, use (have an instance variable of) MovablePoint to represent its center and an integer radius to represent the radius. Override toString() to an appropriate representation.  Implement the Movable interface methods by moving the center MovablePoint using the move methods of that class. For this class, have a single constructor that configures a MovablePoint (4 values to pass to the MovablePoint constructer), and the radius as we demonstrate below in our test program.

Test Program and Demonstration (5 Points)

<table width="0">

 <tbody>

  <tr>

   <td width="765">Write out a single test program, MovableTester, (class with a main method) that includes these test statements and some of your ownMovable m1 = new MovablePoint(5, 6, 10,12);     // upcast System.out.println(m1); m1.moveLeft();System.out.println(m1);Movable m2 = new MovableCircle(2, 1, 2, 20,50); // upcast. Constructor takes in 4 point values and//radiusSystem.out.println(m2); m2.moveRight();System.out.println(m2);</td>

  </tr>

 </tbody>

</table>




In addition, add one “public static” method called chaChaSlide(Movable[]) that takes in a collection of moveable things to your tester, in the same way we had an “average” method in our class example.   This method returns nothing, but moves the objects in the following way listed below. In your main method, call that method with a single collection containing a variety of (at least one of each) points and circles,

<ol>

 <li>Move to the left</li>

 <li>Move to the right</li>

 <li>Take it back now y’all (Move down)</li>

 <li>One hop this time (Move up)</li>

 <li>Move to the left</li>

 <li>Take it back now y’all (Move down)</li>

 <li>One hop this time (Move up)</li>

 <li>To the right (Move right)</li>

 <li>To the left (Move left)</li>

 <li>Take it back now y’all (Move down)</li>

 <li>One hop this time, one hop this time (Move up x 2)</li>

</ol>

<h1></h1>