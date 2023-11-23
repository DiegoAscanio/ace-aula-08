## Fasores — Operações Matemáticas
### Integração e Derivação

<div class="regular">

Considerando nossa função senoidal de tensão \\(v(t) = V_{m} \cos(\omega t + \phi)\\), temos:

\\[
\begin{align}
    \frac{dv(t)}{dt} &= -\omega V_{m} \sin(\omega t + \phi) \\\\
    \int v(t) dt &= \frac{\sin{\omega t + \phi}}{\omega} + K
\end{align}
\\]

Na representação fasorial, podemos escrever \\(v(t) = ⨈ e^{j \omega t}\\), e assim:
Considerando apenas o fasor \\(⨈\\), temos:

\\[
\begin{align}
    \frac{d ⨈ e^{j \omega t}}{dt} &= j \omega ⨈ e^{j \omega t} \\\\
    \int{⨈ e^{j \omega t}} dt &= \frac{⨈ e^{j \omega t}}{j \omega} + K
\\]

Quando analisarmos as grandezas de interesse nos circuitos excitados por apenas uma fonte senoidal, podemos considerar apenas o fasor \\(⨈\\) e desprezar o termo \\(e^{j \omega t}\\), pois ele não afeta o valor da grandeza em questão.

</div>
