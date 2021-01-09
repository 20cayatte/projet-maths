# Question 3
On suppose par l'absurde qu'il existe une solution 

$$
\begin{array}{ccccc}
x & : &  \mathbb{R} & \to & \mathbb{R}^2 \\ 
& & t & \longmapsto &  (x_{1},x_{2})
\end{array}
$$
initialisée dans $\mathbb{R}_{+}^{*} \times \, \mathbb{R}_{+}^{*}$
telle qu'il existe $t_{0}$ $\in$ $\mathbb{R}$ tq $x_{1}(t_{0})=0$ (ou  $x_{2}(t_{0})=0$ par symétrie  ) , alors la solution coïncide avec 
$$
\begin{array}{ccccc}
y & : &  \mathbb{R} & \to & \mathbb{R}^2 \\ 
& & t & \longmapsto &  (0,x_{2}(t_{0})e^{t-t_{0}} ) 
\end{array}
$$ 
au point $t_{0}$ . $y$ est également solution de l'équation de Lotka Volterra donc elles sont égales.  

En effet si deux solutions de l'équation de Lotka Volterra se coupent en un point elles sont égales par unicité de Cauchy Lipschitz. 


## question 4 
Soit 
$$
\begin{array}{ccccc}
H & : & \mathbb{R} \times \mathbb{R} & \to & \mathbb{R} \\ 
& & (x_{1},x_{2}) & \longmapsto &  \delta x_{1} - \gamma ln(x_{1}) + \beta x_{2} - \alpha ln(x_{2})
\end{array}
$$
$H$ est dérivable et $H'(t)= \delta \dot x_{1} - \frac{\gamma \dot x_{1}}{x_{1}} + \beta \dot x_{2} - \frac {\alpha \dot x_{2}}{x_{2}}$ 
$H'(t)= \delta x_{1}(\alpha-\beta x_{2}) - \gamma (\alpha-\beta x_{2}) - \beta (\gamma - \delta x_{1}) + \alpha  (\gamma - \delta x_{1})$ 
$H'(t)= \delta x_{1}\alpha-\delta x_{1}\beta x_{2} - \gamma \alpha- \gamma\beta x_{2} + \beta \gamma x_{2} - \beta\delta x_{1}x_{2} + \alpha  \gamma - \delta x_{1}\alpha$
$H'(t)=0$
donc $H$ est constante.
$$
$$
Soit une solution maximale 

$$
\begin{array}{ccccc}
x & : &  ]t_{m}^{-};t_{m}^{+}[ & \to & \mathbb{R}^2 \\ 
& & t & \longmapsto &  (x_{1},x_{2})
\end{array}
$$
initialisée dans $\mathbb{R}_{+}^{*} \times \, \mathbb{R}_{+}^{*}$

Pour montrer que la solution maximale est définie sur $\mathbb{R}$ on suppose par l'absurde que   par exemple $t_{m}^{+}$ est fini. 
$\;$ 
Alors d'après le théorème du domaine maximal d'existence on a $\lim\nolimits_{ t \to t_{m}^{+} }$ $d((t,x(t),\partial(\mathbb{R} \times \mathbb{R}_{+}^{*} \times \mathbb{R}_{+}^{*} ))$  $=$ $0$ ou bien $\lim\nolimits_{t \to t_{m}^{+}} \|x(t)\|$ $=$ $+\infty$
. 
Le premier cas n'est pas possible car si $x_{1}$ par exemple tend vers $0$ le $ln(x_{1})$ va diverger vers $+\infty$ et donc comme $\delta x_{1}  + \beta x_{2} - \alpha ln(x_{2})$ est minoré, $H$ tend vers $+\infty$ ce qui est absurde. 

Le second cas n'est pas non plus possible car si $\lim\nolimits_{t \to t_{m}^{+}} \|x(t)\|$ $=$ $+\infty$ cela veut dire que (par symétrie) $x_{1}$ tend vers $+\infty$ (car positif ) et donc comme  $ln(x_{1})=o(x_{1})$ et $\beta x_{2} - \alpha ln(x_{2})$ est minoré alors $H$ tend vers $+\infty$  ce qui est absurde.
$$
$$ 
En conclusion, la solution maximale est définie sur $\mathbb{R}$.


## question 9
Soit $x$ une solution de l'équation de Lotka Volterra. Comme pour un tel $x$ H est constant, on aura $H(x_{1},x_{2})-H_{0}=H(x_{1},x_{2})-H(x(0))=0$. Donc $x$ est également solution de ce système. 

Soit maintenant $x$ une solution du système. On pose $x(0)=x_{0}$ D'après le théorème d'existence  de Cauchy Lipschitz appliqué aux équations de Lotka Volterra avec pour condition initiale $x_{0}$, il existe une solution $y$. Celle ci est d'après le début de la question solution du nouveau système. Donc $x$ et $y$ sont solutions du système avec la même condition initiale, par le théorème d'unicité de Cauchy Lispchitz elles sont égales. Donc $x$ est solution de Lotka Volterra.

Ainsi les solutions de Lotka Volterra sont exactement les solutions pour tout choix de
 $$
\begin{array}{ccccc}
u & : &  \mathbb{R}^2 & \to & \mathbb{R}^2 \\ 
\end{array}
$$


## question 10 
$H((x(t))-H_0= \delta x_1-\gamma ln(x_1) + \beta x_2 - \alpha ln(x_2)-H_0$

$\frac{d(H(x(t)-H_0)}{dt}= \delta \dot x_{1} - \frac{\gamma \dot x_{1}}{x_{1}} + \beta \dot x_{2} - \frac {\alpha \dot x_{2}}{x_{2}}
$ 



$\frac{d(H(x(t)-H_0)}{dt}= \frac{ \dot x_{1}}{x_{1}}(\delta x_1 -\gamma)+ \frac{ \dot x_{2}}{x_{2}}(\beta x_2 - \alpha)$


$\frac{d(H(x(t)-H_0)}{dt}= (\alpha - \beta x_2) (\delta x_1 - \gamma) -  (\gamma - \delta x_1) (\beta x_2 - \alpha) - (u_1(x_1,x_2) \frac {\delta x_1 - \gamma}{x_1} + u_2(x_1,x_2) \frac {\beta x_2 - \alpha}{x_2}) (H(x(t)-H_0)$

$\frac{d(H(x(t)-H_0)}{dt}=0 -  (u_1(x_1,x_2) \frac {\delta x_1 - \gamma}{x_1} + u_2(x_1,x_2) \frac {\beta x_2 - \alpha}{x_2}) (H(x(t)-H_0)$


On calcule 
$$ \nabla H(x_1,x_2)=
\begin{pmatrix}
\delta - \frac{\gamma}{x_1} \\

 \beta - \alpha/{x_2}
\end{pmatrix}
$$ 

$$ \nabla H(x_1,x_2)=
\begin{pmatrix}
 \frac{\delta x_1 -\gamma}{x_1} \\

  (\beta x_2 -\alpha)/{x_2}
\end{pmatrix}
$$ 

On choisit $u(t)= k \times \nabla H(x(t))$

Alors $\frac{d(H(x(t)-H_0)}{dt}= - k\|\nabla H(x(t))\|^2 \times (H(x(t)-H_0)$
