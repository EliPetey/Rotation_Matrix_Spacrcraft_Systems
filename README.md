# Rotation_Matrix_Spacrcraft_Systems
Simple MATLAB powered script that calculates the Rotation Matrix from a given Euler Angle and Euler Axis

**Rotation_1 uses the Euler Axis and Euler Angle**
e is defined as a column vector 
ee' is defined as the outer product it returns a 3x3 matrix
ex is the matrix product. It is not an operation but a definition hence you have to define it within the function. 
For faster computation, define it OUTSIDE the function if you have to repeatedly call the funciton in a loop.

**Rotation_2 uses quaternion elements, without any trigonometric operations**
It is computationally very fast
As you can see from tic and toc, Rotation_2 is significantly faster
However, if computer is lightly loaded, the difference is not really noticeable. It is only when I repeatedly run it by spamming F5 then the true benefits of using Quaternions are shown. Up to 2.779 times faster. 
