
Status: 

![[15.3.pdf]]


## 15.3 Area by Double Integration

If $\mathcal{R}$ is a two-dimensional region, if we take the integrand $f$ to be $1$, then $\iint_{\mathcal{R}}1dA$ gives the area of the region $R$. The main remaining task is to evaluate this integral by appropriate iterated integral, as done in the previous section. 

The region $\mathcal{R}$ is typically bounded by two or more curves. To do integral over $\mathcal{R}$, one needs to decide whether to "slice" it into vertical slices or horizontal ones, and in the former case, finds out the leftmost vertical slice and the rightmost vertical slice, while in the latter case, the lowest slice and the highest slice. These are typically found by finding the intersection points of the region. 

**Example 2** is a simple illustration of this. The region is bounded by $y=x^2$ and $y=x+2$. The intersection points of the two curves are given by solving these two equations jointly, which gives $x^2=x+2$, from which one gets $x=-1$ and $x=1$. One finds that $(-1,1)$ is the leftmost point and $(1,2$) is the rightmost point. $(1,2)$ is also the highest point. However, the lowest point is given by the minimum of $y=x^2$ over the interval $[-1,1]$, which is at $(0,0)$. 

If we slice this region by vertical slices, then $x$ runs from $-1$ to $1$ and for each such $x$, $y$ runs from the lowest point of that slice with value $x^2$ to the highest point of that slice with value $x+2$. Thus, $$\iint_{\mathcal{R}}dA=\int_{-1}^1\int_{x^2}^{x+2}dydx.$$ 
One can try to slice this region by horizontal slices, but the leftmost boundary of each horizontal slice depends on the level of $y:$ for $0\leq y\leq 1$, $x$ runs from $-\sqrt{ y }\text{ to }\sqrt{ y }$, while for $1\leq y\leq 2$, $x$ runs from $y-2$ to $\sqrt{ y }$. 

Thus, $$\iint _{\mathcal{R}}dA=\int_{0}^1\int_{-\sqrt{ y }}^\sqrt{ y }dxdy.$$

In computing the average value of $f$ over $\mathcal{R}$, one needs to compute the area of $\mathcal{R}$ and $\iint_{\mathcal{R}}f(x,y)dA$. For example, if one takes $f(x,y)=xy$ and $\mathcal{R}$ to be the quarter circle $x^2+y^2=1$ in the first quadrant, the area of $\mathcal{R}$ is $\frac{\pi}{4}$, and one needs to evaluate $\iint_{\mathcal{R}}xydA$. 


### Reading Questions/Quizzes 

1. Evaluate the above integral $\iint_{\mathcal{R}}xydA$ and find the average of $xy$ over this region. Then find the average of $xy$ over the square $0\leq x\leq_{1},0\leq y\leq 1$. Which of these two averages is bigger. Do you have an intuitive explanation? 