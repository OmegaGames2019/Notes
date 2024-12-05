
Status: 

![[15.2.pdf]]


## 15.2 Double Integrals Over More General Regions

The bad news is this is a very long section. The good news is that it there are more examples than in the previous section. The reason there are so many examples is because the domains over which we are integrating can be many different shapes in R2. The main idea is that you want to set up an iterated integral as we did for rectangles, but the limits of integration for the inner integral will usually be in terms of the other variable. Honestly, you just need to look at lots of examples to see how that works in practice. 

Find the following definitions/concepts/formulas/theorems: 

- Fubini’s Theorem (a stronger form which applies to non-rectangular regions)  
- vertical/horizontal cross-sections (I will introduce the terms horizontally/vertically simple in lecture)  
- Properties of Double Integrals (none of which should surprise you)

The first couple of pages deal with how we generalize domains and what properties they need to have. **Example 1** is a basic example of integration over a triangular domain. They calculate this integral in both of the possible orders to provide evidence that Fubini’s Theorem works. Notice that when the inner integral is dy, that we have an x in the upper limit of integration. When the inner integral is dx, we have a y in the lower limit of integration. In general, you can only have variables in your limits of integration which are NOT the variable you are currently integrating with respect to but ARE variables that you will be integrating with respect to later in the iterated integral. This is true for triple integrals as well.  

**Example 2** is important because the order of integration matters. The choice is forced because if you try to integrate with respect to x first, the integrand is unmanageable. When we integrate with respect to y first, something good happens.  
**Example 3** just asks us to switch the order of integration. The technique here is that you draw the region of integration, rewrite the boundary curves so that they are functions of the other variable (recall inverse functions from high-school algebra), then use those new functions as the limits of integration. For practice, evaluate both of these integrals to make sure the book isn’t lying to you about the value.

**Example 4** is interesting mostly for the setup of the integral. The evaluation is annoying, and the fraction arithmetic is worse. Look at it, but don’t worry about it too much. 

### Reading Questions/Quizzes 

1. Sketch the regions of integration associated with the given double integral and rewrite it as a double integral with the order of integration reversed. 
	1. $\int_{-2}^{2}\int_{y^2}^4f(x,y)dxdy$
	2. $\int_{0}^4\int_{x^2}^{4x}f(x,y)dydx$
2. Evaluate the double integrals (sometimes it’s easier to do the integral in reverse order). 
	1. $\int_{-2}^2\int_{y^2}^4e^{\frac{y}{\sqrt{ x }}}dxdy$
	2. $\int_{0}^1\int_{x}^1e^{y^2}dydx$