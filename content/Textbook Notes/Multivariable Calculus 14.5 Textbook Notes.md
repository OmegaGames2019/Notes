
Status: 

![[14.5.pdf]]


## 14.5 Directional Derivatives and Gradient Vectors 

In considering the rate of increase/decrease of a function of several variables at a point, the direction plays a role. In section 14.3, we focused on the special directions along each of the coordinate axes, which introduced the partial derivatives; but we need to compute the rate along any direction. For a function of two variables $(x, y)$ defined near $(x_{0}, y_{0})$, take any direction $〈a, b〉$, the rate of change of $f$ at $(x_{0}, y_{0})$ in the direction of $〈a, b〉$ is $$\frac{d}{dt}\bigg|_{t=0}f(x_{0}+at,y_{0}+bt)$$ if it exists, and will be denoted as $D_{(a,b)}f(x_{0},y_{0})$. Once $<a,b>$ is given, this becomes a one-variable calculus problem. Since there exists infinitely many directions, do we need to do this computation for every $<a,b>$? Some of the questions that we need to address include: 
- Is there a simple dependency of $D_{(a,b)}f(x_{0},y_{0}) \text{ on }<a,b>$? 
- What's the meaning of direction of steepest ascent/descent? What about directions $<a,b>$ such that $D_{(a,b)}f(x_{0},y_{0})=0$? 

The motivation for directional derivatives (all of the stuff above the definition) is useful for visualizing what’s going on. Please read it. 

It turns out the notion of the gradient plays a crucial role in answering the above questions. By definition, it looks like we are just giving a name to the vector whose components are the partial derivatives of a function. But this vector has some amazing properties which will allow use to find directional derivatives, paths of steepest ascent, and normal vectors to level curves and surfaces. The gradient will also be a critical tool that we use to analyze vector fields in chapter 16.  

Find the following definitions/concepts/formulas/theorems: 

- directional derivative (definition and formula (3) or (4) for finding it using the dot product — but this needs the differentiability of $f$ at the point)  
	- The derivative of $f$ at $P_{0}(x_{0},y_{0})$ in the direction of the unit vector $u=u_{1}i+u_{2}j$ is the number $$\left( \frac{df}{ds} \right)_{u,P_{0}}=\lim_{ s \to 0 } \frac{f(x_{0}+su_{1},y_{0}+su_{2})-f(x_{0},y_{0})}{s}, $$ provided the limit exists. It is also denoted as $D_{u}f(P_{0}) \text{ or }D_{u}f|_{P_{0}}$ (read as "The derivative of $f$ in the direction of $u$, evaluated at $P_{0}$) 
- properties of the directional derivative 
	- The equation $z=f(x,y)$ represents a surface $S$ in space. If $z_{0}=f(x_{0},y_{0})$, then the point $P(x_{0},y_{0},z_{0})$ lies on $S$. The vertical plane that passes through $P$ and $P_{0}(x_{0},y_{0})$ parallel to $u$ intersects $S$ in a curve $C$ (Figure 14.28). The rate of change of $f$ in the direction of $u$ is the slope of the tangent to $C$ at $P$ in the right-handed system formed by the vectors $u$ and $k$. 
	- ![[Interpretation of Directional Derivative.png]]
	- The function $f$ increases most rapidly when $\cos \theta=1$, which means that $\theta=0$ and $u$ is the direction of $\nabla f$. That is, at each point $P$ in its domain, $f$ increases most rapidly in the direction of the gradient vector $\nabla f$ at $P$. The derivative in this direction is $$D_{u}f=|\nabla f|\cos(0)=|\nabla f|$$
	- Similarly, $f$ decreases most rapidly in the direction of $-\nabla f$. The derivative in this direction is $D_{u}f=|\nabla f||\cos \pi=-|\nabla f|$
	- Any direction $u$ orthogonal to a gradient $\nabla f\neq{0}$ is a direction of zero change in $f$ because $\theta$ then equals $\frac{\pi}{2}$ and $$D_{u}f=|\nabla f|\cos \frac{\pi}{2}=|\nabla f|\cdot{0}=0$$
- tangent line to a level curve- Big question: what would you get if you extended this formula into $\mathbb{R}^3$? What would the formula be, and what would it represent? Could you keep going into higher dimensions?  
	- If you extend this formula into $\mathbb{R}^3$, it would not be the equation for a line; it would be the equation for a plane: $$f_{x}(x_{0},y_{0})(x-x_{0})+f_{y}(x_{0},y_{0})(y-y_{0})+f_{z}(x_{0},y_{0})(z-z_{0})=0$$
- Algebra rules for gradients 
	- Sum rule: $\nabla (f+g)=\nabla f+\nabla g$
	- Difference rule: $\nabla (f-g)=\nabla f-\nabla g$
	- Constant multiple rule: $\nabla(kf)=k\nabla f$ (any number $k$)
	- Product rule: $\nabla(fg)=f\nabla g+g\nabla f$
		- Scalar multipliers on left of gradients
	- Quotient rule: $\nabla\left( \frac{f}{g} \right)=\frac{g\nabla f-f\nabla g}{g^2}$ 
		- Scalar multipliers on left of gradients 
- extension of gradient into three dimensions 
	- $\nabla f=\frac{\partial f}{\partial x}i+\frac{\partial f}{\partial y}j+\frac{\partial f}{\partial z}k$
- Chain Rule for Paths 
	- If $r(t)=x(t)i+y(t)j+z(t)k$ is a smooth path $C$, and $w=f(r(t))$ is a scalar function evaluated along $C$, then according to the Chain Rule, Theorem 6 in Section 14.4, $$\frac{dw}{dt}=\frac{\partial w}{\partial x} \frac{dx}{dt}+\frac{\partial w}{\partial y} \frac{dy}{dt}+\frac{\partial w}{\partial z} \frac{dz}{dt}$$

**Example 1** is a direct calculation using the limit definition of the directional derivative. Please don’t ever calculate a directional derivative this way if you can avoid it. **Example 2** is how you should be calculating directional derivatives.  

**Example 3** illustrates how the gradient relates to the direction of greatest increase/decrease and the directions of zero change (which are tangent to the level curve or surface as one would expect). 

**Example 4** shows how to use the gradient to find the tangent line to an implicitly defined curve in $\mathbb{R}^2$. What we are really doing in this example is “going up a dimension” to think about this 2D object as a level curve of some 3D object. We certainly could use calculus 1 implicit differentiation techniques to find this tangent line, but the calculations are much faster and cleaner this way.  

**Example 5** applies the algebra rules in a couple of typical ways. There should be no surprises here. **Example 6** is a straightforward application of the gradient for a function of three variables. Directly above **example 6**, there is a sentence that says, “In any direction orthogonal to $∇f$ , the derivative is zero.” How many such directions are there? If you put all of those directions together, what shape do you get? 


### Reading Questions/Quizzes

1. Let $f (x, y) = x^2y$.  
	1. Compute the directional derivative of $f$ at $(x, y)$ in the direction of $〈a, b〉$. 
		1. $D_{<a,b>}f(x,y)= <2xy,x^2>\cdot<a,b> =2axy+bx^2$
	2. Compute the gradient vector of $f$ at $(x, y)$. 
		1. $\nabla f(x,y)=2xyi+x^2j$
	3. Sketch the gradient of $f$ at $(−1, 2)$ together with the level curve that passes through this point.  
		1. TK
	4. Find an equation of the tangent line to the level curve of $f$ that passes through $(−1, 2)$. 
		1. $-4(x+1)+1(y-2)=0$
	5. Find the direction of steepest ascent of $f$ and direction of steepest descent at $(−1, 2)$. 
		1. $\nabla f(-1,2)= \langle-4,1\rangle$. The direction of steepest ascent is $y$ and the direction of steepest descent is $x$. 
	6. Find an equation of the tangent plane to the graph of $f (x, y)$ at $(−1, 2, 2)$. Identify its normal vector. 
		1. TK