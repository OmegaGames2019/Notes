Status: Adult 

![[13.1.pdf]]

### 13.1 Curves in Space and their Tangents 

A curve in space is given by a vector-valued function $r(t) = 〈f (t), g(t), h(t)〉$of a parameter $t$
defined on some interval $(a, b)$ or $[a, b]$ of $\mathbb{R}$.  When one plots the graph of a function $y = g(t)$ of one variable $t$, one plots both the $t$ and the $y$-axis. When one plots the “graph" of a vector-valued function $r(t) = 〈f (t), g(t), h(t)〉$, however, one often omits the $t$-axis, and only plots the collection of points $(f (t), g(t), h(t))$ for $t ∈ (a, b)$. What one sees is a curve, but for a specific point on this curve, the value $t$ that gives rise to this point is not plotted (it is possible that more than one values of $t$ may give rise to the same point). 

If one treats a parametric curve $r(t) = 〈f (t), g(t)〉$ as an $\mathbb{R}^2$-valued function, it is possible  
to plot the “graph" of this function including the $t$-axis. This GeoGebra/3d plot plots the $\mathbb{R}^2$-  
valued functions $r_{2}(t) = 〈sin(2t), cos(2t)〉$ and $r(t) = 〈sin(t), cos(t)〉$ over $0 ≤ t ≤ 2π$ (plotted  
as parametric curves $〈sin(2t), cos(2t), t〉$ and $〈sin(t), cos(t), t〉$ in 3D and treating the $z$-axis for  
the $t$-axis). They are different functions, but both $(sin(2t), cos(2t))$ and $(sin(t), cos(t))$ lie on  
the circle $x^2 + y^2 = 1$ as one can see from the top view over the z-axis and one would get both  
parametric curves as the curve $x^2 + y^2 = 1$ if one does not plot the $t$-axis.  

Likewise, two different vector-valued functions may produce the same curve in space, as is  
the case of $r(t) = 〈\cos t, \sin t, t〉$ and $r_{3}(t) = 〈\cos t^3, \sin t^3, t^3〉$. Note that $r_{3}(t) = r(t^3)$, which  
means that the point $r_{3}(t)$ is simply the point on the first curve at time $t^3$.  

So we use the terminology curve for a vector-valued function of one variable, but there is  
this subtle difference between its geometric interpretation and its property as a function.  

- Read the definition of the derivative of a vector-valued function $r(t) = 〈f (t), g(t), h(t)〉$and its interpretation as the velocity vector if a particle moves with time t according to this function.  
- Why does the definition of a smooth curve require that $\frac{dr}{dt}$ be continuous and never 0? Plot the curve $r(t) = (t^2, t^3, 0)$ and investigate whether it is smooth at the point corresponding to t = 0.  
- Study the definition of a piecewise smooth curve. Is the curve $r(t) = (t^2, t^3, 0)$ piecewise smooth according to this definition?  
- Interpret $||\frac{dr}{dt}‖$ as the speed and $\frac{d^2r}{dt^2}=r''(t)$ as the acceleration if a particle moves with time $t$ according to $r(t)$.  
- Read about the differentiation rules, paying particular attention to the Dot Product Rule, Cross Product Rule, and Chain Rule. 
- Study the property of a differentiable vector-valued function $r(t)$ satisfying ‖r(t)‖ equals a constant (Hint: $r(t) · r(t) = a$ constant, so its derivative in $t$ will be = 0).  


### Reading Questions/Quizzes 


1. Given $r(t) = 〈\cos t, \sin t, t〉$ and $r_{3}(t) = 〈\cos t^3, \sin t^3, t^3〉$. Plot both curves for $−1 ≤ t ≤ 1$ (you may use GeoGebra or Desmos) and compute $\frac{dr(t)}{dt}, ||\frac{dr(t)}{dt}||, \frac{d^2r(t)}{dt^2}, \frac{dr_{3}(t)}{dt}, ||\frac{dr_{3}(t)}{dt}||, \frac{d^2r_{3}(t)}{dt^2}$. Does $r(t)$ travel with constant velocity, or constant speed, or constant acceleration? What about $r_{3}(t)$? 
	1. $\frac{dr(t)}{dt}= <-\sin t,\cos t,1>$
	2. $||\frac{dr(t)}{dt}||=\sqrt{ \sin^2t+\cos^2t+1 }=\sqrt{ 2 }$
	3. $\frac{d^2r(t)}{dt^2}= <-\cos t,-\sin t,1>$
	4. $\frac{dr_{3}(t)}{dt}= <-3t^2\sin t^3,3t^2\cos t^3,3t^2>$
	5. $||\frac{dr_{3}(t)}{dt}||=\sqrt{ 9t^4\sin^2t^3+9t^4\cos^2t^3+3t^2 }=\sqrt{ 9t^4(\sin^2t^3+\cos^2t^3)+3t^2 }=t\sqrt{ 9t^2+3 }$
	6. $|| \frac{d^2r_{3}(t)}{dt^2})||= <-6t\sin t^3-9t^4\cos t^3,6t\cos t^3-9t^4\sin t^3,6t>$
	7. $r(t)$ does not travel with constant velocity, travels with constant speed, does not travel with constant acceleration
	8. $r_{3}(t)$ does not travel with constant velocity, speed, or acceleration
2. Set $v(t) = ‖r′(t)‖ = \sqrt{r′(t) · r′(t)}$. Derive a formula for $v′(t)$ in terms of $r′(t)$ and $r′′(t)$ 
	1. $v'(t)=\frac{r''(t)\cdot r'(t)}{\sqrt{ r'(t)\cdot r'(t) }}$