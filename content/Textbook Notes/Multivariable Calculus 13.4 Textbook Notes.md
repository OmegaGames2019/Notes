
Status: Baby

![[13.4.pdf]]


## 13.4 Curvature and Normal Vectors of a Curve 

This section is omitted in the department syllabus, but it’s worthwhile for our honors sections to do a brief discussion of at least part of this section. Then central concept here is the curvature of a curve and the principal normal vector of a curve (under some condition). Intuitively, the curvature of a curve at a point measures how fast its “direction angle” is turning per unit length of movement along the curve. Technically, if $T(t)$ is the unit tangent vector of the curve $r(t)$ (defined when $r′(t)\neq 0$, namely, for a smooth curve): $\displaystyle T(t)=\frac{r'(t)}{||r'(t)||}$, then the curvature should be $|| \frac{dT}{ds}||=||v(t)^{-1} \frac{dT}{dt}||=v(t)^{-1}|| \frac{d}{dt}\left( \frac{r'(t)}{||r'(t)||} \right)||$. 

What remains is to develop an effective way of computing this quantity. **Example 2** demonstrates how to do this kind of computation for a circle of radius $a$. It’s instructive to compute the curvature of the helix curve (see **Example 5**). **Exercises 5, 6** gives formulae for computing the curvature of a plane curve given as a graph or in parametric form. 

### Reading Questions/Quizzes 

1. Compute the curvature of the curve given by $r(t) = 〈1−t^2, 3+3t^2, t^2〉$ wherever it is defined. Another observation about $T$ is that $T · T = 1$ for all $t$ (and $s$), so we get $0=\frac{d}{ds}(T\cdot T)=2 \frac{dT}{ds}\cdot T$, which means that the vector $\frac{dT}{ds}$ is always orthogonal to the tangent vector $T$, therefore is a vector normal to the curve. If this vector $\frac{dT}{ds}$ is not zero, then it has a unit vector pointing in its direction: $|| \frac{dT}{ds}||^{-1} \frac{dT}{ds}$, which is called the principal normal vector to $r(t)$ at this point. Denote it by $N$, then we have $N=|| \frac{dT}{ds}||^{-1} \frac{dT}{ds}$ , from which we deduce $\frac{dT}{ds}=|| \frac{dT}{ds}||N=\kappa N$, where $κ = ‖ \frac{dT}{ds} ‖$ is the curvature. 
	1. From my 13.3 textbook notes, $T(t)= \frac{<-1,3,1>}{\sqrt{ 11 }}$ when $t>0$ and $T(t)= \frac{<1,-3,-1>}{\sqrt{ 11 }}$ when $t<0$. Since $\frac{dT}{ds}$ can be represented as $\frac{dT}{dt}\cdot \frac{dt}{ds}$ and $\frac{dT}{dt}=0$, the curvature $\kappa$ is 0. 