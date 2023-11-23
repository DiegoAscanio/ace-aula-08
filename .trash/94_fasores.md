## O Conceito de Fasor - Transformada Fasorial Inversa

<div class="regular">

\\[
Ƒ^{-1} \\{ V_{m} e^{j \phi} \\} = ℜ  \left\\{ V_{m} e^{j \phi} e^{j \omega t} \right\\} \tag{7}
\\]

Estudando a equação 7, o termo a esquerda, \\(Ƒ^{-1} \\{ V_{m} e^{j \phi} \\}\\), representa a própria **transformada fasorial inversa** e o termo a direita, \\(ℜ  \left\\{ V_{m} e^{j \phi} e^{j \omega t} \right\\}\\) , indica como devemos obter a transformada fasorial a inversa, ou seja, devemos multiplicar o fasor \\(V_{m} e^{j \phi}\\) por \\(e^{j \omega t}\\) e, então, extrair a parte real do resultado.

Reiterando, a transformada fasorial é valiosa porque permite determinar a amplitude máxima e o ângulo de fase da resposta permanente senoidal pela álgebra de números complexos. As seguintes observações corroboram este fato:

</div>

<div class="regular grid-50-50" style="border: solid 2px #663399;">

<div class="grid-element">

1. A componente transitória da resposta senoidal se extingue à medida que o tempo passa. Portanto, quando \\(t \rightarrow \infty\\), a componente permanente é quem satisfaz a equação diferencial que descreve o sistema.
2. Em um circuito linear estimulado por fontes senoidais, a resposta permanente também é senoidal com a mesma frequência da fonte.

</div>

<div class="grid-element">

3. Usando a notação para \\(\cos(\theta) = ℜ \left\\{ e^{j \theta} \right\\}\\) é possível propor \\(ℜ \left\\{ A e^{j \beta} e^{j \omega t} \right\\}\\) como solução para o regime permanente do sistema, onde \\(A\\) é a amplitude máxima da resposta e \\(\beta\\) seu ângulo de fase.
4. Quando substituímos a solução de regime permanente proposta na EDO do sistema, o termo exponencial \\(e^{j \omega t}\\) se cancela, deixando a solução para \\(A\\) e \\(\beta\\) no domínio dos números complexos.

</div>

</div>
