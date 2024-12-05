
Status: 

![[14.6.pdf]]


## 14.6 Tangent Planes and Differentials 

Just as the existence of the tangent line of the graph of a function $y = f (x)$ of a single variable at $(x_{0}, y_{0})$ is equivalent to the differentiability of $f$ at $x_{0}$, the existence of the tangent plane of the graph of a function $y = f (x, y)$ of two variables at $(x_{0}, y_{0}, f (x_{0}, y_{0}))$ is equivalent to the differentiability of $f$ at $(x_{0}, y_{0})$. Recall that $f (x, y)$ is differentiable at $(x_{0}, y_{0})$ if both $f_{x}(x_{0}, y_{0})$ and $f_{y} (x_{0}, y_{0})$ exist and the function $$L(x,y):=f(x_{0},y_{0}))+f_{x}(x_{0},y_{0})(x-x_{0})+f_{y}(x_{0},y_{0})(y-y_{0})$$ has the following approximation property fo $f(x,y)$ near $(x_{0},y_{0})$: $$f(x,y)-L(x,y))=\epsilon_{1}(x-x_{0})+\epsilon_{2}(y-y_{0})$$ where $\epsilon_{1},\epsilon_{2}\to(x_{0},y_{0})$. 

The graph of $L(x,y)$ is a plane sharing $(x_{0},y_{0},f(x_{0},y_{0}))$ with the graph of $f(x,y)$. This plane is tangent to the graph of $f(x,y)$ at $(x_{0},y_{0},f(x_{0},y_{0}))$ because their vertical difference, $f(x,y)-L(x,y)$, goes to $0$ at a faster rate than $||(x-x_{0},y-y_{0})||=\sqrt{ (x-x_{0})^2+(y-y_{0})^2 }$. 

The textbook takes a peculiar approach by first discussing the tangent plane of the level surface of a function of three variables $w=f(x,y,z)$ at a point and treating the tangent plane of the graph of $z=f(x,y)$ as that of the 0-level surface of the function $f(x,y)-z$ (as in formula (3)). The level surface of a function of three variables is in general more difficult to visualize than the graph of a function of two variables. 

Find the following definitions/concepts/formulas/theorems: 

- tangent plane to a level surface (definition and formula) 
	- The tangent plane to the level surface $f(x,y,z)=c$ of a differentiable function $f$ at a point $P_{0}$ where the gradient is not zero is the plane through $P_{0}$ where the gradient is not zero is the plane through $P_{0}$ normal to $\nabla f|_{P_{0}}.$ 
- normal line of a surface at a point (definition and formula) 
	- The normal line of the surface of $P_{0}$ is the line through $P_{0}$ parallel to $\nabla f|_{P_{0}}$
- tangent plane to a graph surface 
	- The plane tangent to the graph surface $z=f(x,y)$ of a differentiable function $f$ at the point $P_{0}(x_{0},y_{0},z_{0})=(x_{0},y_{0},f(x_{0},y_{0}))$ is $$f_{x}(x_{0},y_{0})(x-x_{0})+f_{y}(x_{0},y_{0})(y-y_{0})-(z-z_{0})=0$$
- formula for estimating change in value of differentiable multivariable function 
	- To estimate the change in the value of a differentiable function when we move a small distance $ds$ from a point $P_{0}$ in a particular direction $u$, use this formula: $$df=(\nabla f|_{P_{0}}\cdot u)ds$$ where $\nabla f|_{P_{0}}\cdot u$ is the directional derivative and $ds$ is the distance increment 
- linearization of $f (x, y)$ centered at $(x_{0}, y_{0})$ 
	- The linearization of a function $f(x,y)$ at a point $(x_0,y_0)$ where $f$ is differentiable is the function $$L(x,y)=f(x_{0},y_{0})+f_{x}(x_{0},y_{0})(x-x_{0})+f_{y}(x_{0},y_{0})(y-y_{0}).$$ The approximation $$f(x,y)\approx L(x,y)$$ is the standard linear approximation of $f$ at $(x_{0},y_{0}).$ 
- Error in the standard linear approximation 
	- If $f$ has continuous first and second partial derivatives throughout an open set containing a rectangle $R$, then the error $E(x,y)$ incurred in replacing $f(x,y)$ on $R$ by its linearization $$L(x,y)=f(x_{0},y_{0})+f_{x}(x_{0},y_{0})(x-x_{0})+f_{y}(x_{0},y_{0})(y-y_{0}).$$ satisfies the inequality $$|E(x,y)|\leq \frac{1}{2}M(|x-x_{0}|+|y-y_{0}|)^2$$
- total differential (this should be familiar from calc 1, and is really just a sometimes convenient alternate notation) 
	- If we move from $(x_0,y_0)$ to a point $(x_{0}+dx,y_{0}+dy)$ nearby, the resulting change $$df=f_{x}(x_{0},y_{0})dx+f_{y}(x_{0},y_{0})dy$$ is the linearization of $f$ called the total differential of $f$. 
- Extensions of the above concepts to functions of three variables 
	- TK

**Examples 1-3** are all straightforward, and you will hopefully not have trouble working through them. Finding tangent planes uses techniques that we developed in **chapter 12**. **Examples 4-7** all involve using partial derivatives to produce linearization, and then use the linearization to estimate the function somewhere near the point at which the linearization is centered. **Example 4** doesn’t produce an equation for the linearization, using the directional derivative to accomplish the same purpose. This works because we knew the direction of the motion in the domain whose effect we were going to be estimating. The other examples are more typical, where you find the linearization (possibly in differential form) and then use it to estimate function value changes.  

**Example 8** is a linearization of a three variable function. Is the linearization still a plane, or is it something else? If you graph $w = f (x, y, z)$, how many dimensions does the graph have? 


### Reading Questions/Quizzes 

1. Let $f (x, y, z) = x^2y + x sin z$.  
	1. Compute the directional derivative of $f$ at $(x, y, z)$ in the direction of $〈a, b, c〉$
		1. $D_{\langle a,b,c\rangle}f(x,y,z)=\langle 2xy+\sin z,x^2,x\cos z\rangle\cdot\langle a,b,c\rangle=(2xy+\sin z)a+bx^2+cx\cos z$
	2. Compute the gradient vector of $f$ at $(x, y, z)$. 
		1. $\nabla f(x,y,z)=\langle 2xy+\sin z,x^2,x\cos z\rangle$ 
	3. Sketch the gradient of $f$ at $(−1, 2, 0)$ together with the level surface that passes through this point. 
		1. TK
	4. Find an equation of the tangent plane to the level surface of $f$ that passes through $(−1, 2, 0)$. 
		1. $-4(x+1)+1(y-2)+0(z-0)=0$ 
	5. Find a direction normal to the level surface of $f$ that passes through $(−1, 2, 0)$ and write down equations for the normal line to the level surface of f through that point. 
		1. $n(t)=-4(t+1)i+(y-2)j$
	6. Find all directions $u$ such that $D_{u}f (−1, 2, 0) = 0$. 
		1. $D_{\langle a,b,c\rangle}f(x,y,z)=\langle 2xy+\sin z,x^2,x\cos z\rangle\cdot\langle a,b,c\rangle=(2xy+\sin z)a+bx^2+cx\cos z$
		2. $D_{\langle a,b,c\rangle}f(-1,2,0)=-4a+b=0$
		3. Answer: Any direction that satisfies $b=4a$ where $\langle a,b,c\rangle$ is the direction 
	7. Find the direction of steepest ascent of $f$ and direction of steepest descent at $(−1, 2, 0)$. 
		1. Steepest ascent: $y$
		2. Steepest descent: $x$ 
	8. Compute the linearization of $f$ at $(−1, 2, 0)$. 
		1. $L(x,y,z)=2-4(x+1)+1(y-2)+1(z+0)$
2. Define $f (x, y, z) = (1 + \sin(x + y) + z)^{-1/2}$. Compute its total differential at $(0, 0, 0)$ and use the total differential to estimate $f (0.1, 0.1, −0.1)$ 
	1. $df=-\frac{1}{2}dx-\frac{1}{2}dy-\frac{1}{2}dz$
	2. $f(0.1,0.1,-0.1)\approx-4\cdot{0}.1+1\cdot 0.1=-0.3$ 