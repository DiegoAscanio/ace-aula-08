## Impedância do Resistor — Dedução

<div class="footnotesize">

Pela lei de Ohm, se a corrente em um resistor variar senoidalmente com o tempo — isto é, se \\(i = I_{m} \cos(\omega t + \theta_{i})\\) —, a tensão nos terminais do resistor será:

\\[
\begin{align}
    v &= R \left[ I_{m} \cos(\omega t + \theta_{i}) \right] \\\\
      &= R I_{m} \left[ \cos(\omega t + \theta_{i}) \right] 
\end{align}
\\]

Onde \\(I_{m}\\) é a amplitude da corrente em apéres e \\(\theta_{i}\\) é o ângulo de fase da corrente. Podemos aplicar uma transformada fasorial em \\(v = R I_{m} \cos(\omega t + \theta_{i})\\) para obter um fasor 𝕀 para a corrente. Fazemos isso à partir do fato de que:

\\[
    v = R I_{m} \cos(\omega t + \theta_{i}) = I_{m} \Re \left[ e^{\theta_{i}} e^{j\omega t} \right] = \Re R \left[ I_{m} e^{\theta_{i}} e^{j \omega t} \right] 
\\]

E como sabemos, \\(𝕀 = I_{m} e^{\theta_{i}} = I_{m} \angle \theta_{i} \\), logo, \\(v = \Re R \left[ 𝕀 e^{j \omega t} \right] \\).

Como \\(e^{\omega t}\\) se cancela na solução da EDOs que descreve o circuito **(ver 4ª observação da pág. 346 do livro do NILSSON 10ª ed.)** , podemos escrever um fasor 𝕍 para a tensão a partir do fasor 𝕀 como:

\\[
    𝕍 = R 𝕀
\\]

</div>

<div class="footnotesize grid-50-50">

<div class="grid-element">

- A equação \\(𝕍 = R 𝕀\\) mostra que a tensão fasorial em um resistor é simplesmente a resistência multiplicada pela corrente fasorial.

</div>

<div class="grid-element">

- Ainda podemos deduzir que nos terminais de um resistor não existe nenhum deslocamento de fase entre a tensão e a corrente, pois, se \\(𝕍 = R 𝕀\\), \\(𝕍 = V_{m} \angle {\theta_{v}}\\) e \\(𝕀 = I_{m} \angle {\theta_{i}}\\), logo, \\(V_{m} \angle {\theta_{v}} = R I_{m} \angle {\theta_{i}}\\), então, \\(V_{m} = R I_{m}\\) e \\(\theta_{v} = \theta_{i}\\).

</div>

</div>
