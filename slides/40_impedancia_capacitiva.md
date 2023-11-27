## Impedância causada pela Capacitância — Relação Tensão e Corrente em Um Capacitor.

<div class="scriptsize grid-50-50">

<div class="grid-element">

Obtemos a relação entre os fasores de tensão e corrente nos terminais de um capacitor de maneira semelhante ao que fizemos para o indutor.

Sabemos que a corrente de um capacitor é dada por \\(i = C \frac{dv}{dt}\\). Ao admitirmos que o nosso circuito é estimulado por uma fonte de tensão cossenoidal da forma \\(v = V_{m} \cos(\omega t + \theta_{v})\\), por conveniência das ferramentas matemáticas dos números complexos, adotamos a representação fasorial da tensão para calcular sua derivada e obter a corrente, também em sua notação fasorial, por assim termos aplicado para a tensão.

Ao considerarmos a representação fasorial 𝕍 para a tensão, temos que \\(\frac{dv}{dt} = j \omega 𝕍\\). Portanto:

\\[
𝕀 = j \omega C 𝕍 \\\\
\text{E a representação da tensão em função da corrente é dada por:} \\\\
𝕍 = \frac{1}{j \omega C} 𝕀 \tag{7}
\\]

<div class="grid-66-33">

<div class="grid-element">

A equação (7) é a relação entre o fasor tensão e o fasor corrente em um capacitor, que possui um circuito equivalente no domínio da frequência como mostrado ao lado: 

</div>

<div class="grid-element">

<!-- _class: transparent center -->
![](https://i.imgur.com/i5dv5z9.png)

</div>

</div>

</div>

<div class="grid-element">

Considere o número complexo \\(\frac{1}{j \omega C}\\) que já está expresso em coordenadas retangulares. Ele também pode ser reescrito como \\(\frac{1}{\omega C} \cdot \frac{1}{j}\\).

Considere agora apenas \\(\frac{1}{j}\\). Multipliquemos este número por 1, na forma de \\(\frac{j}{j}\\). Assim:

\\[
\frac{1}{j} = \frac{j}{j} \cdot \frac{1}{j} = \frac{j}{j^2} = \frac{j}{-1} = -j
\\]

Logo, \\(\frac{1}{j} = -j\\), pois, \\(j^{2} = -1\\). Portanto, \\(\frac{1}{j \omega C} = - \frac{j}{\omega C}\\). Com isso, podemos escrever \\(\frac{1}{j \omega C}\\) como \\(- \frac{j}{\omega C}\\).

Vamos agora expressar este número em coordenadas polares, para isso, devemos encontrar um angulo \\(\theta \text{ tal que } \frac{1}{\omega C} e^{j \theta} = \frac{1}{\omega C}\left( \cos(\theta) + j \sin(\theta) \right) = -j \omega C \\). Esta equação só pode ser satisfeita quando \\(\theta = - \frac{\pi}{2} = -90°\\). Logo, a forma exponencial de \\(- \frac{j}{\omega C}\\) é \\(\frac{1}{\omega C} e^{(j - 90°)}\\) e sua forma polar: \\(\frac{1}{\omega C} \angle -90°\\).

Considerando que na equação \\(𝕍 = \frac{1}{j \omega C} 𝕀\\), que a representação polar de \\(\frac{1}{j \omega C}\\) é \\(\frac{1}{\omega C} \angle -90°\\) e a representação fasorial da corrente \\(𝕀\\) é \\(I_{m} \angle \theta_{i}°\\), podemos representar a tensão \\(𝕍\\) como uma multiplicação de números complexos em suas formas polares tal como:

\\[
\begin{align}
𝕍 &= \frac{1}{\omega C} \angle -90° \cdot I_{m} \angle \theta_{i}° \therefore \\\\
𝕍 &= \frac{I_{m}}{\omega C} \angle (\theta_{i} - 90°) \tag{8}
\end{align}
\\]

</div>

</div>
