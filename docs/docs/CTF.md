---
File: 
aliases: 
share: True
Title: The Classical Theory of Field
Type: Book
Status: Reading
Author: 
- Landau L.D.
- Lifshitz E.M.
Stars: ⭐⭐⭐⭐
url: 
tags: 
---
# Chapter 2 Relativistic Mechanics

## The Principle of Least Action

 For each mechanical system, there exists a certain integral $S$ called $action$, which has a minimum(or extremum) for the actual motion so that its variation $\delta S$ is zero.

Consider a free particle: the action of a free particle must not depend on the frame of reference → the action must be Lorentz invariant—that is a scalar → the integrand must be a differential of the first order → the action of a free particle must have the form
$$S = -\alpha \int_a^b ds$$
where the integral is along the world line and $a$ and $b$ are two given world points, $\alpha$ is some constant that characterizes the particle.

!!! TIP "As we can see in § 3, $\int_a^bds$ has a maximum along a straight line, so the constant $\alpha$ must be positive."

***The action of a free particle has a maximum when the integral path is a straight line between the two given world points.*** So we can say the world line of a free particle is a straight line in spacetime.

Write the action in the form
$$ S = \int_{t_1}^{t_2} Ldt. $$

It’s the integral of time. $L(t)$ is the $Lagrange function$ of the mechanical system.

Because the interval in 4-space can be written as 
$$ds = c\sqrt{1-\frac{v^2}{c^2}}dt$$
so the action becomes 
$$S = -\int_{t_1}^{t_2} {\alpha c\sqrt{1-\frac{v^2}{c^2}}dt}$$
where $v$ is the velocity of the particle. So the Lagrangian for the particle is 
$$L = -\alpha c \sqrt{1-\frac{v^2}{c^2}}.$$

When the velocity is much smaller than $c$ , we should get $L = mv^2/2$ . So when $c\to \infty$, we have
$$\lim_{c\to\infty} L = -\alpha c + \frac{\alpha v^2}{2c} \approx \frac{1}{2}mv^2.$$
The term $\alpha c$ is just a constant and won't affect the equation of motion, so we can ignore that and have $\alpha = mc$.

Thus the action for a free particle is 
$$S = -mc\int_a^b ds$$
and the Lagrangian is 
$$
L = -mc^2 \sqrt{1-\frac{v^2}{c^2}}.
$$

## Energy and Momentum
!!! note "Def: Momentum of a particle"
	$$\mathbf{p} = \frac{\partial L}{\partial \mathbf{v}}$$

Using the Lagrangian of a free particle, we find
$$
\mathbf{p} = -mc^2 \frac{-2\mathbf{v}/c^2}{2\sqrt{1-v^2/c^2}} = \frac{m\mathbf{v}}{\sqrt{1-v^2/c^2}}.
$$

^9cc1a8

!!! note "Def: Force acting on the particle"
	$$\mathbf{F} = \frac{d\mathbf{p}}{dt}$$

!!! note "Def: Energy of the particle"
	$$\mathscr{E} = \mathbf{p}\cdot\mathbf{v} - L$$

Also using the Lagrangian of a free particle, we have
$$
\mathscr{E} = \frac{m\mathbf{v}}{\sqrt{1-v^2/c^2}}\cdot \mathbf{v} - \left(-mc^2 \sqrt{1-\frac{v^2}{c^2}}\right) = \frac{mc^2(1-v^2/c^2)+mv^2}{\sqrt{1-v^2/c^2}} = \frac{mc^2}{\sqrt{1-v^2/c^2}}.
$$

^2539ba

For small velocity, we have 
$$
\mathscr{E} \approx mc^2\left(1-\frac{1}{2}(-\frac{v^2}{c^2})\right)
= mc^2 + \frac{1}{2}mv^2
$$
!!! tip "This means the total energy is the kinetic energy plus the static energy."

Although we speak of a "particle", we haven't used the property that it is "elementary". Thus **the formulas are equally applicable to any composite body consisting of many particles**, where by $m$ we mean the total mass of the body, and by $v$ the velocity of its motion as a whole.
!!! attention
	$\sum{m_\alpha c^2} \neq mc^2$ for the energy $mc^2$ contains both the kinetic energy of the particles and their interaction energy.

Squaring the [[CTF#^2539ba|energy]] and the [[CTF#^9cc1a8|momentum]] we can get:
$$\frac{\mathscr{E}^2}{c^2} = \frac{m^2 c^2}{1-v^2/c^2} = \frac{m^2 (c^2-v^2) + v^2}{1-v^2/c^2} = m^2 c^2 + \frac{m^2 v^2}{1-v^2/c^2}
= p^2 + m^2 c^2.$$

^19c0ef

!!! note "Def: Hamiltonian function $\mathscr{H}$"
	The energy written in terms of the momentum, which in this case is $$\mathscr{H} = c\sqrt{p^2 + m^2 c^2}$$

Also, for low velocities, we have 
$$\mathscr{H} = c\sqrt{p^2 + m^2 c^2} \approx mc^2 + \frac{p^2}{2m}.$$
Comparing the energy and momentum of a free particle, we get
$$\mathbf{p} = \mathscr{E}\frac{\mathbf{v}}{c^2}.$$
For $v=c$, the relation becomes ${p}=\frac{\mathscr{E}}{c}$.

!!! FAQ "Why a particle with nonzero mass can't move with the velocity of light?"
	For $v=c$, the momentum and energy of the particle will become infinite.
	(*But particles with zero mass moving with the velocity of light can exist*.)

**We can write these formulas in 4-dimensional form.**

The interval is 
$$ds = \sqrt{dx_i dx^i}$$
so the variation of the $ds$ is
$$\delta(ds) = \frac{ds}{dx^i} \delta(dx^i) = \frac{dx_i + \delta_{ij}dx^j}{2ds}\delta(dx^i) = \frac{dx_i}{ds}\delta(dx^i).$$

According to the principle of least action, $\delta S$ must be zero. So we have
$$\delta S = -mc\,\delta\int_{a}^{b}\sqrt{dx_i dx^i} = -mc\int_{a}^{b}\frac{dx_i}{ds}\delta(dx^i) = -mc\int_{a}^{b}u_{i}d\delta x^i = 0$$
$$\Rightarrow \delta S = -mcu_i \delta x^i\Big{|}_a^b + mc\int_a^b \delta x^i \frac{du_i}{ds}ds = 0$$
$$\Rightarrow \frac{du_i}{ds} = 0$$
This means the 4-dimensional velocity of a free particle remains constant.

To write the variation of action as a function of the coordinates, we keep point $a$ fixed and make point $b$ the variable, which can just move in the trajectories determined by equation $\frac{du_i}{ds} = 0$ so the second part of $\delta S$ is always zero. And there is no harm to let $(\delta x^i)_a$ be zero. In this case, we finally get the variation of action as a function of coordinates:
$$\delta S = -mcu_i\delta x^i.$$
The 4-vector 
$$p_i = -\frac{\partial S}{\partial x^i}$$
is called **momentum 4-vector (4-momentum)**. Because we have $\partial S/\partial x = p_x$ and $-\partial S/ \partial t = \mathscr{E}$, the components 4-momentum are 
$$p_i = (\mathscr{E}/c, -\mathbf{p}),$$
and the covariant components are
$$p^i = (\mathscr{E}/c, \mathbf{p}).$$

From $\delta S = -mcu_i\delta x^i$ and $p_i = -\frac{\partial S}{\partial x^i}$, we can see
$$p^i = mcu^i.$$
Once we get the 4-velocity of the free particle, we can instantly write down its energy and 3-momentum. And we now get the transformation formulas of energy and 3-momentum, which are directly given by the 4-vector transformation formulas:
$$p_x = \gamma(p_x'+\beta \frac{\mathscr{E'}}{c}), \quad p_y = p_y', \quad p_z = p_z', \quad \frac{\mathscr{E}}{c} = \gamma(\frac{\mathscr{E}'}{c}+\beta p_x')$$
where
$$\beta = \frac{V}{c},\quad \gamma = \frac{1}{\sqrt{1-\beta^2}}.$$

Using the identity of $u_iu^i = 1$, we have $p_ip^i = m^2c^2$. This is the same as the [[CTF#^19c0ef|energy-momentum relation]]. 

By analogy with the usual definition of the force, the **force four-vector** is defined as the derivative:
$$g^i = \frac{p^i}{ds} = mc \frac{du^i}{ds}.$$

!!! note "formulas in 4-dimensional form"
	- interval 
	 $$ds = \sqrt{dx_i dx^i}$$
	 $$\delta(ds) = \frac{ds}{dx^i} \delta(dx^i) = \frac{dx_i + \delta_{ij}dx^j}{2ds}\delta(dx^i) = \frac{dx_i}{ds}\delta(dx^i)$$
	- principle of least action 
	 $$\delta S = -mc\,\delta\int_{a}^{b}\sqrt{dx_i dx^i} = -mc\int_{a}^{b}\frac{dx_i}{ds}\delta(dx^i) = -mc\int_{a}^{b}u_{i}d\delta x^i = 0$$
	 $$\Rightarrow \delta S = -mcu_i \delta x^i\Big{|}_a^b + mc\int_a^b \delta x^i \frac{du_i}{ds}ds = 0$$
	 $$\Rightarrow \frac{du_i}{ds} = 0$$
	- the velocity of a free particle remains constant
	  $$\frac{du_i}{ds} = 0$$
	- 4-momentum
	  $$p_i = -\frac{\partial S}{\partial x^i} = (\frac{\mathscr{E}}{c}, -p_x, -p_y, -p_z)$$
	  $$p^i = (\frac{\mathscr{E}}{c}, p_x, p_y, p_z)$$
	- 4-dimensional energy-momentum relation
	  $$p_ip^i = m^2c^2$$
	- 4-dimensional force
	  $$g^i = \frac{p^i}{ds} = mc \frac{du^i}{ds}$$
	- relativistic Hamilton-Jacobi equation
	  $$g^{ij}\frac{\partial S}{\partial x^i}\frac{\partial S}{\partial x^j} = m^2c^2$$

## Transformation of Distribution Functions

!!! tip "Aim: Find the transformation law of distribution function $f(\mathbf{p})$."
	The $\mathbf{p}$ is a 3-vector and the *volume element* $dp_x dp_y dp_z$ is