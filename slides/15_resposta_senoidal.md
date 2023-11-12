## Resposta Senoidal

<div class="grid-50-50 regular">

<div class="grid-element">

Queremos mostrar através da dificuldade da obtenção da resposta senoidal pelos métodos tradicionais de resolução de EDOs a importância de se ter alternativas simplificadas que sejam capazes de resolver esse tipo de problema. No nosso caso, a representação fasorial.

Considere o circuito abaixo alimentado por uma tensão senoidal \\(v_{s} = V_{m} \cos(\omega t + \phi)\\).

<!-- _class: transparent center -->
![](https://i.imgur.com/9fiWK0d.png)

Por conveniência é considerado que \\(I(0) = 0\\) e o tempo só é contado a partir do instante em que a chave é fechada. Qual a função a resposta da corrente \\(i(t)\\) neste circuito RL?

</div>
<div class="grid-element">

Sabemos pela LKT nas malhas:

\\[
\begin{align}
v_{s} &= v_{R} + v_{L} \therefore \\\\
V_{m} \cos(\omega t + \phi) &= R i(t) + L \frac{di(t)}{dt} \therefore \\\\
L \frac{di(t)}{dt} + R i(t) &= V_{m} \cos(\omega t + \phi)
\end{align}
\\]

Não desenvolveremos a [solução da EDO](https://ava.cefetmg.br/mod/assign/view.php?id=107802), mas sim mostrar (e aceitar) que ela é dada por:

\\[
\begin{align}
    i(t) &= \frac{-V_{m}}{\sqrt{R^{2} + \omega^{2} L^{2}}} \cos(\phi - \theta) e^{-(\frac{R}{L}) t} \\\\
         &+ \frac{V_{m}}{\sqrt{R^{2} + \omega^{2} L^{2}}} \cos({\omega t + \phi - \theta}) \\\\
\end{align}
\\]

Onde \\(\theta\\) é o ângulo cuja tangente é \\(\frac{\omega L}{R}\\). Assim, se:
\\[
\begin{align}
    \tan{\theta} &= \frac{\omega L}{R} \therefore \\\\
    \theta &= \arctan{\frac{\omega L}{R}}
\end{align}
\\]

</div>

</div>
