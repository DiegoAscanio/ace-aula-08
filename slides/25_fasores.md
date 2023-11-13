## Transformada Fasorial — Verificação das Observações

<div class="grid-50-50 regular">

<div class="grid-element">

Em relação as observações contidas no slide anterior, utilizaremos o circuito RL tema desta aula para verificar as observações.

</div>

<div class="grid-element">

<!-- _class: transparent center -->
![](https://i.imgur.com/9fiWK0d.png)

</div>

</div>

<div class="regular">

Pelo fato de utilizarmos uma função cossenoidal para descrever o sinal senoidal da nossa fonte de tensão, então, usamos a equação \\(\cos(\theta) = ℜ \left\\{ e^{j\theta} \right\\}\\) para fazer a transformada fasorial necessária. A grandeza de interesse (pelo exemplo do livro) é a corrente de regime permanente do circuito \\(i_{rp}(t)\\) que também é descrita por uma função senoidal do tipo cosseno, por conveniência.

Considerando este fato, bem como que a amplitude da corrente é \\(I_{m}\\), logo, a representação fasorial da corrente de regime permanente é dada por:

\\[
    i_{rp} (t) = ℜ \left\\{I_{m} e^{j \beta} e^{j \omega t} \right\\}
\\]

Ou seja, \\(i_{rp}(t)\\) é dada pela parte real de \\(\left\\{I_{m} e^{j \beta} e^{j \omega t} \right\\}\\). Quando substituimos a corrente \\(i_{rp}(t)\\) pela sua representação fasorial na equação diferencial \\(L \frac{di(t)}{dt} + R i(t) = V_{m} \cos(\omega t + \phi) \\) que descreve o circuito RL, obtemos:

\\[
    ℜ \\left\\{(j \\omega L + R)I_{m} e^{j \beta} e^{j \omega t} \\right\\} + ℜ \\left\\{R I_{m} e^{j \beta} e^{j \omega t} \\right\\} = ℜ \\left\\{V_{m} e^{j \phi} e^{j \omega t} \\right\\} \\tag{8}
\\]

</div>
