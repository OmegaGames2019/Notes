
Status: 

![[15.7.pdf]]

## 15.7 Triple Integrals in Cylindrical and Spherical Coordinates

We have already seen double integrals where the domain is expressed in polar coordinates. This section introduces triple integrals in both cylindrical and spherical coordinates. Again, the motivation is that many situations have a natural symmetry to them which make non-rectangular coordinate systems more convenient. We may get less complicated limits of integration, a simpler integrand, or both. 

One very important thing to notice is that there are extra factors which show up in the integrand when you change coordinate systems. So not only do you need to rewrite the function using techniques similar to the ones we discussed for polar integrals, you also get an extra factor of $r$ (for cylindrical, just like it was for polar) or $\rho^2\sin \phi$ (for spherical). Section 15.8 (Substitution in Multiple Integrals) will give a more systematic reason for the presence of these factors (from the Jacobian of the change of variables; see **Example 1** in 15.8 for polar coordinates and the computations for cylindrical and spherical right above Figure 15.65), but these two specific cases have intuitive geometrical explanations based on the volumes of the cylindrical wedges (when a partition is done in cylindrical/spherical coordinates, the associated shape of each rectangular box in these coordinates are these wedges). 

![[Spherical Coordinate System]]

Find the following definitions/concepts/formulas/theorems: 

- Definition of cylindrical coordinates 
- Equations relating rectangular and cylindrical coordinates 
- Cylindrical wedge 
- Definition of triple integral in cylindrical coordinates 
- Definition of spherical coordinates 
- Equations relating rectangular, cylindrical, and spherical coordinates 
- Spherical wedge definition of triple 
- Integral in spherical coordinates 

As with many of the multiple integrals we have already seen, the hardest part is setting up the integral. One consideration is to think about which way of decomposing the solid is easier to describe: as stacks of thin columns associated with one of the coordinates, say, $z$ in cylindrical coordinates, or $\rho$ in spherical coordinates, or as stacks of two-dimensional slices "perpendicular to" a coordinate? 

We use the solid enclosed by $z=8-x^2-y^2$ and $z=x^2+y^2$ to illustrate this. The two graphs intersect along $8-x^2-y^2=x^2+y^2$, which gives $x^2+y^2=4$. We can think of this solid as stacks of vertical columns whose heights at $(x,y)$ ranges from $x^2+y^2$ to $8-x^2-y^2$ for every $(x,y)$ with $x^2+y^2\leq{4}$. In terms of cylindrical coordinates, this is for every $0\leq r\leq{2}$ and $0\leq\theta \leq 2\pi$, the heights $z$ ranging from $r^2$ to $8-r^2$.

### Reading Questions/Quizzes

1. Sketch the region described by the following cylindrical coordinates in three-dimensional space. $$0\leq r\leq{4}\cos\theta,\text{ }0\leq\theta\leq \frac{\pi}{2},\text{ }0\leq z\leq{5}$$
2. Sketch the region described by the following spherical coordinates in three-dimensional space. $$1\leq\rho\leq 2\sec \phi, \text{ }0\leq \phi\leq \frac{\pi}{4}$$
3. $D$ is the right circular cylinder whose base is the circle $r=2\sin\theta$ in the $xy$-plane and whose top lies in the plane $z=4-y$. Set up the iterated integral for evaluating $\iiint_{D}f(r,\theta,z)rdzdr d\theta$ over the given solid region $D$. 
4. For the following question, **(a)** find the spherical coordinate limits for the integral that calculates the volume of the given solid and then **(b)** evaluate the integral: The solid between the sphere $\rho=\cos \phi$ and the hemisphere $\rho=2,\text{ }z\geq 0$. 
5. For the following question, **(a)** find the spherical coordinate limits for the integral that calculates the volume of the given solid and then **(b)** evaluate the integral: The solid enclosed by the surface $\rho=1-\cos \phi$. 