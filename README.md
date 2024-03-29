# Indefinite Multiple Integration of Scalar and Vector Differentials

# NOTE:  I currently only have a theory of integrating polynomial differentials

Given an coordinate system and an n-volume whose lines are aligned with the coordinate grid, we can form the definite multiple integral of a large class of differentials by the method of computing an indefinite integral, which is evaluated only at the corners of the boundary of the n-volume.  For an n-volume whose lines are not aligned with the coordinate grid, we can first approximate the n-volume as one whose lines are aligned with the coordinate grid.  This allows us to take approximate multiple integrals of a large class of differentials.

I will be using Clifford's Vector Algebra, and I will assume flat (Euclidean or Minkowsi) space.


---

# Ingredients

R is the position vector, and dR is its differential.

By "element of the clifford algera", I mean any constant element.

A monomial is any product of elements of the clifford algebra and any number of R's.  The rank of the monomial is the number of R's.

A polynomial is a linear combination of scalars and monomials.  The rank of a polynomial is the largest rank of any of its component monomials.

An elementary monomial differential is a product of monomials and dR's.  The rank of an elementary monomial differential is the number of dR's.

A polynomial differential is any linear combination of elementary monomial differentials of equal rank.

# Equal and Unequal Contractions

Consider any two vectors, v and w, and any element of the clifford algebra, A.

If the coordinate vectors (not components) of v are {v_i} and the coordinate vectors of w are {w_i}, then we can define the equal and unequal contractions v and w in any product vAw as so

<img src="equal contraction definition.png" title="equal contraction definition" />

<img src="unequal contraction definition.png" title="unequal contraction definition" />

We can now epxand vAw in terms of the contractions

<img src="expansion in contractions.png" title="expansion in contractions" />

Note that the equal contraction generalizes the dot product and the unequal contraction generalizes the wedge product.

# Elementary Contracted Monomial Differentials

An elemnentary contracted monomial differential is one where all R's and dR's are fully contracted.

# Indefinite (Multiple) Integral of Polynomial Differentials

To take the indefinite integral of any elementary contracted monomial differential, simply promote any one of the dR's to an R (it does not matter which, all paths to fully integrate a differential lead to the same result), count n_eq_R, the number of R's equally contracted onto that R that was just promoted (including that R), and multiply the result by 1/n_eq_R.

For instance

<img src="monomial integral examples.png" title="monomial integral examples" />

# Computing a Definite Integral from the Indefinite Integral

We can intepret the full indefinite integral of an elementary contracted monomial differential as being a combination of repeated integrations from R=0 and volume integrations.

The equal contraction of multiple dR's corresponds to a repeated integral.  The unequal contraction of multiple dR's corresponds to a volume integral.

Consider a differential of rank n in which all dR's are equally contracted.  In this case, an nth indefinite integral will turn this into a function F(R), which we can use to evaluate an nth repeated definite integral (from R=0) between an arbitrary start and end point as:  F(end) - F(start)

Consider a differential of rank n in which all dR's are unequally contracted.  In this case, an nth indefinite integral will turn this into a function F(R), which we can use to evaluate an n-volume definite integral.  First, approximate the volume of integration as a figure whose lines are along the coordinate axes.  Next, evaluate F(R) at each corner of the approximated figure and alternately add and subtract these values until all corners are covered.


MORE TO COME

Hard to explain :(

---

# Everything below here is old


# Ingredients

Given either coordinate functions <img src="https://latex.codecogs.com/gif.latex?x_i" title="x_i" />'s or basis clifford vectors <img src="https://latex.codecogs.com/gif.latex?x_i" title="x_i" />'s

The basis differentials are the set of <img src="https://latex.codecogs.com/gif.latex?dx_i" title="dx_i" />'s

A monomial is any product of <img src="https://latex.codecogs.com/gif.latex?x_i" title="x_i" />'s.  The rank of a monomial is the number of <img src="https://latex.codecogs.com/gif.latex?x_i" title="x_i" />'s.

A polynomial is a linear combination of scalars (constants) and monomials.  The rank of a polynomial is the largest rank of any of its component monomials.

A linear polynomial (or linear function) is a polynomial with rank 1.

The elemntary differentials I will consider are products of <img src="https://latex.codecogs.com/gif.latex?x_i" title="x_i" />'s, inverses of polynomials, and at least one <img src="https://latex.codecogs.com/gif.latex?dx_i" title="dx_i" />.  The rank of an elementary differential is the number of <img src="https://latex.codecogs.com/gif.latex?dx_i" title="dx_i" />'s in the product.

The differentials we will consider will be linear combinations of elementary differentials of equal rank.

We will call the coordinate functions <img src="https://latex.codecogs.com/gif.latex?x_i" title="x_i" /> (not basis vectors) that appear in the differential, its "parameters".

# Note

With my definition of elementary differential, in each connected component of the domain of a differential, for each parameter <img src="https://latex.codecogs.com/gif.latex?x_i" title="x_i" /> of the element differential, there is at exactly 1 value of <img src="https://latex.codecogs.com/gif.latex?x_i" title="x_i" /> for which the elementary differential is 0 for arbitrary values of the other parameters.  Note also that this value is always 0, infinity, or -infinity.

# The Indefinite Integral

To form the form the indefinite integral of any elemntary differential, the order of integration does not matter, so we can pick any <img src="https://latex.codecogs.com/gif.latex?dx_i" title="dx_i" /> to integrate over first.  All such integrals are equal as long as the n-volume we integrate over is aligned with the coordinate grid.  Second, if need be, we note that, along the grid, <img src="https://latex.codecogs.com/gif.latex?x_i" title="x_i" /> is proportional to <img src="https://latex.codecogs.com/gif.latex?dx_i" title="dx_i" />, and we use the commutation rules of the coordinate basis to simplify the product.  Finally, for any arbitrary point in the domain of the elementary differential, the indefinite integral is that integral that starts at that <img src="https://latex.codecogs.com/gif.latex?x_i" title="x_i" />, for which the elementary differential is 0, and at ends at the arbitrary point.

The indefinite integral of any other differential is equal to the sum of the indefinite integrals of its elementary differentials.

# Note

By my definition of differentials and indefinite integrals, any indefinite integral has 0 scalar term.

# Forming a Definite (Multiple) Integral from the Indefinite (Multiple) Integral

Consider a rank-n differential.  (We'll assume that its parameters are x_1 to x_n) and form its indefinite n-integral I(x_1, ..., x_n)

Next, consider any (oriented) n-volume in the domain of the differential, and approximate it as an (oriented) n-volume that is aligned with the grid.

To evaluate the definite n-integral of the differential over this approximated n-volume, simply evaluate I(x_1, ..., x_n) at each corner of the approximated n-volume's boundary, and alternately add and subtract each value.

# Examples

For x, y either scalars or vectors

<img src="https://latex.codecogs.com/gif.latex?\int&space;\int&space;x^{-2}&space;y&space;dx&space;dy&space;=&space;-\frac{1}{2}&space;x^{-2}&space;y&space;x&space;y" title="\int \int x^{-2} y dx dy = -\frac{1}{2} x^{-2} y x y" />

Letting <img src="https://latex.codecogs.com/gif.latex?F(x,y)&space;=&space;-\frac{1}{2}&space;x^{-2}&space;y&space;x&space;y" title="F(x,y) = -\frac{1}{2} x^{-2} y x y" />, we can compute the following definite integral (for either scalars or vectors)

<img src="https://latex.codecogs.com/gif.latex?\int_{y_1}^{y_2}&space;\int_{x_1}^{x_2}&space;x^{-2}&space;y&space;dx&space;dy&space;=&space;F(x_2,&space;y_2)&space;-&space;F(x_2,&space;y_1)&space;&plus;&space;F(x_1,&space;y_1)&space;-&space;F(x_1,&space;y_2)" title="\int_{y_1}^{y_2} \int_{x_1}^{x_2} x^{-2} y dx dy = F(x_2, y_2) - F(x_2, y_1) + F(x_1, y_1) - F(x_1, y_2)" />

Similarly, we can form this integral over any other area whose boundary is aligned with the coordinate grid by evaluating F(x,y) at the corners of the boundary and alternately adding and subtracting these values.

# Problems with repeated integration

With repeated integration, we can only use the above formulation of the indefinite integral to form definite integrals of the form

<img src="https://latex.codecogs.com/gif.latex?\int_a^b&space;\int_{zero}^x&space;\cdots&space;\int_{zero}^x&space;\omega" title="\int_a^b \int_{zero}^x \cdots \int_{zero}^x \omega" />

where "zero" is that value of x that makes omega = 0.

For instance, <img src="https://latex.codecogs.com/gif.latex?\int&space;\int&space;\int&space;dx^3&space;=&space;\frac{1}{6}&space;x^3" title="\int \int \int dx^3 = \frac{1}{6} x^3" /> only allows us to form the definite integral

<img src="https://latex.codecogs.com/gif.latex?\int_a^b&space;\int_0^x&space;\int_0^x&space;dx^3&space;=&space;\frac{1}{6}&space;b^3&space;-&space;\frac{1}{6}&space;a^3" title="\int_a^b \int_0^x \int_0^x dx^3 = \frac{1}{6} b^3 - \frac{1}{6} a^3" />
