## Operações Matemáticas com Números Complexos na Representação Fasorial

<div class="footnotesize">

### Multiplicação / Divisão

Consideremos dois fasores na forma retangular\\(𝕍_{1} = x_{1} + j y_{1} \text{ e } 𝕍_{2} = x_{2} + j y_{2}\\). A multiplicação (divisão) de números complexos é mais fácil de ser realizada quando estes números complexos encontram-se nas coordenadas polares (em notação angular). Portanto, para multiplicar (dividir) dois fasores na forma retangular é necessário convertê-los para a forma polar. 

**Se os fasores já estiverem representados em coordenadas polares, não é necessário convertê-los. Como não é o caso presente, vamos proceder a conversão.**

De acordo com o antepenúltimo slide, dois fasores estão na forma polar quando podem ser escritos como \\(𝕍 = r \angle \phi \\). Ainda de acordo com esse slide, \\(r = \sqrt{x^{2} + y^{2}}\\) e \\(\phi = {\tan}^{-1} \frac{y}{x}\\).

<div class="grid-50-50">

<div class="grid-element solidmargin">

Aplicando esta obtenção de \\(r\\) e \\(\phi\\) para \\(𝕍_{1}\\) e \\(𝕍_{2}\\) temos:

\\[
\begin{align}
    r_{1} &= \sqrt{{x_{1}}^2 + {y_{1}}^{2}} \\\\
    \phi_{1} &= {\tan}^{-1} \frac{y_{1}}{x_{1}} \therefore \\\\
    𝕍_{1} &= r_{1} \angle \phi_{1} \tag{5} \\\\
\end{align}
\\]

\\[
\begin{align}
    r_{2} &= \sqrt{{x_{2}}^2 + {y_{2}}^{2}} \\\\
    \phi_{2} &= {\tan}^{-1} \frac{y_{2}}{x_{2}} \therefore \\\\
    𝕍_{2} &= r_{2} \angle \phi_{2} \tag{6} \\\\
\end{align}
\\]

</div>

<div class="grid-element solidmargin">

Se quiseremos construir um \\(𝕍_{3}\\) a partir da multiplicação de \\(𝕍_{1}\\) e \\(𝕍_{2}\\) basta multiplicar as magnitudes das representações polares dos fasores \\(𝕍_{1}\\) e \\(𝕍_{2}\\) e somar seus ângulos de fases:

\\[
\begin{align}
    𝕍_{3} &= 𝕍_{1} * 𝕍_{2} \therefore  \\\\
    𝕍_{3} &= r_{1} r_{2} \angle \phi_{1} + \phi_{2}
\end{align}
\\]

E se \\(𝕍_{4}\\) for a divisão de \\(𝕍_{1}\\) e \\(𝕍_{2}\\):

\\[
\begin{align}
    𝕍_{4} &= \frac{𝕍_{1}}{𝕍_{2}} \therefore  \\\\
    𝕍_{4} &= \frac{r_{1}}{r_{2}} \angle \phi_{1} - \phi_{2}
\end{align}
\\]


</div>

</div>



</div>
