
Status: 

![[14.3.pdf]]


## 14.3 Partial Derivatives

In this section, we are going to see how the concept of the derivative extends to functions of more than one variable. When we looked at the graphs of functions of two variables in section 14.1, we saw that at a particular point of the domain we may have different rates of change depending on the direction we travel from the point. It therefore does not make sense to talk about “the derivative” of a multivariable function at a point. What does make sense is talking about the derivative of a function at a point in a specific direction; the partial derivative of a function at a point with respect to a particular variable is the derivative of the function at that  
point in the specific direction parallel to the axis of that particular variable.  

If you have a function $f (x, y)$, the partial derivative with respect to $x$ at the point $(a,b)$ in the domain of the function is the rate of change of $f$ at that point along the line $r(t) = (a + t, b)$. That is what happens when we hold $y$ to be the constant $b$ and only let $x$ vary. Note that there are multiple notations that get used. You may see any of $$f_{x}=\frac{\partial f}{\partial x}=\frac{\partial}{\partial x}(f)=\frac{\partial}{\partial x}(f(x,y))$$ all of which mean the same thing (at least if $f$ is a function of $x,y$ for the last one). Other notations that are the equivalent: $$\begin{matrix}f_{x}(a,b)=\frac{\partial f}{\partial x}\bigg|_{(a,b)}\text{  }f_{y}(a,b)=\frac{\partial f}{\partial y}\bigg|_{(a,b)} \\
f_{xx}=\frac{\partial}{\partial x}\left( \frac{\partial f}{\partial x} \right)=\frac{\partial^2}{\partial x^2}(f)=\frac{\partial^2f}{\partial x^2}\text{  }f_{xy}=\frac{\partial}{\partial y}\left( \frac{\partial f}{\partial x} \right)=\frac{\partial^2}{\partial y\partial x}(f)=\frac{\partial^2f}{\partial y\partial x} \text{  etc.}
\end{matrix}$$I will usually use the subscript notation (so $f_{x}, f_{x}(a, b), f_{xx}, f_{xy}$, etc.) because it is a lot less writing/typing. There will be times when the Leibniz notation (the one with the $∂$’s) makes it easier to see what is going on. You should become comfortable with both notations. The rules for computing the partial derivatives are straightforward, as each is simply treating the function as a function of one of its variables and holding the others constant. In particular, the product/quotient rule, the chain rule, and implicit differentiation are used in the same way as in one-variable calculus. For example, if $f (x, y) = xy$ for $x, y > 0$, then $$f_{x}=yx^{y-1},f_{y}=x^y\ln x,f_{x x}=y(y-1)x^{y-2},f_{xy}=x^{y-1}+yx^{y-1}\ln x,f_{yx}=yx^{y-1}\ln x+x^{y-1}$$
From section 14.2 we learned that even if a function of several variables is well behaved (continuous or having derivative as a function of one variable) along each straight line passing a point, the function may still not have a well defined limit at that point. However, it is still natural to study a function of several variables by studying its behavior along one-dimensional lines so that one can apply the tools of one-variable calculus. Thus we will study the partial derivatives of a function and it tuns out that under reasonable conditions (the existence and continuity of all the partial derivatives) we can adapt the tools of one-variable calculus to multi-variable  
calculus.

Find the following definitions/concepts/theorems:  
- partial derivative 
	- When we hold all but one of the independent variables of a function constant and differentiate with respect to that one variable, we get a “partial” derivative. 
- partial derivative of $f$ with respect to $x$ (or $y$)
	- The partial derivative of $f(x,y)$ with respect to $x$ at the point $(x_{0},y_{0})$ is $$\frac{\partial f}{\partial x}\bigg|_{(x_{0},y_{0})}=\lim_{ h \to 0 } \frac{f(x_{0}+h,y_{0})-f(x_{0},y_{0})}{h}, $$provided the limit exists 
- Numerical approximation of partial derivatives 
	- TK
- second-order (and higher) partial derivatives 
	- $\frac{\partial^2f}{\partial x^2}=f_{x x}=\frac{\partial}{\partial x}\left( \frac{\partial f}{\partial x} \right)$
	- $\frac{\partial^2f}{\partial y^2}=f_{yy}=\frac{\partial}{\partial y}\left( \frac{\partial f}{\partial y} \right)$
- mixed partials (a/k/a mixed derivatives) 
	- $\frac{\partial^2f}{\partial y\partial x}=f_{yx}=\frac{\partial}{\partial y}\left( \frac{\partial f}{\partial x} \right)$
	- $\frac{\partial^2f}{\partial x\partial y}=f_{xy}=\frac{\partial}{\partial x}\left( \frac{\partial f}{\partial y} \right)$
- Theorem: The Mixed Derivative Theorem a/k/a Clairault’s Theroem (note the conditions under which this is true!) 
	- If $f(x,y)$ and its partial derivatives $f_{x},f_{y},f_{xy},f_{yx}$ are defined throughout an open region containing a point $(a,b)$ and are all continuous at $(a,b)$, then $$f_{xy}(a,b)=f_{yx}(a,b).$$
- differentiability and tangent plane 
	- A function $z=f(x,y)$ is differentiable at $(x_0,y_0)$ if both $f_{x}(x_{0},y_{0})$ and $f_{y}(x_{0},y_{0})$ exist and if $\Delta z=f(x,y)-f(x_{0},y_{0})$ satisfies $$\Delta z=f_{x}(x_{0},y_{0})\Delta x+f_{y}(x_{0},y_{0})\Delta y+\epsilon_{1}\Delta x+\epsilon_{2}\Delta y.$$ where $\Delta x=x-x_{0},@\Delta y=y-y_{0}$, and both $\epsilon_{1}\to{0}$ and $\epsilon_{2}\to 0$ as $(x,y)\to(x_{0},y_{0})$. We call the function $f$ differentiable if it is differentiable at every point in its domain, and we then say that its graph is a smooth surface. 
	- The tangent plane to a function $z=f(x,y)$ at $(x_{0},y_{0})$ is defined as $$L(x,y)=f(x_{0},y_{0})+f_{x}(x_{0},y_{0})(x-x_{0})+f_{y}(x_{0},y_{0})(y-y_{0}).$$ The fact that $f(x_{0},y_{0})=f(x_{0},y_{0})$ shows that the the function and the tangent plane both coincide at the point $(x_{0},y_{0})$
- smooth surface 
	- A surface is said to be smooth if it does not have singular points, in other words, if it has a (unique) tangent plane at every point 
- Differentiability implies continuity (Theorem 4) 
	- If a function $f(x,y)$ is differentiable at $(x_{0},y_{0})$, then $f$ is continuous at $(x_{0},y_{0})$
- Continuity of partials in a neighborhood implies differentiability (Theorem 3) 
	- If the partial derivatives $f_{x}$ and $f_{y}$ of a function $f(x,y)$ are continuous throughout an open region $R$, then $f$ is differentiable at every point of $R$. 

The motivating examples above example 1 are intended to give you a feel for when you will need to use multivariable functions to model real-world phenomena. **Examples 1, 2, 5, and 7** are very basic examples of partial derivatives. **Example 3** requires the quotient rule, but is otherwise no more scary than the others. **Examples 4 and 6** require versions of the chain rule. Much more on this in section 14.4. The subsection on Partial Derivatives and Continuity and **example 8** are a cautionary tale.  

A more jarring example is the function $$
f(x,y) =
\left\{ 
    \begin{array}{l}
        \frac{2x^2y}{x^4+y^2}\text{ for } (x,y)\neq(0,0) &\\
        0 \text{ for } (x,y)=(0,0)&\\
    \end{array} 
\right.
$$studied in Example 6 of Section 14.2. Note that $f (x, 0) = 0$ and $f (0, y) = 0$ so $f_{x}(x, 0)= 0$ and $f_{y} (0, y) = 0$. At any $(x, y)\neq (0, 0)$, the partials of this $f (x, y)$ can be computed using the quotient rule. So this function has partial derivatives at every point. Furthermore, if we study its behavior along any straight line passing through $(0, 0)$ by picking any $(a, b) \neq (0, 0)$ and setting $F (t) = f (ta, tb) = \frac{2a^2bt}{a^4t^2+b^2}$, it is a differentiable function of $t$ for any such $(a, b)$. Yet, this function does not have a well-defined limit as $(x, y) → (0, 0)$. 

A function can have partial derivatives at a point or even in a neighborhood of that point, but still not be a differentiable function at that point. A sufficient condition for a function to be differentiable at a point is that both (or all if there are more than two independent variables) partials exist in some open region around the point and be continuous at that point (**Theorem 3**). 

Most of the functions we deal with in this course will be differentiable everywhere (or almost everywhere), namely, they satisfy the conditions of **Theorem 3** at most places and the kind of behavior as exhibited in **Example 6** of Section 14.2 happens only at isolated points. You will certainly need to think about this if and when you take a real analysis class.  

**Examples 9 and 10** involve second-order partials. Neither one is terribly complicated, and you should make sure you understand them. In particular, notice that applying **Theorem 2** makes **example 10** much easier. If you intend to be a math major, take a look at the proof of **Theorem 2** in Appendix 9 in the back of the book. You should give the section on Differentiability a quick read, but don’t get hung up on it. The only big takeaway is that if a function is well-enough behaved to be differentiable a point (so its partials exist in some open region around the point), then it must be continuous there. 


### Reading questions/quizzes

1. Compute $f_{x}(x, y), f_{y} (x, y)$ of the function $f (x, y)$ above. Are $f_{x}(x, y), f_{y} (x, y)$ continuous at any $(x, y) \neq (0, 0)$? Are they continuous at $(x, y) = (0, 0)$? Is this $f (x, y)$ differentiable at any $(x, y) \neq (0, 0)$? Is it differentiable at $(x, y) = (0, 0)$? (Is it continuous at $(0, 0)$?) 
	1. $f_{x}=\frac{4xy(x^4+y^2)-8x^5y}{(x^4+y^2)^2}$
	2. $f_{y}=\frac{2x^2(x^4+y^2)-4x^2y^2}{(x^4+y^2)^2}$
	3. Since $f(x,y)$ is a rational function, it must be continuous at every point such that $x^4+y^2\neq{0}$. This means that the function is continuous at every point except for $(0,0$). 
	4. To see if these functions are continuous at $(x,y)=(0,0)$, we must examine the limits of $f_{x}\text{ and }f_{y}$ as $(x,y)\to(0,0)$. Since in both cases, neither of these limits approach a finite value, the functions are not continuous at $(0,0)$. 
	5. When $(x,y)\neq(0,0)$, the function is continuous and thus it must be differentiable (Differentiability implies continuity, but is the reverse true?) 
	6. When $(x,y)=(0,0)$, since the partial derivatives do not exist, it is not continuous at $(0,0)$. 
2. Define $\displaystyle g(x,y) =\left\{     \begin{array}{l}\frac{2x^3y}{x^4+y^2}\text{ for }(x,y)\neq(0,0) &\\    0 \text{ for } (x,y)=(0,0)&\\\end{array} \right.$ and answer the same questions about $g(x,y)$. 
	1.  $f_{x}=\frac{6x^2y(x^4+y^2)-8x^6y}{(x^4+y^2)^2}$
	2. $f_{y}=\frac{2x^3(x^4+y^2)-4x^3y^2}{(x^4+y^2)^2}$
	3. Since $f(x,y)$ is a rational function, it must be continuous at every point such that $x^4+y^2\neq{0}$. This means that the function is continuous at every point except for $(0,0$). 
	4. To see if these functions are continuous at $(x,y)=(0,0)$, we must examine the limits of $f_{x}\text{ and }f_{y}$ as $(x,y)\to(0,0)$. Since in both cases, neither of these limits approach a finite value, the functions are not continuous at $(0,0)$. 
	5. When $(x,y)\neq(0,0)$, the function is continuous and thus it must be differentiable (Differentiability implies continuity, but is the reverse true?) 
	6. When $(x,y)=(0,0)$, since the partial derivatives do not exist, it is not continuous at $(0,0)$. 
3. Compute $f_{x},f_{y},f_{x x},f_{xy},f_{yx},f_{yy}$ for $f(x,y)=xy\sin^2(x^2y)$
	1. $f_{x}=y\sin^2(x^2y)+2x^2y\sin(2x^2y)$
	2. $f_{y}=x\sin^2(x^2y)+xy\sin(2x^2y)$
	3. $f_{xx}=6xy\sin(2x^2y)+8x^3y\cos(2x^2y)$
	4. $f_{yy}=2x\sin(2x^2y)+2xy\cos(2x^2y)$
	5. $f_{xy}=f_{yx}=2x\sin(2x^2y)+4xy\sin(2x^2y)+8x^3y\cos(2x^2y)$
4. Define $\displaystyle h(x,y) =\left\{     \begin{array}{l}xy\frac{x^2-y^2}{x^2+y^2}\text{ for }(x,y)\neq(0,0) &\\    0 \text{ for } (x,y)=(0,0)&\\\end{array} \right.$
	1. Verify that $h_{x}(0,y)=-y$ and $h_{x}(x,0)=x$
		1. $h_{x}=y \frac{x^2-y^2}{x^2+y^2}+x\frac{2x(x^2+y^2)-2x(x^2-y^2)}{(x^2+y^2)^2}=y \frac{x^2-y^2}{x^2+y^2}+\frac{4x^2y^2}{(x^2+y^2)^2}$
			1. $h_{x}(0,y)=-y$
			2. $h_{x}(x,0)=0$ (how?) 
	2. Use the definition of partial derivatives to evaluate $h_{xy}(0,0)$ and $h_{yx}(0,0)$ and verify that they are not equal 
		1. Help