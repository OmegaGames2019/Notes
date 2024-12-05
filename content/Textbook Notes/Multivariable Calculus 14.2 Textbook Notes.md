
Status: Baby

![[14.2.pdf]]

### 14.2 Limits and Continuity in Several Variables  

In Calculus I (probably in Precalculus as well), you learned about limits and continuity. When  
you defined $lim_{x→c} f (x)$, you were told that in order for this limit to exist that the two one-sided  
limits had to exist and be equal. And then you were told that in order for a function to be  
continuous at some point $x = c$ that $lim_{x→c} f (x)$ and $f (c)$ both had to exist and they had to be  
equal.  

In multi-dimensions the limits are very different in one particular way. When you only have  
one real input variable, your domain is just part of the number line. If you look at a point on  
the number line, there are only two ways to approach it: from below (or left) and from above  
(or right). But if we are talking about $f (x, y)$, the domain is some part of the plane $\mathbb{R}^2$. For  
an arbitrary point in the middle of your domain, there are infinitely many paths that you can  
follow to get there. The limit only exists if it is the same on any of these infinitely many paths.  

Since there is no good way to enumerate these infinitely many paths, the proper way to describe  
a function having a limit at some $(x_{0}, y_{0})$ in the domain is as done in the Definition at the  
beginning of the section.  

In situations where $lim_{(x,y)→(x_{0},y_{0})} f (x, y)$ exists, the continuity condition $lim_{(x,y)→(x_{0},y_{0})} f (x, y)=f (x_{0}, y_{0})$ is straightforward to check. To show that f (x, y) is not continuous at $(x_{0}, y_{0})$, one has to show that either $lim_{(x,y)→(x_{0},y_{0})} f (x, y)$ does not exist or it does exist but not equal $f (x_{0}, y_{0})$. The first possibility is often harder to address (read the Two-Path Test)  

Find the following definitions/concepts/formulas/theorems:  

- Limit of a function of two variables ($\epsilon$-$\delta$ definition) 
	- Suppose that every open circular disk centered at $(x_{0},y_{0})$ contains a point in the domain of $f$ other than $(x_{0},y_{0})$ itself. We say that a function $f(x,y)$, approaches the limit $L$ as $(x,y)$ approaches $(x_{0},y_{0})$ and write $\displaystyle\lim_{ (x,y) \to (x_{0},y_{0}) }f(x,y)=L$ if, for every number $\epsilon<0$, there exists a corresponding number $\delta>0$ such that for all $(x,y)$ in the domain of $f$, $|f(x,y)-L|<\epsilon$ whenever $0<\sqrt{ (x-x_{0})^2+(y-y_{0})^2 }<\delta$
- Theorem 1: Properties of Limits (functions of two variables)  
	- ![[Theorem 1 of Limits of Functions of Two Variables.png]]
- Techniques for showing that the limit of a function of two variables does not exist (Two-Path Test)  
	- Take the limit of the function as it approaches from two or more paths. 
	- If a function $f(x,y)$ has different limits along different paths in the domain of $f$ as $(x,y)$ approaches $(x_{0},y_{0})$, then $\displaystyle\lim_{ (x,y) \to (x_{0},y_{0}) }f(x,y)$ does not exist. 
- Continuity (functions of two variables) 
	- Suppose that every open circular disk centered at $(x_{0},y_{0})$ contains a point in the domain of $f$ other than $x_{0},y_{0}$ itself. Then a function $f(x,y)$ is continuous at the point $(x_{0},y_{0})$ if 
		- $f$ is defined at $(x_{0},y_{0})$
		- $\displaystyle\lim_{ (x,y) \to (x_{0},y_{0}) }f(x,y)$ exists 
		- $\displaystyle\lim_{ (x,y) \to (x_{0},y_{0}) }f(x,y)=f(x_{0},y_{0})$
	- A function is continuous if it is continuous at every point of its domain 
- Continuity of compositions of continuous functions (this part is the same as for the one variable case) 
	- As with the definition of limit, the definition of continuity applies at boundary points as well as interior points of the domain of $f$. 
	- A consequence of Theorem 1 is that algebraic combinations of continuous functions are continuous at every point at which all the functions involved are defined. This means that sums, differences, constant multiples, products, quotients, and powers of continuous functions are continuous where defined. In particular, polynomials and rational functions of two variables are continuous at every point at which they are defined. 
	- If $f$ is continuous at $(x_{0},y_{0})$ and $g$ is a single-variable function continuous at $x_{0},y_{0}$, then the composition $h=g \circ f$ defined by $h(x,y)=g(f(x,y))$ is also continuous at $(x_{0},y_{0})$
- Limit of a function of three variables 
	- The definitions of limit and continuity for functions of two variables and the conclusions about limits and continuity for sums, products, quotients, powers, and compositions all extend to functions of three or more variables 
- Extreme Value Theorem (multivariable edition; the new ingredient is the domain must be a closed bounded set) 
	- The Extreme Value Theorem (Theorem 1, Section 4.1) states that a function of a single variable that is continuous at every point of a closed, bounded interval $[a,b]$ takes on an absolute maximum value and an absolute minimum value at least once in $[a,b]$. The same holds true of a function $z=f(x,y)$, that is continuous on a closed, bounded set $R$ in the plane (like a line segment, a disk, or a filled-in triangle). The function takes on an absolute maximum value at some point in $R$ and an absolute minimum value at some point in $R$. The function may take on a maximum or minimum value more than once over $R$. Similar results hold for functions of three or more variables. A continuous function $w=f(x,y,z)$ must take on absolute maximum and minimum values on any closed, bounded set (such as a solid ball or cube, spherical shell, or rectangular solid) on which it is defined. We will learn how to find these extreme values in Section 14.7. 
- Important: There is a technique for showing that a limit (of a two-variable function) exists by using the Sandwich Theorem (a/k/a the Squeeze Theorem). Note that this technique does not appear in the main body of the section. It is on page 822, below exercise 58. Please read it, and we will discuss it in class. 
	- TK
- Important: There is a technique for showing that a limit (of a two-variable function) exists by switching to polar coordinates. Note that this technique does not appear in the main body of the section. It is on page 822, below exercise 64. Please read it, and we will discuss it in class.  
	- TK

**Examples 1 and 2** are short and direct applications of rules to (reasonably) well-behaved functions. Make sure that you look at the justifications carefully, though. One of the most common errors on this type of question is applying some limit law or theorem incorrectly and getting a value for a limit when the limit does not actually exist. **Example 2** has a peculiar feature that the textbook didn’t address: the function is defined only for $x > 0, y > 0$ and $x \neq y$, and $(0, 0)$ is not an interior point of the domain of definition of this function; however, the technique for dealing with this quotient of $\frac{0}{0}$ form is worth pondering—l’Hopistal’s rule does not apply in this multi-dimension setting.  

**Example 3** uses the $\epsilon$-$\delta$ definition to find the limit. This problem is much easier by converting to polar coordinates, which we will do in class, because the condition $\sqrt{ x^2+y^2 }< δ$ is most naturally expressed as $r < δ$ in polar coordinates. **Example 4** uses the $\epsilon$-$δ$ definition to show that a limit does not exist. I do not expect you to apply the $\epsilon$-$δ$ definition on quizzes or exams. **Example 5** is a standard example of how you go about testing continuity at a point in the domain of a multivariable function. Example 6 uses the Two-Path Test to show that a limit does not exist.  

It’s very nice when you find two different limits as you approach the point on two different lines or curves. The frustrating part is that sometimes you consider lots of different paths and get the same limit every time, but you can’t find one that’s different. And you also can’t find a theorem that tells you that the function actually has a limit. This is what a lot of higher level math (and much of mathematical research) is like. You try to prove that something is true for a while and can’t. Then you spend some time trying to find a counterexample that shows the something is false and you can’t. But some of the counterexamples you tried gave you a new technique that you use to try and prove the theorem... and you still can’t prove the theorem. But it is very satisfying when you end up with either a valid proof or a valid counterexample after a long struggle.  

### Reading Questions/Quizzes:  

1.  What rules of Theorem 1 allow one to draw quick conclusions on the limit $\\lim_{ (x,y) \to (2,-3) }\left( \frac{1}{x}+\frac{1}{y} \right)^2$
	1. Utilizing the power rule, this can be simplified into squaring the limit of just the inside of the parenthetical 
2. What rules of Theorem 1 allow one to draw quick conclusions on the limit $\lim_{ (x,y) \to (0,0) } \frac{e^y\sin x}{x}$
	1. Using the product rule, this limit can be found by splitting it into two different limits, with the first being the limit of $e^y$ and the second being the limit of $\frac{\sin x}{x}$ 
3. By considering different paths of approach, show that the function $\frac{x^2}{x^2+y^2}$ does not have a limit as $(x, y) → (0, 0)$ 
	1. With the path as $x=0$, the limit evaluates to $0$. However, with the path as $y=0$, the limit evaluates to $1$. Therefore, the limit does not exist. 