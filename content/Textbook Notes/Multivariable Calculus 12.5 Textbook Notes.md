Status: Adult

![[12.5.pdf]]

## Formulas 

- A vector equation for the line $L$ through $P_{0}(x_{0},y_{0},z_{0})$ parallel to a nonzero vector $v$ is $r(t)=r_{0}+tv, -\infty<t<\infty$, where $r$ is the position vector of a point $P(x,y,z)$ on line $L$ and $r_0$ is the position vector of $P_{0}(x_{0},y_{0},z_{0})$
- The standard parametrization of the line through $P_{0}(x_{0},y_{0},z_{0})$ parallel to a nonzero vector $v=v_{1}i+v_{2}j+v_{3}k$ is $x=x_{0}+tv_{1},y=y_{0}+tv_{2},z=z_{0}+tv_{3},-\infty<t<\infty$
- The distance from a point $S$ to a line through $P$ parallel to $v$ is $d=\frac{|\vec{PS}\times v|}{|v|}$
- The plane through $P_{0}(x_{0},y_{0},z_{0})$ normal to a nonzero vector $n=Ai+Bj+Ck$ has: 
	- Vector equation: $n\cdot  \vec{P_{0}P}=0$
	- Component equation: $A(x-x_{0})+B(y-y_{0})+C(z-z_{0})=0$
	- Component equation simplified: $Ax+By+Cz=D$, where $D=Ax_{0}+By_{0}+Cz_{0}$
- Distance from a point $S$ to a plane through a point $P$ with a normal $n$ is $d=|\vec{PS}\cdot \frac{n}{|n|}|$

## Lines and Planes in Space 12.5

- Identify the two elements used in constructing a line in space.  
	- A point and a direction vector 
- Given two points $P=(x_{0},y_{0},z_{0})$ and $Q=(x_{1},y_{1},z_{1})$, identify a vector giving the direction of the line passing through P and Q 
	- $\vec{PQ}= <x_{1}-x_{0},y_{1}-y_{0},z_{1}-z_{0}>$
- How many equations are involved in a parametric equation for a line? How many parameters are involved? 
	- Three parametric equations, one parameter ($t$) 
- Is it possible to use one of the coordinates as a parameter in the parametric equations of a line? If so, how to do that? 
	- Yes, if for example $x=t$, you can substitute $t$ for $x$ and rewrite $y$ and $z$ in terms of $x$ 
- Can you use the distance formula from a point to a line to find the height of the triangle with P, Q, R as vertices and PQ as a base? 
	- ![[Height of triangle defined by vectors]]
- Identify the two elements used in constructing a plane in space. 
	- A point on the plane and its "tilt", defined by a vector normal to the plane 
- Learn the vector equation, component equation, and component equation simplified for a plane. 
	- See formulas section 
- Can you write a simplified component equation for a plane in a vector equation form? 
	- $\vec{n} \cdot (r - P_0) = 0$
- Can you find a normal to the plane passing through three given points in space (study Example 7)?  
	- Yes. Given three points $P,Q,R$, construct two vectors with the same initial point (eg. $\vec{PQ}$ and $\vec{PR}$). These two vectors define a plane. Taking the cross product of these two vectors results in an orthogonal (normal) vector to the plane 
- How many equations are involved in the equation for a plane in space? Can you describe a plane in parametric form? If so, how many parameters would be involved?  
	- Three equations, two parameters 
	- $$\begin{cases}
x=x_{1}+su_{1}+tv_{1} \\
y=y_{1}+su_{2}+tv_{2} \\
z=z_{1}+su_{3}+tv_{3}
\end{cases}$$
- Given two intersecting planes, it will form a line (unless the two planes are identical). How do you find a direction vector for this line? How do you find a parametric equation for this line? (Study Examples 8 and 9). 
	- Given two intersecting planes with normal vectors $n_{0}=x_{0}j+y_{0}i+z_{0}k$ and $n_{1}=x_{1}i+y_{1}j+z_{1}k$, the direction vector is the vector orthogonal to $n_{0}$ and $n_{1}$, or $n_{0}\times n_{1}$
- How do you find the intersection of a line with a plane? (Study Example 10) 
	- Substitute the equation of the line into the equation of the plane and find the value of $t$ that satisfies the equation. Then, plug that value into either of the two equations to find the resulting point 
- Study the distance formula from a point to a plane.  
	- See formulas section 
- Study the definition of angle between two planes and the illustration in Figure 12.44, in which an angle between two lines lying in the two planes respectively is also labeled as the angle θ between two planes. Note that these two lines are orthogonal to the line of intersection of the two planes. Can you justify this? Can this hold if one or both lines are not orthogonal to the line of intersection of the two planes? 
	- This can be justified because the angle between the two planes is the same as the angle between their normal vectors since the two lines lying in the two planes are parallel to those normal vectors. 
	- However, if one or two of these lines are not orthogonal to the line of intersection, they are not parallel to the normal vectors of the planes and thus do not represent the angle between the two planes 

## Reading questions/quizzes 

- Find parametric equations for the line through P = (1, −2, 1) and Q = (−1, 0, 1). 
	- $$\begin{cases} 
x=-2t+1 \\
y=2t-2 \\
z=1
\end{cases}$$
- Find the distance from origin to the line in the previous part 
	- ![[Distance from point to plane]]
- Find an equation for the plane through P = (1, −2, 1), Q = (−1, 0, 1), and R = (1, 2, 1) (in both vector form and simplified component form) and identify a normal vector of this plane.  
	- ![[Forming a plane from three points]]
- Find the distance from origin to the plane in the previous part. Is this distance smaller or bigger than the distance in part 2?
	- $D=\frac{|1\cdot 0-1|}{\sqrt{ 1^2 }}=1$
	- The distance is smaller than the distance in part 2 


## References 

[[12.5.pdf]]
[[Multivariable Full Textbook.pdf]]