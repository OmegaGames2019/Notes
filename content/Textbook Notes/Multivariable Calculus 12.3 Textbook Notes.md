Status: Adult

![[12.3.pdf]]
## Formulas

- The work done by a constant force $F$ acting through a displacement $D=\overline{PQ}$ is $W=F\cdot D$

### Find definitions/descriptions for the following terms: 

- The dot product between two vectors 
	- The dot product $u\cdot v$ ("u dot v") of vectors $u= <u_{1},u_{2},u_{3}>$ and $v= <v_{1},v_{2},v_{3}>$ is the scalar $u\cdot v=u_{1}v_{1}+u_{2}v_{2}+u_{3}v_{3}$
- Compute angle between two vectors in terms of their dot product  
	- The angle $\theta$ between two nonzero vectors $u= <u_{1},u_{2},u_{3}>$ and $v= <v_{1},v_{2},v_{3}>$ is given by $\theta=\arccos\left( \frac{u_{1}v_{1}+u_{2}v_{2}+u_{3}v_{3}}{|u||v|} \right)=\arccos\left( \frac{u\cdot v}{|u||v|} \right)$
- Relation of dot product between vectors and the law of cosines 
	- ![[Parallelogram Law of Addition of Vectors | 300x400]]
	$|w|^2=|u|^2+|v|^2-2|u||v|\cos \theta$
	$2|u||v|\cos \theta=|u|^2+|v|^2-|w|^2$
	Because $w=u-v$, the component form of $w$ is $<u_{1}-v_{1},u_{2}-v_{2},u_{3}-v_{3}>$
	Therefore, $|u|^2=(\sqrt{ u_{1}^2+u_{2}^2+u_{3}^2 })^2=u_{1}^2+u_{2}^2+u_{3}^2$ 
	$|v|^2=(\sqrt{ v_{1}^2+v_{2}^2+v_{3}^2 })^2=v_{1}^2+v_{2}^2+v_{3}^2$
	$|w|^2=(\sqrt{ (u_{1}-v_{1})^2+(u_{2}-v_{2})^2+(u_{3}-v_{3})^2 })^2$
		$=(u_{1}-v_{1})^2+(u_{2}-v_{2})^2+(u_{3}-v_{3})^2$
		$=u_{1}^2-2u_{1}v_{1}+v_{1}^2+u_{2}^2-2u_{2}v_{2}+v_{2}^2+u_{3}^2-2u_{3}v_{3}+v_{3}^2$
	And $|u|^2+|v|^2-|w|^2=2(u_{1}v_{1}+u_{2}v_{2}+u_{3}v_{3})$
	Therefore, $2|u||v|\cos \theta=|u|^2+|v|^2-|w|^2=2(u_{1}v_{1}+u_{2}v_{2}+u_{3}v_{3})$
		$|u||v|\cos \theta=u_{1}v_{1}+u_{2}v_{2}+u_{3}v_{3}$
		$\cos\theta=\left( \frac{u_{1}v_{1}+u_{2}v_{2}+u_{3}v_{3}}{|u||v|} \right)=\left( \frac{u\cdot v}{|u||v|} \right)$
		$\theta=\arccos\left( \frac{u\cdot v}{|u||v|} \right)$
- Orthogonal relation between two vectors in terms of their dot product 
	- Vectors $u$ and $v$ are orthogonal if $u\cdot v=0$
- Algebraic properties of the dot product 
	- $u\cdot v=v\cdot u$
	- $(cu)\cdot v=u\cdot(cv)=c(u\cdot v)$
	- $u\cdot(v+w)=u\cdot v+u\cdot w$
	- $u\cdot u=|u|^2$
	- $0\cdot u=0$
- The scalar component of u in the direction of v and the (orthogonal) projection of u in the direction of v.
	- The vector projection of $u$ onto $v$ is the vector $proj_{v}u=\left( \frac{u\cdot v}{|v|^2} \right)=\left( \frac{u\cdot v}{|v|} \right) \frac{v}{|v|}$
	- The scalar component of $u$ in the direction of $v$ is the scalar $|u|\cos \theta=\frac{u\cdot v}{|v|}=u\cdot \frac{v}{|v|}$

### Reading Questions/Quizzes

- Is $u \cdot v$ always a nonnegative number for any vectors u and v? 
	- Because $u\cdot v=|u||v|\cos \theta$, and $\cos \theta$ can be negative, $u\cdot v$ is not always a nonnegative number
- Is the scalar component of u in the direction of v always a nonnegative number for any vectors u and v? 
	- Because the scalar component is $|u|\cos \theta$ and $\cos \theta$ can be negative, it is not always a nonnegative number 
- Is the scalar component of u in the direction of v a vector? 
	- No, a scalar is not a vector 
- Is the projection of u in the direction of v a vector or a scalar? 
	- Yes, because it is a vector projection 
- Is it true that $(u-proj_{v}u)\cdot v=0$?  
	- Yes, because $u-proj_{v}u$ represents the orthogonal vector to $v$ and the dot product of two orthogonal vectors is 0, it is true 
- Is it true that |u · v| ≤ |u||v| always holds? 
	- Yes (see Cauchy-Schwarz Inequality) 
- When does u · v = |u||v| hold? When does u · v = −|u||v| hold?  
	- The former holds when the vectors are pointing in the same direction, and the latter holds when the vectors are pointing in equally opposite directions
- Is it possible that u · v = 2|u||v| for non-zero vectors u, v?
	- No, because the maximum value for cosine is 1, which means the max value for $u\cdot v=|u||v|\cos \theta$ is $|u||v|$ at $\theta=0+2\pi n$ when $\cos \theta=1$

## References

[[Multivariable Full Textbook.pdf]]
[[12.3.pdf]]