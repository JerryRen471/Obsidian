---
File: 
aliases: 
share: True
Title: The Classical Theory of Field
Type: Book
Status: Reading
Author: [Landau L.D., Lifshitz E.M.]
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

> [!TIP] As we can see in § 3, $\int_a^bds$ has a maximum along a straight line, so the constant $\alpha$ must be positive.

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
> [!note] Def: Momentum of a particle
> $$\mathbf{p} = \frac{\partial L}{\partial \mathbf{v}}$$

Using the Lagrangian of a free particle, we find
$$
\mathbf{p} = -mc^2 \frac{-2\mathbf{v}/c^2}{2\sqrt{1-v^2/c^2}} = \frac{m\mathbf{v}}{\sqrt{1-v^2/c^2}}.
$$

^9cc1a8

>[!note] Def: Force acting on the particle
>$$\mathbf{F} = \frac{d\mathbf{p}}{dt}$$

>[!note] Def: Energy of the particle
>$$\mathscr{E} = \mathbf{p}\cdot\mathbf{v} - L$$

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
>[!tip] This means the total energy is the kinetic energy plus the static energy.

Although we speak of a "particle", we haven't used the property that it is "elementary". Thus **the formulas are equally applicable to any composite body consisting of many particles**, where by $m$ we mean the total mass of the body, and by $v$ the velocity of its motion as a whole.
>[!attention]
>$\sum{m_\alpha c^2} \neq mc^2$ for the energy $mc^2$ contains both the kinetic energy of the particles and their interaction energy.

Squaring the [[CTF#^2539ba|energy]] and the [[CTF#^9cc1a8|momentum]] we can get:
$$
\frac{\mathscr{E}^2}{c^2} = \frac{m^2 c^2}{1-v^2/c^2} = \frac{m^2 (c^2-v^2) + v^2}{1-v^2/c^2} = m^2 c^2 + \frac{m^2 v^2}{1-v^2/c^2}
= p^2 + m^2 c^2.
$$

>[!note] Def: Hamiltonian function $\mathscr{H}$
>The energy written in terms of the momentum, which in this case is $$\mathscr{H} = c\sqrt{p^2 + m^2 c^2}$$

