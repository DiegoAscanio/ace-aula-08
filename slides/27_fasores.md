## Transformada Fasorial — Verificação das Observações

<div class="regular">

Porque escolhemos a função cosseno para ser nossa representação senoidal é que extraimos a parte real da função exponencial. Se tivéssemos escolhido a função seno para analisar o regime permanente senoidal, teríamos extraído a parte imaginária da função exponencial (pela notação fasorial) que preconiza que \\(\sin(\theta) = ℑ \\left\\{ e^{j \theta} \\right\\} \\). Portanto, se considerássemos a representação senoidal da corrente do regime permanente como uma função seno, nossa equação para o estado estacionário neste regime seria:

\\[
ℑ \\left\\{ (j \omega L + R) I_{m} e^{j \beta} e^{j \omega t} \\right\\} = ℑ \\left\\{ V_{m} e^{j \phi} e^{j \omega t} \\right\\} \tag{9}
\\]

Retomando agora a equação 8:

\\[
    ℜ \\left\\{(j \\omega L + R)I_{m} e^{j \beta} e^{j \omega t} \\right\\} + ℜ \\left\\{R I_{m} e^{j \beta} e^{j \omega t} \\right\\} = ℜ \\left\\{V_{m} e^{j \phi} e^{j \omega t} \\right\\} \\tag{8}
\\]

Observe que as partes complexas e reais das equações 8 e 9 são iguais. Portanto,

\\[
    (j \omega L + R)I_{m} e^{j \beta} = V_{m} e^{j \phi} \\therefore \\\\
    I_{m} e^{j \beta} = \\frac{V_{m} e^{j \phi}}{R + j \omega L} \\tag{10}
\\]

</div>


