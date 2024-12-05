
Status: 

![[15.8.pdf]]

## 15.8 Substitutions in Multiple Integrals 

Just as change of variables is an important tool in evaluating integrals in one variable, the same is true in evaluating integrals in several variables. In this section we study how this is done. We already worked with some specific change of variables: from rectangular coordinates $(x,y)$ to its polar coordinates $(r,\theta)$, where the integral in $dxdy$ changes into integrals in $rdr d\theta$; similarly from rectangular coordinates $(x,y,z)$ to its cylindrical coordinates $(r,\theta,z)$, where the integral in $dxdydz$ changes into integrals in $r dr d\theta dz$; and from rectangular coordinates $(x,y,z)$ to its spherical coordinates $(\rho,\theta,\phi)$, where the integral in $dxdydz$ changes into integrals in $\rho^2\sin \phi d\rho d\theta d\phi$. In this section, we will study the general rule for change of variables in multiple integrals. 

A change of variables in two variables from $(x,y)$ to $(u,v)$ can be expressed as $x=g(u,v),\text{ } y=h(u,v)$. We assume that it transforms the region $D$ in the $(x,y)$ variables into a region $G$ in the $(u,v)$ variables. We also assume that both $g$ and $h$ have continuous partial derivatives for $(u,v)\in G$. The key ingredient is a change of variables in multiple variable integral is the Jacobian matrix $\begin{bmatrix} \frac{\partial x}{\partial u} \frac{\partial x}{\partial v}\\ \frac{\partial y}{\partial u} \frac{\partial y}{\partial v}\end{bmatrix}$ and Jacobian determinant in $J(u,v)=\det\begin{bmatrix} \frac{\partial x}{\partial u} \frac{\partial x}{\partial v}\\ \frac{\partial y}{\partial u} \frac{\partial y}{\partial v}\end{bmatrix}$. Another notation for $J(u,v)$ is $\displaystyle\frac{\partial(x,y)}{\partial(u,v)}$. 

Similarly for a change of variable in three variables. The reason that this matrix and its determinant enters is through linear approximation of $(u,v)\mapsto(g(u,v),h(u,v))$: suppose we do a partition of $G$ into small rectangles parallel to the $u$ and $v$ axes, and $(u,v)$ is the vertex of one such rectangle and $\Delta u$ and $\Delta v$ are the lengths of this small rectangle, $$\begin{bmatrix}
g(u+\Delta u,v+\Delta v)-g(u,v) \\
h(u+\Delta u,v+\Delta v)-h(u,v)
\end{bmatrix}\approx \begin{bmatrix}
\frac{\partial x}{\partial u} \frac{\partial x}{\partial v} \\ \frac{\partial y}{\partial u} \frac{\partial y}{\partial v} 
\end{bmatrix} \begin{bmatrix}
\Delta u \\
\Delta v
\end{bmatrix}$$ up to an error which is vanishingly small compared to $\sqrt{ (\Delta u)^2+(\Delta v)^2 }$. Then the image in $D$ of this rectangle is approximated by the parallelogram with edges $$\begin{bmatrix}
\frac{\partial x}{\partial u} \\
\frac{\partial y}{\partial u}
\end{bmatrix}\Delta u\text{ and } \begin{bmatrix}
\frac{\partial x}{\partial v} \\
\frac{\partial y}{\partial v}
\end{bmatrix}\Delta v;$$ the area of this parallelogram is $$\left| \det \begin{bmatrix}
\frac{\partial x}{\partial u}\Delta u & \frac{\partial x}{\partial v}\Delta v \\
\frac{\partial y}{\partial u}\Delta u & \frac{\partial y}{\partial v}\Delta u
\end{bmatrix}\right|=\left|\det \begin{bmatrix}
\frac{\partial x}{\partial u} \frac{\partial x}{\partial v}\\ \frac{\partial y}{\partial u} \frac{\partial y}{\partial v}
\end{bmatrix}\right||\Delta u\Delta v|=||J(u,v)||\Delta u\Delta v|.$$ This is how $|J(u,v)$ enters into the change of variables formula. 

In actual implementation of change of variables, the harder part is to find an appropriate $g$ and $h$ such that the corresponding region of integration $G$ is easy to work with (as close to a rectangular region as possible) and the resulting integral is easy to evaluate. 

When making a linear change of variables $$\begin{bmatrix}
x \\
y
\end{bmatrix}=\begin{bmatrix}
a & c \\
b & d
\end{bmatrix} \begin{bmatrix}
u \\
v
\end{bmatrix}$$ the vector $\begin{bmatrix}u\\v\end{bmatrix}=\begin{bmatrix}1\\0\end{bmatrix}$ maps to $\begin{bmatrix}x\\y\end{bmatrix}=\begin{bmatrix}a\\b\end{bmatrix}$, while the vector $\begin{bmatrix}u\\v\end{bmatrix}=\begin{bmatrix}0\\1\end{bmatrix}$ maps to $\begin{bmatrix}x\\y\end{bmatrix}=\begin{bmatrix}c\\d\end{bmatrix}$, so the unit square in the $uv$-plane with the origin $\begin{bmatrix}1\\0\end{bmatrix},\begin{bmatrix}0\\1\end{bmatrix},\text{ and }\begin{bmatrix}1\\1\end{bmatrix}$ as its vertices is mapped to the parallelogram in the $xy$-plane with the origin, $\begin{bmatrix}a\\b\end{bmatrix},\begin{bmatrix}c\\d\end{bmatrix},\text{ and }\begin{bmatrix}a+c\\b+d\end{bmatrix}$ as its vertices. 

Find the following definitions/concepts/formulas/theorems: 

- Coordinate transformation (aka map or mapping) 
- One-to-one transformation/map (means the same thing it did in high school algebra) 
- Image/preimage 
- Jacobian (aka Jacobian determinant - you should notice that there are several notations) 
- Theorem: Substitution for Double Integrals (aka Change of Variables Formula) 
- Polar coordinates map (in **Example 1**)
- Linear transformation/map
- Change of variables formula for three variables 
- Jacobian equivalent for cylindrical and spherical coordinates 

**Example 1** just computes the Jacobian for polar coordinates. We showed why the $r$ was there geometrically (and informally), and this is a completely independent justification for the presence of $r$ in $r dr d\theta$. 

**Examples 2 and 3** work with linear maps between coordinate systems. **Example 2** can be done without making a change of variables, but the important thing to learn is how a linear change of variables maps a rectangle to a parallelogram. In **Example 3**, the part that causes difficulty in evaluating the integral is the factor $\sqrt{ x+y }$, while the $(y-2x)^2$ factor is manageable. The choice of change of variables is not unique. One could also work with $\tilde{u}=x$ (namely, no change on $x$), and $\tilde{v}=x+y$, then $$\sqrt{ x+y }(y-2x)^2=\sqrt{ \tilde{v} }(\tilde{v}-2\tilde{u})^2=\sqrt{ \tilde{v} }(\tilde{v}^2-2\tilde{u}\tilde{v}+4\tilde{u}^2),$$ and the region of integration in $\tilde{u},\tilde{v}$ becomes $\tilde{G}:0\leq \tilde{u}\leq 1, \tilde{u}\leq \tilde{v}\leq1$. Note that we often introduce $u,v$ as functions of $x,y$ and then need to invert it to find $x,y$ as functions of $u,v$. But an important property as a consequence of implicit differentiation, we have $$J(u,v)=\det \begin{bmatrix}
\frac{\partial x}{\partial u}  & \frac{\partial x}{\partial v}  \\
\frac{\partial y}{\partial u} & \frac{\partial y}{\partial v}
\end{bmatrix}=\left(\det \begin{bmatrix}
\frac{\partial u}{\partial x} & \frac{\partial u}{\partial y} \\
\frac{\partial v}{\partial x} & \frac{\partial v}{\partial y}
\end{bmatrix}\right)^{-1}$$ so we need not necessarily find the inverse directly but only compute $$\det \begin{bmatrix}
\frac{\partial x}{\partial u}  & \frac{\partial x}{\partial v}  \\
\frac{\partial y}{\partial u} & \frac{\partial y}{\partial v}
\end{bmatrix}.$$ In the case of our $\tilde{u}=x,\tilde{v}=x+y$, $$\det \begin{bmatrix}
\frac{\partial \tilde{u}}{\partial x} & \frac{\partial \tilde{u}}{\partial y} \\
\frac{\partial \tilde{v}}{\partial x} & \frac{\partial \tilde{v}}{\partial y}
\end{bmatrix}=\det \begin{bmatrix}
1 & 0 \\
1 & 1
\end{bmatrix}=1$$
**Example 4** is a more complicated example, mostly because the map is nonlinear and the change of variable is a bit artificial. Can $u=xy,v=y$ work? 

**Example 5** is a linear transformation, but with the twist that there are three independent variables. The key point is still that we are mapping a slanted solid region into a rectangular one because the integration process is simpler. 
 

### Reading Questions/Quizzes 

1. For the change of variables given by $u=x-y,v=2x+y$, find $\frac{\partial(x,y)}{\partial(u,v)}$. 
2. Find a linear change of variables to transform the parallelogram $\mathcal{R}$ in the $xy$-plane with the origin, $\begin{bmatrix}1\\2\end{bmatrix},\begin{bmatrix}1\\4\end{bmatrix},\text{ and }\begin{bmatrix}2\\6\end{bmatrix}$ as its vertices into the unit square in the $uv$-plane the origin, $\begin{bmatrix}1\\0\end{bmatrix},\begin{bmatrix}0\\1\end{bmatrix},\text{ and }\begin{bmatrix}1\\1\end{bmatrix}$ as its vertices. Then compute $\frac{\partial(x,y)}{\partial(u,v)}$ and evaluate $\iint_{\mathcal{R}}ydxdy$. 
3. In the set up of the above problem, suppose $\mathcal{R}$ is a region in the $xy$-plane with area 5 and $\mathcal{G}$ is the region in the $uv$-plane mapped from $\mathcal{R}$ by this change of variables. Find the area of $\mathcal{G}$. 
4. Solve the system $$u=x-y,\text{ }v=2x+y$$ for $x$ and $y$ in terms of $u$ and $v$. Then find the value of the Jacobian $\frac{\partial(x,y)}{\partial(u,v)}$. Also, find the image under the transformation $u=x-y, \text{ } v=2x+y$ of the triangular region with vertices $(0,0), (1,1), \text{ and } (1,-2)$ in the $xy$-plane. Sketch the transformed region in the $uv$-plane. 
5. For $u=x-y,v=2x+y$ in the previous problem, verify that $\frac{\partial(x,y)}{\partial(u,v)}=\left( \frac{\partial(u,v)}{\partial(x,y)} \right)^{-1}.$
6. For the change of variables from rectangular coordinates $(x,y)$ to polar coordinates, verify that $\frac{\partial(x,y)}{\partial(r,\theta)}=r.$
7. Use the transformation from number 4 to evaluate the integral $$\iint_{\mathcal{R}}(3x^2+14xy+8y^2)dxdy$$ for the region $\mathcal{R}$ bounded by the lines $y=-\frac{3}{2}x+1,y=-\frac{3}{2}x+3,y=-\frac{1}{4}x,\text{ and }y=-\frac{1}{4}x+1.$
8. Let $\mathcal{R}$ be the region in the first quadrant of the $xy$-plane bounded by the hyperbolas $xy=1,xy=9$, and the lines $y=x,y=4x$. Use the transformation $x=\frac{u}{v},y=uv$ with $u>0$ and $v>0$ to rewrite $$\iint_{\mathcal{R}}\left( \sqrt{ \frac{y}{x} }+\sqrt{ xy } \right)dxdy$$ as an integral over an appropriate region $\mathcal{G}$ in the $uv$-plane. Then evaluate the $uv$-integral over $\mathcal{G}$. 
9. Evaluate the appropriate determinant to show that the Jacobian of the transformation from Cartesian $\rho \phi\theta$-space to Cartesian $xyz$-space is $\rho^2\sin \phi$. 