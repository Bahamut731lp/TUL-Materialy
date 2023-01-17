**Určete Taylorův polynom druhého stupně se středem v bodě $[0,1]$ pro funkci $f(x,y)=e^{xy+x}+\text{arccotg}(2x) + \frac{sin(xy)}{y}$**

$$\large\begin{aligned}
T_2 &= f(x,y) + \frac{df(x,y)(x-x_0, y - y_0)}{1!} +
\frac{d^2f(x,y)(x-x_0, y - y_0)}{2!} = \\

&= f(0,1) + 
\left(\frac{\partial{f}}{\partial{x}}(0, 1)\cdot{x}+\frac{\partial{f}}{\partial{y}}(0, 1)\cdot{(y-1)}\right) \\
&+\left(\frac{\partial^2{f}}{\partial{x^2}}(0, 1)\cdot{x^2}+2\frac{\partial^2{f}}{\partial{xy}}(0, 1)\cdot{x \cdot (y-1)}+\frac{\partial^2{f}}{\partial{y^2}}(0, 1)\cdot{y^2}\right) \\

\end{aligned}$$



$$\Large\begin{aligned}
\frac{\partial{f}}{\partial{x}} &= e^{xy+x}\cdot(y+1) - \frac{1}{1+x^2}\cdot2+cos(xy)\\
\frac{\partial{f}}{\partial{y}} &= e^{xy+x}\cdot{x} \\


\end{aligned}
$$