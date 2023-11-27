## Impedância causada pela Indutância — Relação Tensão e Corrente em Um Indutor.

<div class="scriptsize grid-50-50">

<div class="grid-element solidmargin">

Considerando uma corrente \\(i = I_{m} \cos(\omega t + \theta_{i})\\) circulando em um indutor, a tensão \\(v\\) nos terminais do indutor é dada por:

\\[
\begin{align}
    v &= L \frac{di}{dt} = - \omega L I_{m} \sin(\sin \omega t + \theta_{i}) \therefore \\\\
    v &= - \omega L I_{m} \cos(\sin \omega t + \theta_{i} - 90°)
\end{align}
\\]

Considerando que na solução da equação que descreve a configuração indutiva o termo \\(e^{j \omega t}\\) é [cancelado](#38), a representação fasorial da tensão é dada por: 

\\[
\begin{align}
    𝕍 &= - \omega L I_{m} e^{\left(j \theta_{i} - 90° \right)} \therefore \\\\
      &= - \omega L I_{m} e^{j \theta_{i}} e^{-j 90°} \tag{1} \\\\
    e^{-j 90°} &= \cos(-90°) + j \sin(-90°) = -j \tag{2} \\\\
    \text{substituindo (2) em (1)} \\\\
    𝕍 &= j \omega L I_{m} e^{j \theta_{i}} \therefore \\\\
    𝕍 &= j \omega L 𝕀 \tag{3} \therefore \\\\
    \text{Onde } 𝕀 &= I_{m} e^{j \theta_{i}}, \text{ a representação fasorial da corrente } \\\\
\end{align}
\\]

<div class="grid-50-50">
<div class="grid-element">

Segundo a equação (3) o fasor tensão nos terminais de um indutor é igual a \\(j \omega L\\) vezes o fasor corrente, como ilustrado pela figura ao lado, que representa o circuito equivalente no domínio da frequência para um indutor:

</div>
<div class="grid-element">

<!-- _class: center transparent -->
![](https://i.imgur.com/gaD7rLA.png)

</div>
</div>


</div>

<div class="grid-element solidmargin">

Considerando na equação (3) que \\(\omega L j\\) é um número complexo expresso em coordenadas retangulares, podemos pela equação de Euler escrever:

\\[
\begin{align}
    \omega L e^{j \theta} = \omega L \left( \cos(\theta) + j \sin(\theta) \right) = \omega L j \tag{4}
\end{align}
\\]
A equação (4) é verdadeira se, e somente se, \\(\theta = 90°\\). Assim: 
\\[
\omega L j = \omega L e^{j 90°} = \omega L \angle 90° \tag{5}
\\]
Substituindo (5) em (4) temos que \\(𝕍 = \omega L \angle 90° 𝕀\\) e como \\(𝕀 = I_{m} e^{j \theta_{i}} = I_{m} \angle \theta_{i} \\), logo: 

\\[
𝕍 = \omega L \angle 90° \times I_{m} \angle \theta_{i} = \omega L I_{m} \angle (90° + \theta_{i}) \tag{6}
\\].

O que indica que a tensão e a corrente do indutor estão defasadas em exatamente 90°, ou seja, <span class="tooltip">que a tensão está adiantada 90° em relação à corrente,<span class="tooltiptext">Também podemos expressar o deslocamento de fase em segundos onde T/4 = 90°.</span></span> o que corresponde ao comportamento de um indutor, que se opõe a variações instantâneas de corrente, como mostrado pela figura abaixo:

<figure>

<!-- _class: center transparent -->
![reduced-img](https://i.imgur.com/E57neTY.png)

<figcaption class="tiny" style="text-align: center;">

Relação entre as fases da corrente e da tensão nos terminais de um indutor quando \\(\theta_{i} = 60°\\)

</figcaption>
</figure>


</div>

</div>

</div>
