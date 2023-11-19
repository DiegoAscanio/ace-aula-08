## O Conceito de Fasor - Transformada Fasorial

<div class="grid-50-50 regular">

<div class="grid-element">

Continuemos nossa análise pela equação 3:

\\[
\begin{align}
    v_{s}(t) &= ℜ\\\{V_{m} e^{j\phi} e^{j\omega t}\\} \tag{3}
\end{align}
\\]

A quantidade \\(V_{m} e^{j \phi}\\) é um número complexo que contém informações sobre a amplitude e o ângulo de fase da tensão senoidal \\(V_{m} \cos(\omega t + \phi)\\). Este número complexo \\(V_{m} e^{j \phi}\\) é, por definição, a **representação do fasor** (ou, **transformada fasorial**) da função senoidal dada.

Assim, o fasor **V** é definido como:

\\[
\\begin{align}
    \\mathbf{V} &= V_{m} e^{j \\phi} = Ƒ \left\\{ V_{m} \\cos(\\omega t + \\phi) \right\\} \tag{4}
\\end{align}
\\]

Onde a notação \\(Ƒ \left\\{ V_{m} \\cos(\\omega t + \\phi) \right\\}\\) é lida como **"a transformada fasorial de \\(V_{m} \\cos(\\omega t + \\phi)\\)"**.

</div>
<div class="grid-element">

Preste bastante atenção neste conceito de **transformada fasorial**, pois, tal conceito é fundamental para a análise de circuitos em regime permanente senoidal.

O que de fato significa uma transformada fasorial? É uma função de transformação que converte funções representadas no domínio do tempo (**real**) para o domínio dos números complexos, também conhecido como **domínio da frequência**.

Como diferenciar uma variável representada no domínio do tempo de outra representada no domínio da frequência? 
- Por convenção adotamos a notação de variáveis (fasores) no domínio da frequência em negrito, como por exemplo, **V** na equação 4 e as variáveis no domínio do tempo não utilizamos destaques em seus nomes.

Por que a transformada fasorial é importante? Porque, como veremos a seguir, ela permite reduzir a análise de circuitos em regime permanente senoidal a simples operações algébricas de números complexos.

</div>

</div>
