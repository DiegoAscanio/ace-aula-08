## Operações Matemáticas com Números Complexos na Representação Fasorial

<div class="small">

### Adição (Subtração)

Consideremos dois fasores na forma polar (exponencial) \\(𝕍_{1} = r_{1} e^{j \theta_{1}} \text{ e } 𝕍_{2} = r_{2} e^{j \theta_{2}}\\). A soma (subtração) de números complexos é mais fácil de ser realizada quando estes números complexos encontram-se nas coordenadas retangulares. Portanto, para somar (subtrair) dois fasores na forma polar (exponencial) é necessário convertê-los para a forma retangular. 

**Se os fasores já estiverem representados em coordenadas cartesianas, não é necessário convertê-los. Como não é o caso presente, vamos proceder a conversão.**

De acordo com o penúltimo slide, dois fasores estão na forma retangular quando podem ser escritos como \\(𝕍 = x + jy\\). Ainda de acordo com esse slide, \\(x = r \cos \theta\\) e \\(y = r \sin \theta\\). 

<div class="grid-50-50">

<div class="grid-element solidmargin">

Aplicando esta obtenção de \\(x\\) e \\(y\\) para \\(𝕍_{1}\\) e \\(𝕍_{2}\\) temos:

\\[
\begin{align}
    x_{1} &= r_{1} \cos \theta_{1} \\\\
    y_{1} &= r_{1} \sin \theta_{1} \therefore \\\\
    𝕍_{1} &= x_{1} + j y_{1} \tag{1} \\\\
\end{align}
\\]

\\[
\begin{align}
    x_{2} &= r_{2} \cos \theta_{2} \\\\
    y_{2} &= r_{2} \sin \theta_{2} \therefore \\\\
    𝕍_{2} &= x_{2} + j y_{2} \tag{2} 
\end{align}
\\]

</div>

<div class="grid-element solidmargin">

Se quiseremos construir um \\(𝕍_{3}\\) a partir da soma de \\(𝕍_{1}\\) e \\(𝕍_{2}\\) basta somar os termos reais e imaginários de \\(𝕍_{1}\\) e \\(𝕍_{2}\\) separadamente, como abaixo:

\\[
\begin{align}
    𝕍_{3} &= 𝕍_{1} + 𝕍_{2} = (x_{1} + j y_{1}) + (x_{2} + j y_{2}) \\\\
    𝕍_{3} &= (x_{1} + x_{2}) + j (y_{1} + y_{2}) \tag{3}
\end{align}
\\]

E se \\(𝕍_{4}\\) for a subtração de \\(𝕍_{1}\\) e \\(𝕍_{2}\\):

\\[
\begin{align}
    𝕍_{4} &= 𝕍_{1} - 𝕍_{2} = (x_{1} + j y_{1}) - (x_{2} + j y_{2}) \\\\
    𝕍_{4} &= (x_{1} - x_{2}) + j (y_{1} - y_{2}) \tag{4}
\end{align}
\\]


</div>

</div>



</div>
