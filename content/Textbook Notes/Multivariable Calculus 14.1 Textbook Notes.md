
Status: Baby

![[14.1.pdf]]

### 14.1 Functions of Several Variables

In Calculus I and II, we spend (almost) all of our time discussing functions with one input  
and one output. In chapter 13, we discussed vector-valued functions which we can think of as functions with one input and several outputs. In this section, we will explore functions of two  
or three variables, which have multiple inputs and a single (scalar) output. Almost all of our  
discussion apply to functions of four or more variables, but we should focus on two or three first  
and use the working experience in such settings to apply the same rules to higher dimensions.  
Our main goal is to understand how these functions behave and how the concepts in one variable calculus extend to functions of multi-variables, such as the limit of a function on approach to a point, the continuity and differentiability of a function at a point, how to the  
points where a function attains its maximum or minimum, how to integrate a function of multi-  
variables, etc.  

One basic step is to understand when different input variables have the same output values.  
One way to do this is to construct the graph of such functions, which would give a sense of  
which input variables give higher output values and which give lower output values.  
These functions are difficult to draw by hand for a function of two-variables $z = f (x, y)$, and  
they become essentially impossible to draw with three or more input variables. An alternative  
way to visualize these functions is to consider their level curves (and level surfaces with more  
than two inputs). Namely, we don’t draw an axis for the output variable, but only draw the sets  
of input variables that give the same output values: for the function $z = f (x, y)$, we take various  
values $c$ and for each $c$, we figure out the set $C_{c} = \{(x, y) : f (x, y) = c\}$, which typically is a curve  
in the $xy$-plane; while for the function $w = g(x, y, z)$, we consider $S_{c} = \{(x, y, z) : g(x, y, z) = c\}$,  
which typically is a surface in the $xyz$ space (as, for any given c, one aims to solve one of the  
variables in terms of the remaining two, therefore identifying the set as a graph of two variables).  
You can use Matlab, Maple, Mathematica, Desmos, or GeoGebra to draw the graph or level  
curve many functions of two variables and level surface of functions of three variables.  
Later on we will discuss functions which have both multiple inputs and multiple outputs.  
Functions with the same number of inputs and outputs are vector fields which are the focus of  
chapter 16 at the end of this course.  

This section introduces many concepts, but most have an intuitive geometric meaning. Find  
the following definitions/concepts:  

- Function of $n$ variables: its domain and range (One can specify any set as the domain, but when a function is given in terms of some algebraic expressions, one generally takes its domain to be the largest set on which the expressions are well defined.)  
	- What does the domain of a function of $n$ variables look like? (Think mostly about $n = 2$ and $n =3$ or your head will start to hurt. Trust me on this one.)  
		- For $n=2$, the domain will be an expression that can be represented on a one-dimensional number line. To that end, for $n=3$, the domain is an expression that can be represented in a two-dimensional coordinate plane. 
	- What does the range of a function of $n$ variables look like?  
		- For $n=2$, the range is a set of values that can be expressed on a two-dimensional coordinate plane. To that end, for $n=3$, the range is a set of values that can be expressed on a three-dimensional coordinate plane. 
- Interior/interior point 
	- A point $(x_{0},y_{0})$ in a region (set) R in the $xy$-plane is an interior point of $R$ if it is the center of a disk of positive radius that lies entirely in $R$ (**Figure 14.2**).
- Boundary/boundary point 
	- A point $(c_{0},y_{0})$ is a boundary point of $R$ if every disk centered at $(x_{0},y_{0})$ contains points that lie outside of $R$ as well as points that lie in $R$. (The boundary point itself need not belong to $R$.) 
- Open vs. closed regions (in $\mathbb{R}$, these are exactly the open and closed intervals you know from high school) 
	- A region is open if it consists entirely of interior points. A region is closed if it contains all its boundary points (**Figure 14.3**).
- Bounded vs. unbounded sets 
	- A region in the plane is bounded if it lies inside a disk of finite radius. A region is unbounded if it is not bounded. 
- Graphing a function of two variables 
	- Graph the function's level curves and go from there. Let a variable $c$ equal some arbitrary values (preferably whole numbers) and substitute $c$ for $z$. This will yield a function in $\mathbb{R}^2$ that can easily be graphed on the $xy$-plane. 
- Level curve/graph/surface contour curve (what is the difference between a level curve and a contour curve?)  
	- The set of points in the plane where a function $f(xy)$, has a constant value $f(x,y)=c$, is called a level curve of $f$. The set of all points $x,y,f(x,y)$ in space, for $(x,y)$, in the domain of $f$, is called the graph of $f$. The graph of $f$ is often called the surface $z=f(x,y)$
- Graphing a function of three variables level surface 
	- Using the same principles as graphing a function of two variables, substitute some arbitrary value $c$ for $w$. This will yield a function in $\mathbb{R}^3$, which can be graphed by finding the level curves of that surface. 
- How does direction relate to rate of change of the function values (teaser: this relates to directional derivatives in section 14.5) 
	- The function values will change differently depending on which direction you travel on the graph because steepness will vary depending on which direction you go in. 

The motivating examples above **Example 1** are intended to give you a feel for when you  
will need to use multivariable functions to model real-world phenomena. **Examples 1 and 2**  
describe how to find the domain and range of a function of several variables. These are must-  
read (and understand). **Example 3**, the paragraph below it, and the pictures in the left margin  
are all about being able to visualize graphs of functions of two variables.  

Any time you have $z = f (x, y)$, you are going to get some graph in $\mathbb{R}^3$ which includes  
exactly one point above, at, or below each point in the $xy$-plane which is in your domain. If $f$ is  
continuous, the graph is a surface without teat in some sense. You should spend some serious  
time on the details. Doing so will help develop your intuition about what these functions  
are doing at various points in space, which will certainly make the rest of the chapter more  
manageable.  

The section on functions of three variables needs some motivation. There are many real world  
situations where we are interested in what some quantity is doing at every point in some 3 or  
higher dimensional space. **Figure 14** on page 810 shows several level surfaces of the function  
in **Example 4**.  

### Reading Questions/Quizzes:  

1. Let $D$ denote the round disk $\{(x, y) : x^2 + y^2 < 1\}$ with its center deleted. Is the center an interior or boundary point of such a domain? Identify all interior and boundary points of this domain. Is $D$ an open region?  
	1. Since the center is not a part of the region, it is a boundary point. It can be reached through any path taken on the interior of the region, but is not part of the region. 
	2. Interior points: $0<x^2+y^2<1$
	3. Boundary points: $x^2+y^2=1$
	4. Open: Yes (because the region does not contain the boundary points) 
	5. The domain is defied by $D_{F}=\{(x,y):x^2+y^2<1,(x,y)\neq(0,0)\}$
2. Let $S$ denote the square ${(x, y) : |x| ≤ 2, |y| ≤ 2}$ with the smaller square $\{(x, y) : |x| ≤ 1, |y| ≤ 1\}$ removed. Identify all interior and boundary points of this domain. Is $S$ an open region? 
	1. Interior points: $1<|x|<2 \text{ and } 1<|y|<2$
	2. Boundary points: $|x|=1,2 \text{ and } |y|=1,2$
	3. Open: No (because the region contains its boundary points) 
3. Describe the level sets of the function $z = x^2 − y^2$.  
	1. The level sets of this function are represented by linear lines. Each level set has two linear lines, with one being a reflection of the other about the $y$-axis. The resulting surface is classified as a cone (one that goes below the $yz$-plane too) 
