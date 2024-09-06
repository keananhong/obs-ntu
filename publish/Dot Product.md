Created: `16-Aug-2024`, `13:41`
Tags: [[SC1004 - Linear Algebra For Computing]]

# Dot Product
- angle between two vectors u and v is $0 \leq \theta \leq \pi$
	- cant be more than 180 obv
- the dot product between two vectors is 
	- $u * v = \lVert u \rVert \lVert v \rVert \cos \theta$
	- if either u or v is 0 then $u * v=0$
- $\theta$ can be derived from
	- $\cos \theta = \frac{u*v}{\lVert u\rVert \lVert v \rVert}$
	- cos theta is u dotprod v  over mag u mag v
	- theta is < 90deg if u.v > 0
	- theta is > 90deg if u.v < 0
	- theta is pi/2 or 90 if u.v = 0

# Component form of dot prod
- $u * v = u_1v_1+u_2v_2+u_nv_n$
- $v * v = v_1^2 +v_2^2+v_n^2 = \lVert v\rVert ^2$
- length of  a vector in terms of dot prod
	- $\lVert v \rVert = \sqrt{v \cdot v}$
- ![[Pasted image 20240816140250.png]]

# angles in R^n
- $\theta = \cos^{-1}(\frac{u \cdot v}{\lVert u \rVert \lVert v \rVert})$
- $\lvert u \cdot v \rvert \leq \lVert u \rVert \lVert v \rVert$
- ![[Pasted image 20240816141359.png]]

# Geometry
- $\lVert u+v \rVert \leq \lVert u \rVert + \lVert v \rVert$
	- magnitude of added vectors is less than mag u plus mag v
	- ![[Pasted image 20240816141552.png]]
	- same with distances