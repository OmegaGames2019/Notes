
Status: 

![[15.1.pdf]]

## 15.1 Double and Iterated Integrals over Rectangles

In chapter 15, we will be studying multiple integration. The first step in that process is to understand the double integral. In single-variable calculus, you learned that the integral of $y = f (x)$ represents the area between the graph of the function and the x-axis. If the area was above the axis, we counted it as positive area. If the area was below the axis, we b counted it as negative. Our definite integrals were written as a $\int_{a}^b f(x)dx$, a notation that meant that we were integrating the function with respect to x on the interval $[a, b]$. Really this came down to the area bounded by the lines $x = a, x = b, \text{ and } y = 0$ and the curve $y = f (x)$ with positive/negative considerations discussed above. Now, our functions are of the form $z = f (x, y)$ and their graphs live in $\mathbb{R}^3$. When we integrate a function, we will need to look at a domain which is a subset of $\mathbb{R}^2$, which we understand to be the $xy$-coordinate plane.

The definition is done in a similar way as in the one-variable case: partition the region $\mathcal{R}$ into the non-overlapping union of small rectangles, form the Riemann sum of the integrand $f (x, y)$, and take the limit when the partition size goes to $0$. If the Riemann sum has a limit, that limit is called the integral of $f$ over the region $\mathcal{R}$, and is denoted as $\iint_{\mathcal{R}}f(x,y)dA$ or $\iint_{\mathcal{R}}f(x,y)dxdy$. 

Also as in one-variable calculus, one uses the definition to relate the integral to the volume under the graph of $f$ over $\mathcal{R}$ and establishes integrability criteria and properties of the integral, but rarely evaluates an integral through this process. Instead, one develops a method of evaluating iterated single variable integrals in the form of $\int_{a}^b\int_{c}^df(x,y)dydx \text{ if }\mathcal{R}=[a,b]\times[c,d]$ to evaluate $\iint_{\mathcal{R}}f(x,y)dA$. This is called Fubini's Theorem. Here, in $\int_{c}^df(x,y)dy$, we hold $x$ fixed and integrate out $f (x, y)$ as a function of $y$, then treat the outcome as a function of x and integrate it over x. 

Find the following definitions/concepts/formulas/theorems:  

- partition (you should have seen this when you defined the integral in Calculus I  
- Riemann sum (same general idea as single-variable, but our little intervals are now little rectangles)  
- limit of Riemann sums  
- norm (of a partition)  
- integrable (essentially the same as single-variable)  
- double integral  
- area element (dA)  
- Continuous functions are integrable  
- iterated integral  
- Theorem: Fubini’s Theorem  
- Double integral over a rectangle 

The first few pages are all about how we extend our understanding of integration and Riemann sums to functions of two variables. There is a lot of notation, but it is really close enough to the single-variable case that it should be readable. The two examples are very basic, and you should not have any trouble working through them. Notice that integration of a multivariable expression with respect to one of its variables treats the other one as a constant. This is for all of the same reasons as why we take partial derivatives the way that we do, and it should not come as a great shock to you. 


### Reading Questions/Quizzes

1. Evaluate $\int_{0}^1x^2ydy$ and then $\int_{0}^2\int_{0}^1x^2ydydx$ as well as $\int_{0}^1\int_{0}^2x^2ydxdy$. 
2. Evaluate $\int_{0}^1\int_{0}^\pi x\sin(xy)dydx$ and then $\int_{0}^\pi\int_{0}^1 x\sin(xy)dxdy$ 
3. Evaluate $\int_{0}^1\int_{0}^1 \frac{y}{1+xy}dydx$ and then $\int_{0}^1\int_{0}^1 \frac{y}{1+xy}dxdy$