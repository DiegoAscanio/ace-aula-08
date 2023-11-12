## 1. Fonte senoidal - Características da Equação da Tensão

<div class="grid-50-50 scriptsize">

<div class="grid-element">

<figure class="center">

<div class="tiny">

<!-- _class: transparent center -->
![](https://i.imgur.com/wW8pzia.png)

<figcaption> Figura 3 - Deslocamento da onda senoidal ao longo do eixo do tempo quando <span>

 \\(\phi = 0\\) 

</span> </figcaption>

</div>

</figure>

Ainda observando a figura 3, as seguintes observações têm de ser feitas:

1. Definir \\(\phi = 0\\) na função \\(v = V_{m} \cos(\omega t + \phi)\\) desloca a onda \\(\frac{\phi}{\omega}\\) unidades de tempo para a direita.
2. Quando \\(\phi > 0\\), a onda senoidal desloca-se para a esquerda.
3. Quando \\(\phi < 0\\), a onda senoidal desloca-se para a direita.

</div>

<div class="grid-element">

4. \\(\phi\\) e \\(\omega t\\) devem ter as mesmas unidades, pois, são argumentos da função cossenoidal.
    1. Se \\(\omega t\\) for expressa em radianos (graus), espera-se que \\(\phi\\) também seja.
    2. Quando os dois ângulos forem expressos em unidades distintas, é necessário fazer a conversão de um deles para a unidade do outro, que pode ser realizada pela seguinte fórmula:
        - \\(\text{número de graus} = \frac{180°}{\pi} (\text{número de radianos})\\)

Retornando à função da tensão, expressa por \\(v = V_{m} \cos(\omega t + \phi)\\), outra característica de suma importância obtida de sua constituição é o seu **valor eficaz** ou **rms**, uma medida que representa a equivalência da tensão senoidal em termos de potência com uma tensão contínua. 

<!-- O Valor eficaz é útil porque possibilita calcular a potência dissipada por uma carga como se tal carga estivesse submetida a uma tensão contínua (facilitando o projeto de sistemas elétricos). -->

O valor eficaz é definido pela raiz quadrada do valor médido da função ao quadradado. Daí, se \\(f = V_{m} \cos({\omega t + \phi})\\), logo, \\(V_{rms}\\) é dado por:

\\[
\begin{align}
    V_{rms} &= \sqrt{\frac{1}{T + T_{0} - T_{0}} \int_{T_{0}}^{T + T_{0}}|f(t)|^{2} dt} \therefore \tag{2} \\\\
    V_{rms} &= \sqrt{\frac{1}{T} \int_{T_{0}}^{T + T_{0}}{{V_{m}}^{2}{\cos^{2}({\omega t + \phi})} dt}} \therefore \\\\
    V_{rms} &= \frac{V_{m}}{\sqrt{2}}
\end{align}
\\]

<!-- 
Com isso, verificamos que o valor eficaz de uma tensão senoidal depende somente da amplitude da tensão e não do ângulo de fase (ou da sua frequência)

Assim, qualquer sinal senoidal pode ser compleamente descrito se conhecermos sua frequência, seu ângulo de fase e sua amplitude (ou o valor máximo ou o valor eficaz)
-->

</div>

</div>
