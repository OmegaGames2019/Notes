
Status: Child

![[15.4.pdf]]

## 15.2 Double Integrals in Polar Form

The basic idea in doing double integrals in polar form is to partition the region into the disjoint union of small "circular rectangles" with circular arc length $r\Delta\theta$ and thickness $\Delta r$. $r\Delta\theta\Delta r$ provides a good approximation for the area of such a "circular rectangles". This process corresponds to doing integration of $f(r\cos\theta,r\sin\theta)r$ over the $r$-$\theta$ variables: $$\iint_{\mathcal{R}}f(x,y)dA=\iint_{\tilde{\mathcal{R}}}f(r\cos\theta,r\sin\theta)r drd\theta ,$$ where $\tilde{\mathcal{R}}$ stands for the description of $\mathcal{R}$ in the $r$-$\theta$ variables. 

The simplest region in terms of the $r$-$\theta$ variables that takes the form of $r_{1}\leq r\leq r_{2}$ and $\theta_{1}\leq\theta\leq\theta_{2}$, which corresponds to the part of the disk within $x^2+y^2\leq r_{2}^2$ but outside of the disk $x^2+y^2\leq r_{1}^2$ and with the polar angle $\theta$ between $\theta_{1}$ and $\theta_{2}$. 

For a more general region $\mathcal{R}$, one needs to find out how to describe the boundary curves of $\mathcal{R}$ in terms of the $r$-$\theta$ variables. This entails writing the boundary curves in terms of polar coordinates and finding the intersection points of the boundary curves. 

In the case of **Example 3**, where the region $\mathcal{R}$ is the semicircular region bounded by the $x$-axis and the curve $y=\sqrt{ 1-x^2 }$, if one has not recognized the latter as part of the circle $x^2+y^2=1$, the substitution $r\sin\theta=\sqrt{ 1-r^2\cos^2\theta }$ and simplification still leads to $r=1$. The bounds $r=0$ and $0\leq\theta\leq \pi$ does not seem to follow algebraically directly from $y=\sqrt{ 1-x^2 }$; this comes from inspecting the enclosed region in a more geometric fashion. 

In the case of **Examples 1 and 2**, the boundary curves are given directly in terms of the polar coordinates $r=1$ and $r=1+\cos\theta$ in **Example 1** and $r^2=4\cos 2\theta$ in **Example 2**. But the bounds for $\theta$ are not given explicitly and have to be worked out. In the case of **Example 1**, the intersection of the two curves and the requirement that the region is inside $r=1+\cos\theta$ but outside of $r=1$, gives the bound of $-\frac{\pi}{2}\leq\theta\leq \frac{\pi}{2}$, and for each such $\theta$, $1\leq r\leq{1}+\cos\theta$. In the case of **Example 2**, one has to figure out that the angle $\theta$ needs to satisfy either $-\frac{\pi}{4}\leq\theta\leq \frac{\pi}{4}$ or $\frac{3\pi}{4}\leq\theta\leq \frac{5\pi}{4}$ (coming from $\cos{2}\theta\geq{0}$). But symmetry consideration reduces the integral into one-quarter of the region. 


### Reading Questions/Quizzes

1. Describe the region enclosed by $r=1$ and $r=1+\cos\theta$, namely, the intersection of the regions $r\leq 1$ and $r\leq 1+\cos\theta$, and find its area. More specifically, sketch the region in the $r$-$\theta$ coordinates. Write out the limits of the iterated integrals of the integral over this region. 
2. Sketch in the $r$-$\theta$ coordinates the region enclosed by $x^2+y^2\leq{1}$ and $(x-1)^2+y^2\leq 1$ and write out the limits of the iterated integral over this region. 
3. Study **Example 6** and rewrite the area integral in polar coordinates but reverse the order of integration by doing the $\theta$-integral first. 