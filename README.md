# Math-Epitech
Projets de mathématique réalisés en Python

101pong:
The goal of this project is to work on a 3D version of this game (or of the Breakout game by the way. . .). Only
one bat will be considered, moving only in the 0-altitude plan (which happens to be (Oxy)).

102architect:
The goal of this project is to develop an application to compute points images in the plan after several
transformations. To make it nice and clean, you chose to use homogeneous coordinates. How clever of you.
O being the origin of both axis, here are the transformations to be implemented:
• Translation,
• Scaling,
• Rotation centered at O,
• Reflection over any axis that passes through O,
• Any combination of the previous transformations.

103cypher:
There are a lot of methods to encrypt a message, from the simplest (such as the 2,000-year-old Caesar
cipher) to the most complex (such as the World War 2 Enigma code); they all need both encryption and
decryption keys (sometimes identical).
In some cases (such as the Hill cipher), the key is represented by a matrix.
You have to carry out such a matrix-based ciphering software, using the following process to encrypt :
• Transcript the key into numbers using the ASCII table,
• Convert the numbered key into a square matrix, the smallest possible size, and filling the lines first,
• Transcript the clear message into numbers using the ASCII table,
• Convert the numbered message into a matrix; its number of columns should fit the key matrix size,
and its number of lines should be as small as possible,
• Multiply the 2 matrices, and write the answer linearly to get the encrypted message

104intersection:
To create synthesis images (when doing ray tracing, for example), potential intersection points between
light rays and scene objects (here cylinders, spheres and cones) must be computed. This is exactly what
you have to do in this project.
To do so, you need to write a 3 dimensional equation of the considered surface, and inject into it the equation of the straight line representing the light ray. You’ll get a quadratic equation, with 0, 1, 2 or an infinite
number of solutions that will give you the intersection points coordinates.
The straight line is defined by the coordinates of a point by which it passes through and the coordinates of
a parallel vector.
O being the origin of the coordinate system, and X, Y and Z the axis, the surfaces that must be handled
in this project are:
• O-centered spheres,
• Cylinders of revolution around Z axis,
• Cones of revolution around Z axis which apex is O.

105torus:
Drawing circles, cylinders and cones is a good start for an image synthesis software, but one have to admit
it is not fully satisfying. . . This project is the continuation of the previous one, and should allow you to draw
more complex forms, such as a torus, which do not emerge from 2nd degree equations, but from superior
degree equations (4th degree in the torus case).
The objective of this project is to solve a 4th degree equation: a4x4 +a3x3 +a2x2 +a1x1 +a0 = 0. A direct
resolution method does exist (Ferrari’s method), but does not generalize. Thus, we will rather compare 3
iterative algorithms:
• The bisection method,
• Newton’s method,
• The secant method.

106bombyx:
In the 70’s, chaos theory opened the way for a better understanding of the evolution of some animal
species. Butterflys for instance. Let’s look at. . . bombyx.
If a generation is crowded, chances are that the next generation will be crowded too, regarding the natural rules of reproduction. But resources may lack for this new generation, so it may not be able to develop.
Therefore, the number of bombyx depends on those two contradictory factors, and its evolution is far from
trivial.

Let’s call xi the number of the ith generation of butterflys.
Here is a model for the evolution of xi:(x1 = n where n is the number of first generation individuals
xi+1 = kxi * (1000−xi / 1000), for i ≥ 1, k being the growth rate, from 1 to 4.

In order to study this evolution, you are asked to plot two things:
• The curve representing the number of individuals in relation to the generation (varying from 1 to 100);
• A synthetic scheme summing all the results for a given n; it consists in plotting every value of xi
(between two given bounds), in relation to k (k varying from 1 to 4 by 0.01 steps).
In both cases, your program shall print on the standard outuput the values to be entered into gnuplot to
draw the graphes.
