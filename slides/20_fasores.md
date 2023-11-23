## Fasores — Representação de Uma Tensão Cossenoidal como um Fasor

<div class="footnotesize">

Como vimos, um fasor contém informações sobre a amplitude \\(r\\) e a fase de uma onda senoidal \\(\phi\\).

Considerando nossa tensão senoidal da forma cosseno de amplitude \\(r\\), frequência angular \\(\omega\\) e fase \\(\phi\\), pela identidade de euler, podemos escrevê-la como:

\\[
    V(t) = r \cos(\omega t + \phi) \equiv \Re\\{r e^{j(\omega t + \phi)}\\}.
\\]

Como do slide anterior sabemos que \\(\cos(\theta) = \Re\{e^{j\theta}\}\\), logo, descartamos a parte imaginária da exponencial complexa e ficamos apenas com sua parte real, representada por \\(\cos(\theta)\\).

Assim, podemos escrever \\(V(t)\\) como:

\\[
    V(t) = \Re\\{r e^{j(\omega t + \phi)}\\}. \\\\
    V(t) = \Re\\{r e^{j \phi} e^{j\omega t}\\}.
\\]

**\\(r e^{j \phi}\\) também por si próprio é um número complexo e também é um fasor, por conter as informações da amplitude \\(r\\) da tensão e da fase \\(\phi\\) da tensão cossenoidal.**

Assim, podemos chamar **\\(r e^{j \phi}\\) como o fasor \\(⨈ \\)** e portanto, a tensão \\(V(t)\\) pode ser escrita como:

\\[
    V(t) = \Re\\{⨈ e^{j\omega t}\\}.
\\]

Que significa que \\(V(t)\\) é a parte real da função complexa resultante da multiplicação do fasor ⨈  por \\(e^{j(\omega t)}\\) e como sabemos, esta parte real, ao final da multiplicação, é dada por \\(r \cos(\omega t + \phi)\\).

**Por conveniência das nossas resoluções, escolheremos sempre a parte real das nossas exponenciais complexas — funções cosseno — e, por isso, não abordaremos suas partes imaginárias. Entretanto, nem por isso estamos livres de lidar com funções senos, por isso, veremos mais a frente identidades trigonométricas que habilitam a conversão de funções senos para cossenos.**

</div>
