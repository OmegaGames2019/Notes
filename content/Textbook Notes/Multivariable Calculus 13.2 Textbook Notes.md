
Status: Baby 

![[13.2.pdf]]

### Integrals of Vector Functions; Projectile Motion

When $r(t) = 〈f (t), g(t), h(t)〉$ and the (indefinite or definite) integrals of $f (t), g(t), h(t)$ are defined, we can define the integral of $r(t)$ accordingly:  

$\int r(t)dt= <\int f(t)dt,\int g(t)dt,\int h(t)dt> \text{ or } \int_{a}^br(t)dt= <\int_{a}^{b}f(t)dt,\int_{a}^{b}g(t)dt,\int_{a}^{b}h(t)dt>$

If we apply this definition to $\frac{dr(t)}{dt}$ in place of $r(t)$, we see that $\int_{a}^{b}  \frac{dr(t)}{dt}dt=\int_{a}^br'(t)dt=r(b)-r(a)$ holds and it represents the net displacement of $r(t)$ from $t = a$ to $t = b$, while $\int_{a}^b ||\frac{dr(t)}{dt}||dt=\int_{a}^b||r'(t)||dt$ represents the total distance the particle traveled following the  
curve $r(t)$ from $t = a$ to $t = b$.  

In the study of ideal projectile motion, one studies a vector-valued function $r(t) = 〈x(t), y(t), z(t)〉$ satisfying $r′′(t) = 〈0, −g, 0〉, r′(0) = v_{0} \text{ and } r(0) = r_{0}$ given,  
where $g$ is the gravitational constant (with a value of 9.8 $\frac{m}{s^2}$). One can immediately reduce this into the one-variable calculus problems:  
$x′′(t) = 0, x(0) = x_{0}, x′(0) = v_{1}; y′′(0) = −g, y(0) = y_{0}, y′(0) = v_{2}; z′′(t) = 0, z(0) = z_{0}, z′(0) = v_{3}$

### Reading Questions/Quizzes

1. Find solutions of the above and reconcile this with the discussion as given in the textbook, especially the relation between v0, α in the textbook and v1, v2, v3 here (Note that in the textbook discussion, z-component is not introduced and j is used to represent the vertical direction, which corresponds to setting v3 = 0 so z(t) = z0 for all t here.)  
4. Compute $\int_{0}^\pi[(-\sin t)i+(\cos t)j+k]dt$
	1. $[(\cos t)i+(\sin t)j+tk]_{0}^\pi=(-1-1)i+(0-0)j+(\pi-0)k=-2i+\pi k$