
Status: 

![[14.8.pdf]]

## 14.8 Lagrange Multipliers

To find the extreme values of a continuous function defined on a bounded closed region, we need to identify its interior critical points and its possible extreme values on the boundary. In one dimension, a closed interval has only two boundary points. In higher dimensions, however, the boundary of a region most of the time consists of infinitely many points. In two dimensions, the boundary of a region is typically the union of a collection of curves and points; in three dimensions, boundary of a region is typically the union of a collection of surfaces, curves, and points. Finding extreme values of a function on such a boundary is much harder than in one dimension. In some situations, such as shown in **Example 6** of 14.7, one can reduce the problem of finding extreme values of a function on a boundary to a one variable calculus problem, when the  
boundary can be represented as a graph of a function, so one of the variables can be substituted  
in terms of the rest. But this approach has very limited usage.  

The method of Lagrangian Multipliers is used to address this problem. The basic idea of Lagrange multipliers is this: if you want to maximize a function, you want to move in the direction of the gradient from wherever you are. If you are subject to a constraint (i.e. you can only move along a boundary curve or surface), you may not be able to move in the direction of the gradient while staying “in bounds” for the constraint. So you do the best you can and move along your constraint curve (or surface) in the direction “closest” to the gradient direction, namely, the orthogonal projection of the gradient of the function at that point in the tangent line/plane of the constraint. When you get to a place where this projection is zero, namely, when the gradient is orthogonal to the constraint where you are (more accurately, orthogonal to the tangent plane of the constraint), moving in any direction in the constraint won’t increase the function value. So where you are is at least a local maximum subject to the constraint.  

We have two vectors at play here: the gradient of the function f whose extreme values we are looking for and the gradient of the function g whose level set is our constraint. When the gradient $∇f$ of $f$ is orthogonal to the tangent plane of the level set of $g$ at point $x$, we know that $∇f (x)$ is parallel to $∇g(x)$, hence the criterion of Lagrangian Multipliers. Algebraically, this relation is expressed as $∇f (x) = λ∇g(x) \text{ for some } λ.$ 

Of course, the point $x$ also needs to satisfy the constraint equation $g(x) = 0$.  

Find the following definitions/concepts/formulas/theorems:  
- constraint (you have seen this before) 
	- A specific region/domain of a function 
- Lagrange multiplier- general concept 
	- A scalar multiplier of a gradient vector 
- Orthogonal Gradient Theorem 
	- Suppose that $f(x,y,z)$, is differentiable in a region whose interior contains a smooth curve $r(t)=x(t)i+y(t)j+z(t)k$. If $P_0$ is a point on $C$ where $f$ has a local maximum or minimum relative to its values on $C$, then $∇f$ is orthogonal to the curve’s tangent vector $r'$ at $P$.
- Lagrange conditions (in the book this is called The Method of Lagrange Multipliers) 
	- Suppose that $f(x,y,z)$ and $g(x,y,z)$ are differentiable and $\nabla g\neq 0$ when $g(x,y,z)=0$. To find the local maximum and minimum values of $f$ subject to the constraint $g(x,y,z)=0$ (if these exist), find the values of $x,y,z, \text{ and } \lambda$ that simultaneously satisfy the equations $$\nabla f=\lambda\nabla g \text{ and } g(x,y,z)=0.$$If they exist, absolute extrema can be found by comparing these values of $f$ at each critical point satisfying the aforementioned two equations. For functions of two independent variables, the condition is similar, but without the variable $z$. 
- critical point/critical value (specifically for optimization with a constraint) 
	- TK
- Lagrange multipliers with two constraints 
	- Many problems require us to find the extreme values of a differentiable function $f(x,y,z)$ whose variables are subject to two constraints. If the constraints are $$g_1(x,y,z)=0 \text{ and } g_2(x,y,z)=0$$ and $g_1$ and $g_2$ are differentiable, with $\nabla g_{1}$ not parallel to $\nabla g_{2}$, we find the constrained local maxima and minima of $f$ by introducing two Lagrange multipliers $\lambda$ and $\mu$. That is, we locate the points $P(x,y,z)$ where $f$ takes on its constrained extreme values by finding the values of $x,y,z,\lambda, \text{ and } \mu$ that simultaneously satisfy the three equations $$\nabla f=\lambda\nabla g_{1}+\mu\nabla g_{2}, g_{1}(x,y,z)=0, g_{2}(x,y,z)=0$$

The first two examples are very long, because they are trying to solve a constrained optimization problem without using Lagrange multipliers. Try to follow along all the way through the examples, but understand that the main purpose of these examples is to motivate the technique about to be introduced. Lagrange multipliers take care of many of the considerations in these examples without having to think deeply into the geometry on every problem. The proof of the Orthogonal Gradient Theorem is just an application of the chain rule for paths. Examples 3 and 4 are both long, but they are about as simple as Lagrange Multiplier examples can be. The setup isn’t too bad in either example, and they perform the same steps in the same order. You should certainly try to work your way through them. 

### Reading Questions/Quizzes

1. In the problem of finding the point $p(x, y, z)$ on the plane $2x + y − z − 5 = 0$ that is closest to the origin, there are two functions: $f_1(x, y, z) = 2x + y − z − 5$ related to the plane and $f_2(x, y, z) = \sqrt{ x^2+y^2+z^2 }$ as the distance from $p(x, y, z)$ to the origin. Which is the function to be minimized and which gives the constraint?  
2. Use a software tool to plot the ellipse $\frac{x^2}{8}+\frac{y^2}{2}=1$ and a set of level curves of the function $f (x, y) = xy$. Adjust the choice of level curves to find those that are tangent to the ellipse. How do those tangent points relate to **Example 3**?  
3. In **Example 3**, write out the equations explicitly given by the method of Lagrange Multipliers. There should be three such equations. What are the unknowns to be solved?  
4. In **Example 3**, it is conceivable to solve for $y$ in terms of $x$ for every point $(x, y)$ on the ellipse $\frac{x^2}{8}+\frac{y^2}{2}=1$, e.g. $y=\sqrt{ 2-\frac{x^2}{4} }$, then treat $f(x,y)=\pm x\sqrt{ 2-\frac{x^2}{4} }$ as a function of $x$. What would be the domain of this pair of functions? What do you make of having to work with two functions? Can you use them to find an alternative solution to this problem? What would be the domain of this pair of functions? What do you make of having to work with two functions? Can you use them to find an alternative solution to this problem?  
5. Use the method of Lagrange multipliers to find 
	1. *Minimum on a hyperbola*: The minimum value of $x + y$, subject to the constraints $xy = 16, x > 0, y > 0$. 
	2. *Maximum on a line*: The maximum value of $xy$, subject to the constraint $x + y = 8$. Comment on the geometry of each solution.