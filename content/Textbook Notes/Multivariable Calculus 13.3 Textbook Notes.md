
Status: Baby

![[13.3.pdf]]

## 13.3 Arc Length in Space

This section is a generalization of something you saw in calculus 2 (or AP Calculus BC).  
When you considered the arc length of a parameterized curve in $\mathbb{R}^2$, you saw the formula $s=\int_{a}^b\sqrt{ \left( \frac{dx}{dt} \right)^2+\left( \frac{dy}{dt} \right)^2 }dt$. Much of the time, this formula produced an integrand which you did not have the techniques to integrate by hand, and that will be true here as well. The examples which you could integrate were usually specifically designed to have a “nice” integrand. As usual, this section will only discuss the situation in $\mathbb{R}^2$, but the techniques presented here generalize  
to dimensions beyond 3 as well. Find the following definitions/concepts/formulas/theorems:  

- Arc length in $\mathbb{R}^3$ (two different forms- one useful, one compact)  
	- $s=\int_{a}^{b}\sqrt{ \left( \frac{dx}{dt} \right)^2+\left( \frac{dy}{dt} \right)^2+\left( \frac{dz}{dt} \right)^2 }dt=\int_{a}^b||\vec{r}'(t)||dt$
- arc length parameter 
	- $s(t)=\int_{t_{0}}^t||r'(u)||du$ where $u$ is a dummy variable to avoid confusion with the upper bound of the limit 
- arc length parametrization 
	- $s(t)=\int_{t_{0}}^t||r'(u)||du$ is the arc length parameter. To parameterize this, $s(t)$ can be rewritten to express $t$ as a function of $s$: $t(s)$. Therefore, the curve $r(t)$ that parameterizes the arc length of $s(t)$ can be written as $r(s)=r(t(s))$
- speed (for a vector-valued function) 
	- Given a vector valued function $\vec{r}(t)$, its speed is represented by $|\vec{r}'(t)|=|v(t)|$
- unit tangent vector 
	- Given a vector valued function $\vec{r}(t)$, its unit tangent vector at point $t_{0}$ can be calculated by $\displaystyle\frac{\vec{r}'(t_{0})}{||\vec{r}'(t_{0})||}$

Note that in the definition for the length of a smooth curve $r(t) = x(t)i+y(t)i+z(t)k$, there is a condition that it is traced exactly once as t increases from $t = a$ to $t = b$. However, this condition is rarely checked in the examples, as it may not easy to check except in a situation such as when one of the coordinate function is a strictly increasing function of t as in the case of Example 1. Furthermore, if one interprets $v(t)=\sqrt{ \left( \frac{dx}{dt} \right)^2+\left( \frac{dy}{dt} \right)^2+\left( \frac{dz}{dt} \right)^2 }$ as the speed of a particle whose position at time $t$ is $r(t)$, then, even if this condition does not hold, one can interpret $\int _a^bv(t)dt$ as the distance traveled by the particle according to this function $r(t)$ from $t = a$ to $t = b$. 

Related to the above is the concept of reparameterization and invariance of arclength under reparameterization. The concept of reparameterization is not formally discussed in this chapter, but there is some informal discussion in Section 11.1.  

Here is a brief summary: suppose that $r(t)$, $t ∈ [a, b]$ is a vector-valued function and that $s = I(t)$ is a (strictly) monotone real-valued function defined on $[a, b]$ such that its values fill exactly $[c, d]$. This $I(t)$ then has a well-defined inverse function $t = I^{-1}(s)$ define on $[c, d]$. For convenience, we assume that $I(t)$ is monotone increasing, therefore, $c = I(a)$, $d = I(b)$. Then the vector-valued function $\tilde{r}(s) := r ◦ I^{-1}(s)$ defined on [c, d] is called a reparameterization of  
$r(t)$. Note that, in this new parametrization, its velocity vector is $\displaystyle\frac{d\tilde{r}(s)}{ds}=\frac{dr}{dt}|_{t=I^{-1}s} \frac{dI^{-1}(s)}{ds}=\frac{\frac{dr}{dt}}{\frac{dI}{dt}}|_{t=I^{-1}(s)}$ by the chain rule and differentiation of an inverse function. Therefore, its speed is $||\frac{d\tilde{r}(s)}{ds}||=\frac{||\frac{dr}{dt}||}{|\frac{dI}{dt}|}|_{t=I^{-1}(s)}$ and the arc length computed according to this new parametrization becomes $\displaystyle\int_{c}^d || \frac{d\tilde{r}(s)}{ds}||ds=\int _c^d \frac{||\frac{dr}{dt}||}{| \frac{dI}{dt}|}|_{t=I^{-1}(s)}ds=\int_{a}^{b}\frac{||\frac{dr(t)}{dt}||}{| \frac{dI}{dt}|| \frac{dI}{dt}|}dt=\int_{a}^b|| \frac{dr(t)}{dt}||dt$ by the change of variable formula for integrals. This result is the same as computed under the earlier parametrization, and show the *invariance of arc length under reparameterization*.  

Arclength parametrization is defined via the special parametrization $s = I(t) =\int_{a}^tv(τ )dτ$ . This function is strictly monotone increasing under the condition that $v(t) > 0$ for all $t$, which is how the smoothness of a curve enters into this discussion. Only in simple examples can this function be computed explicitly; however, one can make conceptual argument without having an explicit expression for $I(t)$. 

One can think of $r(t)$ as describing the position of a particle along a curve by its time t, and its arclength parametrization as describing the position of a particle along a curve by its distance from a reference point (e.g. the position along a highway by its mile marks).  

Since $\displaystyle\frac{d}{ds}=\frac{dt}{ds} \frac{d}{dt}=v(t)^{-1} \frac{d}{dt}$ here we treat both sides as operators so that they can be applied to any functions (either scalar-valued or vector-valued) of $t$ or $s$. In particular, if we reparametrize a given $r(t)$ by its arc length parameter $s: \tilde{r}(s) := r(I^{-1}(s))$,  
then $\frac{d\tilde{r}(s)}{ds}=v(t)^{-1} \frac{dr(t)}{dt}$, and $|| \frac{d\tilde{r}(s)}{ds}||=v(t)^{-1}|| \frac{dr(t)}{dt}||=1$, namely, the tangent vector $\frac{d\tilde{r}(s)}{ds}$ is a unit tangent vector for all s.  

### Reading Questions/Quizzes 

1. Given $r(t) = 〈1 − t^2, 3 + 3t^2, t^2〉$.  
	1. Does this function trace a curve exactly once from $t = −1$ to $t = 1$? Is it a smooth curve for $t$ in $[−1, 1]$? Can you recognize that its path lies on a portion of a straight line? 
		1. Note that the each parameter of the curve has a term $t^2$. This means that for some value of $x\epsilon[-1,1]$ such as $a$, $r(-a)=r(a)$. Therefore, this function traces a curve along the given interval twice.  
		2. The velocity vector is $v(t)= <-2t,6t,2t>$. However, this vector is $<0,0,0>$ at $t=0$, which implies that the graph stops at that point meaning it is not smooth. 
		3. To see if they are a portion of a straight line, we must show that the graph is linear in some way. We can do this by expressing two variables as a function of the other and checking to see if the degrees of the functions are all 1. Since the $z(t)$ is $t^2$, $x(t)=1-z,y(t)=3+3z$. Since these are linear, the path lies on a portion of a straight line. 
	2. Find its arc length parameter $s = ∫_{0}^t ‖r′(τ )‖ dτ$ and compute its length from $t = 0$ to $t = 1$.  
		1. $s=\int_{0}^t\sqrt{ (-2t)^2+(6t)^2+(2t)^2 }dt=\sqrt{ 44 }\int_{0}^ttdt=\frac{\sqrt{ 44 }t^2}{2}=\sqrt{ 11 }t^2$. 
		2. The length from $t=0$ to $t=1$ is $\sqrt{ 11 }$
	3. Find its arc length parametrization. 
		1. $s(t)=\sqrt{ 44 }\int_{t_{0}}^ttdt=\frac{\sqrt{ 44 }(t^2-t_{0}^2)}{2}=\sqrt{ 11 }(t^2-t_{0}^2)$
		2. $t(s)=\pm \sqrt{ \frac{s}{\sqrt{ 11 }} }$
		3. Substituting this back into $r(t)$, we get $r(s)= <1-\frac{s}{\sqrt{ 11 }},3+\frac{3s}{\sqrt{ 11 }}, \frac{s}{\sqrt{ 11 }}$
	4. Find the unit tangent vector of $r(t)$ at $r(t)$ whenever it is defined. Can it be extended as a continuous function of $t$ on $[−1, 1]$? 
		1. $T(t)= \frac{<-2t,6t,2t>}{2\sqrt{ 11 }|t|}$ where $t\neq 0$. Since the proportion of the numerator to the denominator is a constant as $t$ changes, the unit tangent vector is $T(t)= \frac{<-1,3,1>}{\sqrt{ 11 }}$ when $t>0$ and $T(t)= \frac{<1,-3,-1>}{\sqrt{ 11 }}$ when $t<0$ 