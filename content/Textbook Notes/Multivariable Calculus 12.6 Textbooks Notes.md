Status: Child

![[12.6.pdf]]

## Formulas 



## Cylinders and Quadric Surfaces 12.6

- The definition for a cylinder is a descriptive one, involving a curve and a vector $\vec{v}$ such that the family of lines passing a point on the given curve parallel to $\vec{v}$ form a cylinder. In the examples discussed, the direction vector $v= <0,0,1>$, namely, the lines are parallel to the z-axis, and the equations in the examples are $y=x^2$ and $f (x, y) = c$ respectively. Note that z does not appear explicitly.  
- One should think of a surface as given in terms of two parameters. In the example of $y = x^2$, one can treat x and z as parameters so a parametric equation for this cylinder is $(x, z) → (x, x^2, z)$. If a curve is given in parametric form: $x = f (s), y = g(s), z = h(s)$ and $v = <v_{1}, v_{2}, v_{3}>$ is to be the direction vector for the lines used to construct the cylinder , then a parametric equation for the cylinder would be $(s, t)  → (f (s) + tv_{1}, g(s) + tv_{2}, h(s) + tv_{3})$.  
- The graph of a function of two variables gives rise to a surface. For example the graph of $z = x^2 + y^2$ is a kind of paraboloid. One can think of this in terms a parametric surface $(x, y)  → (x, y, x^2 + y^2)$. Sometimes a surface is given implicitly from solving one equation of the form $f (x, y, z) = 0$. Here one thinks of solving one of the variables in terms of the remaining two variables. The simplest example is when $f (x, y, z)$ takes the form a linear function $ax + by + cz + d$. For example, the plane equation $2x − 3y + z − 4 = 0$ can be solved as $z = 4 − 2x + 3y$.  
- When $f (x, y, z)$ is a quadratic function of $x, y, z$, the surface given by $f (x, y, z) = 0$ is called a quadric surface. A general quadratic function of $x, y, z$ is a sum of multiples of $x^2, y^2, z^2, xy, yx, xz, x, y, z, 1$; this section focuses on the simpler case when the terms $xy, yx, xz$ are not present. The equation for a sphere has such a form: $(x − x_{0})^2 + (y − y_{0})^2 + (z − z_{0})2 = R^2$ takes the form of $x^2 + y^2 + z^2 − 2x_{0}x − 2y_{0}y − 2z_{0}z + x_{0}^2 + y_{0}^2 + z_{0}^2 − R^2 = 0$. The coefficients of $x^2, y^2, z^2$ are all the same: 1. When the coefficients of $x^2, y^2, z^2$ are not all the same, for example, when $f(x, y, z) = Ax^2 + By^2 + Cz^2 + Dz − E$, where $A, B, C$ are not all zero, the equation $f (x, y, z) = 0$ gives rise to several commonly encountered quadric surfaces such as ellipsoid, paraboloids, elliptical cones, and hyperboloid.  
- There is no need to memorize the different possible quadric surfaces. They are analogues of ellipses, parabolas, and hyperbolas, but can be more complicated, as in the case of hyperbolic paraboloid in Example 3. One common approach is to study the intersection of such a surface with either the vertical planes $x = d$ or $y = d$ for different values of $d$ or the horizontal planes $z = d$ for different values of $d$. In the case of the equation, $\frac{y^2}{b^2} − \frac{x^2}{a^2} =\frac{z}{c}$ with $a, b, c > 0$, setting $x = d$ for some value $d$, say, $d = 0$ or $d = 1$, one gets an upward opening parabola on such a vertical plane. If one sets $y = d$ for some value $d$, one gets a downward opening parabola on such a vertical plane. If one sets $z = d$ for some value $d$, one gets a hyperbola on such a horizontal plane. This is why such a surface is called a hyperbolic paraboloid 

## Reading Questions/Quizzes 

- Use a similar approach to study the equation $\frac{x^2}{a^2} + \frac{y^2}{b^2} − \frac{z^2}{c^2} = h$ when $h = 1, 0, −1$, respectively, You may take specific values of $a, b, c > 0$ and use GeoGebra or Desmos to plot such a surface. Do you see a case of a cone appearing? 


## References 

[[12.6.pdf]]
[[Multivariable Full Textbook.pdf]]