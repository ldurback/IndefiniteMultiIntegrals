# Indefinite Multiple Integration of Scalar and Vector Differentials

Given a coordinate system and an n-volume whose lines are aligned with the coordinate grid, we can form the definite multiple integral of a large class of differentials by the method of computing an indefinite integral, which is evaluated only at the corners of the boundary of the n-volume.  For an n-volume whose lines are not aligned with the coordinate grid, we can first approximate the n-volume as one whose lines are aligned with the coordinate grid.  This allows us to take approximate multiple integrals of a large class of differentials.

I will be using Clifford's Vector Algebra

# Examples

For x, y either scalars or vectors

<img src="https://latex.codecogs.com/gif.latex?\int&space;\int&space;x^{-2}&space;y&space;dx&space;dy&space;=&space;-\frac{1}{2}&space;x^{-2}&space;y&space;x&space;y" title="\int \int x^{-2} y dx dy = -\frac{1}{2} x^{-2} y x y" />

Letting <img src="https://latex.codecogs.com/gif.latex?F(x,y)&space;=&space;-\frac{1}{2}&space;x^{-2}&space;y&space;x&space;y" title="F(x,y) = -\frac{1}{2} x^{-2} y x y" />, we can compute the following definite integral (for either scalars or vectors)

<img src="https://latex.codecogs.com/gif.latex?\int_{y_1}^{y_2}&space;\int_{x_1}^{x_2}&space;x^{-2}&space;y&space;dx&space;dy&space;=&space;F(x_2,&space;y_2)&space;-&space;F(x_2,&space;y_1)&space;&plus;&space;F(x_1,&space;y_1)&space;-&space;F(x_1,&space;y_2)" title="\int_{y_1}^{y_2} \int_{x_1}^{x_2} x^{-2} y dx dy = F(x_2, y_2) - F(x_2, y_1) + F(x_1, y_1) - F(x_1, y_2)" />

Similarly, we can form this integral over any other area whose boundary is aligned with the coordinate grid by evaluating F(x,y) at the corners of the boundary and alternately adding and subtracting these values.
