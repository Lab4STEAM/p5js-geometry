# p5js-geometry
Edu scripts in p5js for Geometry.


## PYTHAGOREAN THEOREM
### Statement
Let's consider a triangle having an angle of 90 degrees, called a right triangle.
The opposite side to the right angle is called ***hypotenuse***, the other two sides are called ***cathetes***
The square constructed on the hypotenuse is equal to the sum of the squares constructed on the cathetes.

### Formula
We denote by *c* the hipotenuse, and by *a* and *b* the cathetes.
The formula expressing the theorem is: *c<sup>2</sup> = a<sup>2</sup> + b<sup>2</sup>*

### Graphical representation of the Pythagorean theorem.** 
The values of the cathetes can be changed by assigning different values to variables *a* and *b*.
The square constructed on *a* is divided into 10x10 squares, shown on the square constructed on *c*, so as to identify the corresponding area.
The area in *c* corresponding to the square on *b* is colored like the square built on *b*.
[https://editor.p5js.org/Ambra.c/sketches/NhN3pGVwa]

### Graphical demonstration of the Pythagorean theorem.**
Demonstration of the Pythagorean theorem using the First Euclid's Theorem.
We plot the height of the triangle relative to the hypotenuse. Then we extend it to the point L, creating two rectangles *C1* and *C2*.
- *C1*: one side is equal to *c* and one side is equal to ***projection of b on the hypotenuse***;
- *C2*: one side is equal to *c* and one side is equal to ***projection of a on the hypotenuse***.
For the First Euclid's Theorem the square built on a cathet is equivalent to the rectangle that has as dimensions the hypotenuse and the projection of the cathet on the hypotenuse. 
[https://editor.p5js.org/Ambra.c/sketches/Bh5wKgmgX]



## THEOREM OF THE ANGLE AT THE CENTER AND ANGLE AT THE CIRCUMFERENCE
### Statement
An angle at the circumference is half of its corresponding angle at the center.

### Definitions
An ***angle to the circumference*** is a *convex* angle with the vertex on the circumference and the sides that are secant the circumference (or one secant and the other tangent).
The intersection between the angle and the circumference identifies an *arc of circumference*. It's said that the angle *insists* on the arc or that it is *underlaid* to the arc.
Each angle at the circumference identifies one and only one arc, but each arc is associated with infinite angles to the circumference.
An ***angle at the center*** is any angle that has as vertex the center of the circumference and as sides two semirects intersecting the circumference. It could be convex, flat or reflex.
Given an arc of circumference there is one and only one angle at the center that insists on it.

### Relationship between angles at centre and angles at circumference
Each corner of the circumference corresponds to one and only one angle at the center.
For each angle at the center there are infinite angles at the circumference.

### Demonstration
We draw an angle to the circumference. We call *A* its vertex and *B* and *C* the ends of the arc on which it insists.
We draw the corresponding angle at the center.
We call *D* the point diametrically opposite to *A*.
We must demonstrate that the amplitude of the angle at the center *BOC* is twice the amplitude of the angle at the circumference *BAC*.
- The *triangle AOC* is an isosceles triangle, in fact the sides *OA* and *OC* are the radii of the circumference, so they are congruent.
- An isosceles triangle has the angles at the base congruent. So *OAC* = *OCA*.
- The angle *DOC* is an outer angle, so **DOC = OCA + OAC = 2OAC**.
The same procedure shows that:
- **DOB =  OAB + OBA = 2OAB**
Let us now observe that the angle at the center *BOC* is equal to the sum of *DOC* and *DOB*: **BOC = DOC + DOB = 2OAC + 2OAB = 2(OAC + OAB)**.
So:
                ***BOC = 2BAC***
[https://editor.p5js.org/Ambra.c/sketches/p_1S7pFpV]



## RADIUS AND TANGENT IN A CIRCUMFERENCE
Consider a circumference of unknown radius and a segment of known length tangent to that circumference at point *C*.
We construct a triangle that has vertices at points *A* and *C* and at the origin *O* of the circle.
We call *B* the point of intersection between segment AO and circumference. The lenght of the segment *AB* is known.
We can now calculate the radius of the circumference:
- Because *AC* is tangent to the circle at point ‍*C*, the radius going to point *C* is perpendicular to the tangent line. This means that the measure of ‍the angle in *C* is 90°.
- We use the Pythagorean Theorem to solve it.
- The lenght of the *OA* segment is equal to *AB* plus the *radius*. 
- *OA* is the hypotenuse of the triangle, so: ***OA<sup>2</sup> = OC<sup>2</sup> + AB<sup>2</sup>***.
- ***(AB + OB)<sup>2</sup> = radius<sup>2</sup> + AC<sup>2</sup>***.
- ***AB<sup>2</sup> + radius<sup>2</sup> + 2(ABradius) = radius<sup>2</sup> + AC<sup>2</sup>***.
- ***radius = (AC<sup>2</sup> - AB<sup>2</sup>) / 2AB***
[https://editor.p5js.org/Ambra.c/sketches/JzObxkohu]



## ARC OF A CIRCUMFERENCE LENGHT
Consider a circumference of known radius.
We want to calculate the lenght of an arc of circumference between points *A* and *D*.
Point *A* is part of a line passing through the origin and intersecting the circumference at the opposite side at point *B*.
Point *D* is part of a line passing through the origin and intersecting the circumference at the opposite side at point *C*.
The measure of the angle *alpha* between *A* and *C* is known.
So we can calculate proportionally the lenght of the *AD* arc.
We know that:
- circumference = 2PIr
- 2PI = 360°
- PI = 180°
- *beta* = 180° - *alpha*
We can proportionally solve the arc lenght:
        *arc lenght* / *circumference* = *beta* / 360°
        *arc lenght* = (*beta* / 360°)*circumference*
[https://editor.p5js.org/Ambra.c/sketches/KcZGQorST]



## PERFECT SQUARE OF A BINOMIAL
There is a pattern when we square a binomial:
        *(x + b)<sup>2</sup> = x<sup>2</sup> + 2bx + b<sup>2</sup>*
We complete the square when we have an equation like *x<sup>2</sup> + 2bx = c*, and we find the value *b<sup>2</sup> to add to both sides. Then the left side of the equation becomes a perfect square.
We have a perfect square that starts with *x<sup>2</sup> + ax*
We have to find the missing constant term.
To do this :
- *b* is the missing constant term.
- *x<sup>2</sup> + ax + b = (x + c)<sup>2</sup>*
- *x<sup>2</sup> + ax + b = x<sup>2</sup> + 2cx + c<sup>2</sup>*
- *a = 2c*
- *b = c<sup>2</sup>*
- *c = a/2*
- *b =(a/2)<sup>2</sup>*
So the perfect square is:
        ***x<sup>2</sup> + ax + (a/2)<sup>2</sup>***
[https://editor.p5js.org/Ambra.c/sketches/04q-mexnJ]



## FIBONACCI'S SPIRAL
The Fibonacci sequence is a series of positive integers in which each number is the sum of the two preceding ones.
        ***C<sub>n</sub> = C<sub>n-1</sub> + C<sub>n-2</sub>***
The first two terms of the sequence are both equal to 1, while each term from the third onwards is equal to the sum of the two preceding it.
        ***1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, ...***
La sequenza di Fibonacci è utile anche nel calcolo della ***golden section*** e del ***golden number***.
The golden section is the ratio between two unequal lengths of which the greater *a* is the **mean proportional** between the lesser *b* and the *sum* of the two:
        ***b : a = a : (a+b)***
The golden number is the ratio between *a* and *b*, and is equal to *phi = 1.618*.
The ratio between a number of Fibonacci's sequence and its preceding is, at the limit for n tending to infinity, equal to phi.
The Fibonacci spiral is built from the squares whose sides are the numbers of Fibonacci.by joining an infinity of quarters circumference in these squares you can build a spiral, called - precisely - Fibonacci spiral, able to approximate the golden spiral.
[https://editor.p5js.org/Ambra.c/sketches/gL168xlcMa]



## LOGARITHMIC SPIRAL
The logarithmic spiral is the trajectory of a point moving in *uniformly accelerated motion* on a semi-straight line that *rotates* evenly around its origin. The distance segment between successive turns (the turn pitch) is not constant but increases according to a geometric progression.
Each vector radius will be wider than the previous one according to a constant ratio (logarithmic spirals are also called proportional), therefore the growing curve does not change shape.
This spiral never reaches the pole, because the centre of the spiral is an asymptotic point.
Continuing towards the centre, there are infinite identical spirals on a reduced scale. At the same time, as we move further away from the origin, the size of the spiral increases and it always remains similar to itself.
The angle that the spiral forms with the circles centered at the origin (angle of inclination) is constant.
The property by which the curve performs infinite evolutions towards its center is called *self-similarity*.
[https://editor.p5js.org/Ambra.c/sketches/u82qZTpm8]