<style>
  section {
    background: #fff url(./img/background.png) no-repeat center center;
    background-size: cover;
  }

  section.center img {
    display: block;
    margin: auto;
  }

  img[alt=small-img] {
    display: block;
    margin: auto;
    width: 30%;
  }

  .transparent {
    background-color: transparent!important;
  }

  section.transparent img {
    background-color: transparent!important;
  }

  section.ttable table {
    margin: auto;
  }

  .cabecalho {
    position: absolute;
    top: 10%;
    margin-left: 5%;
    margin-right: 10%;
    font-size: 48px;
    font-weight: bold;
  }

  .conteudo {
    top: 30%;
    margin-left: 5%;
    margin-right: 10%;
    font-size: 28px;
    text-align: justify;
  }

  .conteudo-absoluto {
    position: absolute;
    top: 30%;
    margin-left: 5%;
    margin-right: 10%;
    font-size: 28px;
    text-align: justify;
  }
  
  .large {
    font-size: 36px;
  }

  .normal {
    font-size: 22px;
  }
  .regular {
    font-size: 18px;
  }
  .small {
    font-size: 16px;
  }
  .footnotesize {
    font-size: 14px;
  }
  .scriptsize {
    font-size: 12px;
  }
  .tiny {
    font-size: 10px;
  }
  .bold {
    font-weight: bold;
  }
  .center {
    text-align: center;
  }
  section.lead p {
    text-align: justify;
  }
  section.lead h1 {
    text-align: center;
  }
  section.lead h2 {
    text-align: center;
  }
  section.lead h3 {
    text-align: center;
  }
  section.lead h4 {
    text-align: center;
  }

  
  .grid-50-50 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    text-align: justify;
  }

  .grid-25-25-25-25 {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    text-align: justify;
  }

  .grid-33-33-33 {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    text-align: justify;
  }


  .grid-66-33 {
    display: grid;
    grid-template-columns: 2fr 1fr;
    text-align: justify;
  }

  .grid-33-66 {
    display: grid;
    grid-template-columns: 1fr 2fr;
    text-align: justify;
  }

  .grid-element {
    margin-left: 5%;
    margin-right: 5%;
  }
  img[alt=grid-img] {
    width: 100%;
  }
  img[alt=slide-img] {
    width: 75%;
  }

  .dashedmargin {
    border-style: dashed;
  }

  .solidmargin {
    padding: 9px;
    border-style: solid;
  }


</style>

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>


# Análise de Circuitos Elétricos
## Aula 08 - Análise do Regime Permanente Senoidal
 
Prof. M.Sc. Diego Ascânio Santos (ascanio@cefetmg.br)

Aula baseada sobre o material do professor Dr. Emerson Gonçalves de Melo (emerdemelo@usp.br - DEMAR EEL USP), da professora Drª. Thabatta Moreira Alves de Araújo (thabatta@cefetmg.br - DIGDDV), da Khan Academy e da bibliografia padrão da disciplina.

CEFET-MG DIGDDV - Divinópolis, 2023.


---

## Roteiro

1. Fonte senoidal. 
2. Resposta senoidal.
3. O conceito de Fasor.
4. Elementos passivos no domínio da frequência.
5. As leis de Kirchhoff no domínio da frequência.
6. Associações em série e em paralelo e transformações \\(\Delta\\) - Y.
7. Equivalentes de Thévenin e de Norton.
<!--
8. Transformadores.
9. Diagramas fasoriais.
-->


---

## Objetivos

<div class="normal">

1. Entender o conceito de fasor e saber realizar uma transformada fasorial e a transformada inversa.
2. Saber transformar um circuito alimentado por uma fonte senoidal para o domínio da frequência através do conceito de fasor.
3. Saber aplicar as seguintes técnicas de análise de circuitos no domínio da frequência:
    1. Leis de Kirchhoff.
    2. Associação de elementos em série, paralelo e transformação delta-estrela.
    3. Divisão de tensão e corrente.
    4. Equivalentes de Thévenin e Norton.
4. Saber analisar circuitos que contenham transformadores lineares usando métodos fasoriais.
5. Entender as relações terminais do transformador ideal e saber analisar circuitos que contenham transformadores ideiais usando métodos fasoriais.

</div>


---

## Contextualização

Até o momento trabalhamos apenas com circuitos contínuos alimentados por fontes de tensão ou de corrente.

Agora, vamos estudar circuitos energizados por fontes de tensão (ou corrente) que variem com o tempo — também conhecidos como **circuitos de corrente alternada (CA)**.

As fontes objetos do nosso estudo são aquelas que fornecem tensões / correntes que variam de forma senoidal em relação ao tempo.


---

## Contextualização

<div class="normal">

Por que é importante estudarmos correntes alternadas?

- Geração, transmissão, distribuição e consumo de energia elétrica nas aplicações cotidianas — energia elétrica industrial, comercial, residencial — acontecem em condições de regime permanente (tensões e correntes) caracterizadas por funções senoidais alternadas, que variam com o tempo.

- O entendimento do regime senoidal possibilita a previsão do comportamento de sistemas com fontes não senoidais (transformadas de Fourier permitem aproximar quaisquer funções em termos de senoides).

- O regime senoidal simplifica o projeto de sistemas elétricos — um projetista de sistemas elétricos pode formular seus circuitos em termos de uma resposta de um regime permanente senoidal desejável e projetar os circuitos para satisfazer tais características. Se os projetos funcionarem no regime permanente senoidal, eles funcionarão em qualquer regime.

</div>


---

## Aplicação prática do regime permanente senoidal
### Circuito de distribuição residencial de energia elétrica

<div class="grid-50-50">

<div class="grid-element regular">

</div>

<div class="grid-element regular">

</div>


</div>


---

<!-- _class: lead -->
# 1. Fonte senoidal


---

## 1. Fonte senoidal

<div class="grid-50-50 regular">

<div class="grid-element">

Uma fonte de tensão (corrente) senoidal gera uma tensão (corrente) que oscila em um padrão senoidal com o tempo.

<div class="footnotesize">

As análises que realizaremos são inicialmente focadas para fontes de tensão seinoidais, porém, suas conclusões são igualmente estendidas para fontes de corrente senoidais.

</div>

- Funções que variam senoidalmente podem ser expressas por meio de senos ou cossenos.
- Ambas funcionam bem, mas, não podem ser utilizadas ao mesmo tempo.
- Em nossas análises será utilizada a função cosseno e, consequentemente, a fonte de tensão senoidal será expressa por:

\\[
    v = V_{m} \cos({\omega t + \phi})
\\]

- O gráfico desta função é representado pela figura 2.

</div>

<div class="grid-element">

<figure>

<!-- _class: transparent center -->
![grid-img](https://i.imgur.com/aqyAWJd.png)

<div class="footnotesize center">

<figcaption>

Figura 2 - Gráfico da função \\(v = V_{m} \cos({\omega t + \phi})\\)

</figcaption>

</div>

</figure>

</div>

</div>


---

## 1. Fonte senoidal

<div class="grid-50-50 regular">

<div class="grid-element">

Analisando a figura 2, podemos perceber que a função senoidal repete-se por intervalos regulares. Esta característica representa a periodiciade da função senoidal e por isso, esta função também é denominada periódica.

Para os objetivos de nosso estudo, é importante entendermos o intervalo de tempo que a função senoidal leva para atingir todos os seus valores possíveis e, então, começar uma nova repetição destes valores. Este intervalo é denominado período e é representado pela letra <span class="big"> **\\(T\\)** </span>, sendo medido em segundos.

A grandeza recíproca (inversa) a \\(T\\) é denominada frequência e é representada pela letra <span class="big"> **\\(f\\)** </span>, sendo medida em Hertz (Hz). A frequência representa a quantidade de vezes (número de ciclos) por segundo que a função senoidal se repete.

\\[
f = \frac{1}{T}
\\]

</div>

<div class="grid-element">

<figure>

<!-- _class: transparent center -->
![grid-img](https://i.imgur.com/aqyAWJd.png)

<div class="footnotesize center">

<figcaption>

Figura 2 - Gráfico da função \\(v = V_{m} \cos({\omega t + \phi})\\)

</figcaption>

</div>

</figure>

</div>

</div>


---

## 1. Fonte senoidal - Características da Equação da Tensão

<div class="grid-50-50 regular">

<div class="grid-element">

Consideremos novamente a equação que descreve a tensão:

\\[
    v = V_{m} \cos({\omega t + \phi})
\\]

O coeficiente \\(\omega\\) de \\(t\\) contém necessariamente o valor numérico de \\(f\\) — \\(\frac{1}{T}\\) — e é chamado de **frequência angular** da função senoidal, sendo expresso por:

\\[
    \omega = 2 \pi f = \frac{2 \pi}{T} (\frac{\text{radianos}}{\text{segundo}}) \tag{1}
\\]

A cada vez que a função cosseno (ou seno) passa por um conjunto completo de seus valores, seu argumento \\(\omega t \\) percorre \\(2 \pi\\) rad \\((360 °)\\) e é este fato que embasa a definição de frequência angular (na equação 1).

Podemos concluir também que todas as vezes que \\(t\\) for um múltiplo de \\(T\\), \\(\omega t\\) será múltiplo inteiro de \\(2 \pi\\) rad.

</div>

<div class="grid-element">

O coeficiente \\(V_{m}\\) é a **amplitude máxima** da tensão senoidal. Como \\(\pm 1\\) são os valores extremos do cosseno, \\(\pm V_{m}\\) limita a amplitude da tensão senoidal.

O ângulo \\(\phi\\) da equação que descreve a tensão é chamado de **ângulo de fase** da tensão senoidal. Ele determina o valor da função senoidal no instante \\(t = 0\\); portanto, fixa o ponto da onda periódica em que começamos a medir o tempo. A alteração do ângulo de fase \\(\phi\\) provoca um deslocamento da onda senoidal ao longo do eixo do tempo, mas, não exerce nenhum efeito sobre a amplitude \\(V_{m}\\) ou sobre a frequência angular \\(\omega\\), como mostra a figura 3:

<figure class="center">

<div class="tiny">

<!-- _class: transparent center -->
![](https://i.imgur.com/wW8pzia.png)

<figcaption> Figura 3 - Deslocamento da onda senoidal ao longo do eixo do tempo quando <span>

 \\(\phi = 0\\) 

</span> </figcaption>

</div>

</figure>

</div>

</div>


---

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


---

<!-- _class: lead -->

# Exemplos de fontes senoidais 9.1, 9.2, 9.3 e 9.4


---

## Exemplos 9.1, 9.2, 9.3 e 9.4 (NILSSON; RIEDEL 10ª Ed)

<iframe src="https://diegoascanio.github.io/jupyterlite/lab?path=exemplos_9.1_9.2_9.3_9.4.ipynb" width=100% height=100%></iframe> 


---

<!-- _class: lead -->
# Resposta Senoidal


---

## Resposta Senoidal

<div class="grid-50-50 regular">

<div class="grid-element">

Queremos mostrar através da dificuldade da obtenção da resposta senoidal pelos métodos tradicionais de resolução de EDOs a importância de se ter alternativas simplificadas que sejam capazes de resolver esse tipo de problema. No nosso caso, a representação fasorial.

Considere o circuito abaixo alimentado por uma tensão senoidal \\(v_{s} = V_{m} \cos(\omega t + \phi)\\).

<!-- _class: transparent center -->
![](https://i.imgur.com/9fiWK0d.png)

Por conveniência é considerado que \\(I(0) = 0\\) e o tempo só é contado a partir do instante em que a chave é fechada. Qual a função a resposta da corrente \\(i(t)\\) neste circuito RL?

</div>
<div class="grid-element">

Sabemos pela LKT nas malhas:

\\[
\begin{align}
v_{s} &= v_{R} + v_{L} \therefore \\\\
V_{m} \cos(\omega t + \phi) &= R i(t) + L \frac{di(t)}{dt} \therefore \\\\
L \frac{di(t)}{dt} + R i(t) &= V_{m} \cos(\omega t + \phi)
\end{align}
\\]

Não desenvolveremos a [solução da EDO](https://ava.cefetmg.br/mod/assign/view.php?id=107802), mas sim mostrar (e aceitar) que ela é dada por:

\\[
\begin{align}
    i(t) &= \frac{-V_{m}}{\sqrt{R^{2} + \omega^{2} L^{2}}} \cos(\phi - \theta) e^{-(\frac{R}{L}) t} \\\\
         &+ \frac{V_{m}}{\sqrt{R^{2} + \omega^{2} L^{2}}} \cos({\omega t + \phi - \theta}) \\\\
\end{align}
\\]

Onde \\(\theta\\) é o ângulo cuja tangente é \\(\frac{\omega L}{R}\\). Assim, se:
\\[
\begin{align}
    \tan{\theta} &= \frac{\omega L}{R} \therefore \\\\
    \theta &= \arctan{\frac{\omega L}{R}}
\end{align}
\\]

</div>

</div>


---

## Resposta Senoidal

<div class="small">

As seguintes observações a respeito da corrente \\(i(t) = \frac{-V_{m}}{\sqrt{R^{2} + \omega^{2} L^{2}}} \cos(\phi - \theta) e^{-(\frac{R}{L}) t} + \frac{V_{m}}{\sqrt{R^{2} + \omega^{2} L^{2}}} \cos({\omega t + \phi - \theta})\\) têm de ser efetuadas:

1. A expressão \\(\frac{-V_{m}}{\sqrt{R^{2} + \omega^{2} L^{2}}} \cos(\phi - \theta) e^{-(\frac{R}{L}) t}\\) é denominada **componente transitória** da corrente, pois ela se torna infinitesimal (tende à zero) quando \\(t \rightarrow \infty\\).
2. Já a segunda expressão \\(\frac{V_{m}}{\sqrt{R^{2} + \omega^{2} L^{2}}} \cos({\omega t + \phi - \theta})\\) é denominada **componente do regime permanente** da corrente e existirá enquanto a chave do circuito \\(RL\\) permanecer fechada.

    1. Será desenvolvida uma técnica para calcular diretamente a resposta do regime permanente (para não precisar resolver a EDO);
        - Entretanto, tal técnica não permite que a resposta do estado transitório ou a resposta total do sistema sejam obtidas de imediato;
    2. Ao analisar esta segunda expressão verifica-se que a resposta do regime permanente é uma função senoidal;
    3. Que a frequência do sinal de resposta é a mesma do sinal oriundo da fonte de tensão;
    4. De modo geral, a amplitude máxima da resposta de regime permanente é diferente da amplitude máxima da tensão oriunda da fonte.
        - Neste caso, a amplitude máxima da resposta de regime permanente é dada por \\(\frac{V_{m}}{\sqrt{R^{2} + \omega^{2} L^{2}}}\\).
        - E a amplitude máxima da tensão oriunda da fonte é dada por \\(V_{m}\\).
    5. Por fim, é costume que o ângulo de fase do sinal da resposta seja diferente do ângulo de fase da fonte.
        - Neste caso do circuito \\(RL\\), o ângulo de fase da compomenente permanente da resposta é dado por \\(\phi - \theta\\).
        - E o ângulo de fase da fonte é dado por \\(\phi\\).

Todas estas características nos ajudam a entender a motivação do **método dos fasores** — que nos ajuda a resolver as EDOs apenas pela análise da resposta do regime permanente (determinar a amplitude máxima da resposta do regime permanente e o ângulo de fase de seu sinal) quando sejam conhecidas a forma de onda e a frequência da resposta — abordado na sequência.

</div>


---

<!-- _class: lead -->
# Método dos Fasores


---

## Fasores - Método dos Fasores

O método dos fasores é um método matemático que simplifica a análise de circuitos que operam em regime permanente senoidal. Fasores, como veremos na sequência, são representações complexas de ondas senoidais, onde as magnitudes e as fases das ondas são expressas como números complexos. Estas representações permitem transformar equações diferenciais em equações algébricas, o que simplifica muito a análise de circuitos.


---

## O Conceito de Fasor

<div class="regular">

Fasor é um número complexo que contém as informações da amplitude e do ângulo de fase de uma função senoidal. Seu conceito fundamenta-se na identidade de Euler, que relaciona a função exponencial com a função trignométrica:

\\[
    e^{\pm j\theta} = \cos(\theta) \pm j\sin(\theta)
\\]

Esta equação é importante porque nos fornece outra maneira de representar as funções trignométricas cosseno e seno. Podemos expressar a função cosseno como a parte real da função exponencial complexa, e a função seno como a parte imaginária da função exponencial complexa; como visto:

\\[
\\begin{align}
    \\cos(\\theta) &= ℜ  \\left\\{ e^{j \\theta} \\right\\} \\\\
    \\sin(\\theta) &= ℑ  \\left\\{ e^{j \\theta} \\right\\}
\\end{align}
\\]

ℜ (forma alternativa da letra R) e ℑ (forma alternativa da letra I) são operadores que extraem a parte real e a parte imaginária de um número complexo significando, respectivamente, **ℜ : a parte real de** e **ℑ : a parte imaginária de**.

</div>


---

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

Assim, podemos chamar **\\(r e^{j \phi}\\) como o fasor \\(𝕍 \\)** e portanto, a tensão \\(V(t)\\) pode ser escrita como:

\\[
    V(t) = \Re\\{𝕍 e^{j\omega t}\\}.
\\]

Que significa que \\(V(t)\\) é a parte real da função complexa resultante da multiplicação do fasor 𝕍  por \\(e^{j(\omega t)}\\) e como sabemos, esta parte real, ao final da multiplicação, é dada por \\(r \cos(\omega t + \phi)\\).

**Por conveniência das nossas resoluções, escolheremos sempre a parte real das nossas exponenciais complexas — funções cosseno — e, por isso, não abordaremos suas partes imaginárias. Entretanto, nem por isso estamos livres de lidar com funções senos, por isso, veremos mais a frente identidades trigonométricas que habilitam a conversão de funções senos para cossenos.**

</div>


---

## Fasores

<div class="normal">

**Nos circuitos elétricos que trabalharemos, excitados por uma única fonte senoidal, a frequência angular para cada elemento do circuito — resistor, indutor, capacitor — será a mesma da fonte, portanto, nas nossas análises, não precisamos considerar a todo instante a exponencial complexa da frequência angular \\(e^{j \omega t}\\). Precisamos considerar apenas o fasor \\(𝕍 = r e^{j \phi}\\).**

Existem três formas que utilizamos para representar um fasor 𝕍 qualquer:
1. Exponencial
2. Polar
3. Retangular

</div>


---

## Fasores - Representação Exponencial

<div class="regular">

Considere um fasor \\(𝕍\\) qualquer, de amplitude \\(r\\) e ângulo \\(\phi\\).

A representação exponencial do fasor é a que já conhecemos, dada por:

\\[𝕍 = r \cdot e^{j \phi}\\]

</div>

## Fasores - Representação Polar

A forma polar de um fasor é obtida através da forma expoencial \\(r e^{j \phi}\\) e é simplesmente escrita pela notação angular envolvendo a amplitude \\(r\\) e o ângulo de fase \\(\phi\\):

\\[𝕍 = r \angle \phi\\]


---

## Fasores - Representação Retangular

<div class="regular grid-50-50">

<div class="grid-element">

A forma retangular de um fasor é obtida pelas coordenadas cartesianas do ponto que representa o fasor no plano complexo, como mostrado na figura abaixo:

<!-- _class: center transparent -->
![](https://i.imgur.com/wB3Df0c.png)

E por isso, o fasor \\(𝕍\\) é representado em sua forma retangular como:

\\[ 𝕍 = x + j y \\]

</div>

<div class="grid-element">

Se observarmos a forma exponencial \\(r e^{j \phi}\\) a partir da identidade de euler, podemos reescrevê-la como:

\\[ r e^{j \phi} = r \cos \phi + j r \sin \phi \\]

E se compararmos com a forma retangular \\(x + j y\\), podemos concluir que:

<div class="grid-50-50">

<div class="grid-element">

\\[
\begin{align}
    x &= r \cos \phi \\\\
    r &= \sqrt{x^2 + y^2} 
\end{align}
\\]

</div>

<div class="grid-element">

\\[
\begin{align}
    y &= r \sin \phi \\\\
    \phi &= {\tan}^{-1} \left( \frac{y}{x} \right) 
\end{align}
\\]

</div>

</div>

\\[
    z = x + j y = r \left( \cos \phi + j \sin \phi \right) = r e^{j \phi} = r \angle \phi
\\]

<div class="grid-50-50">

<div class="grid-element">

\\[
\begin{align}
    \cos \phi = \Re \left\\{ e^{j \phi} \right\\} 
\end{align}
\\]

</div>

<div class="grid-element">

\\[
\begin{align}
    \sin \phi = \Im \left\\{ e^{j \phi} \right\\} 
\end{align}
\\]

</div>

</div>

</div>

</div>


---

## Fasores - Utilidade das representações

Porque vimos estas representações?

Vimos a representação exponencial, pois, as demais (polar e retangular) derivam-se dela e por fim, vimos tanto a representação polar quanto a representação retangular para ampliar nosso arsenal de ferramentas para realizar operações entre números complexos, pois, para a soma e subtração de números complexos, a representação retangular (cartesiana) é mais adequada, enquanto que para as demais operações, a representação polar é mais adequada como veremos a seguir.


---

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


---

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


---

## Operações Matemáticas com Números Complexos na Representação Fasorial

<div class="small">

### Demais operações com números complexos

Agora, as demais operações matemáticas necessárias de números complexos — **Inversão, Raiz Quadrada e Complexo Conjugado** — são realizadas nas representações polares dos números. Como as conversões já foram vistas e os detalhes das explicações da multiplicação e divisão são similares nestas operações, são mostradas apenas as fórmulas para cada uma destas operações.

Considere o número complexo \\(𝕍 = r e^{j \phi}\\).

<!-- _class: lead -->
#### Inversão

\\[𝕍^{-1} = \frac{1}{𝕍} = \frac{1}{r} \angle - \phi \\]

#### Raiz Quadrada

\\[\sqrt{𝕍} = \sqrt{r} \angle \frac{\phi}{2} \\]

#### Complexo Conjugado

\\[
\begin{align}
𝕍 &= x + j y = r e^{j \phi} = r \angle \phi \\\\
𝕍^{*} &= x - j y = r e^{-j \phi} = r \angle - \phi \\\\
\end{align}
\\]

</div>


---

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

Na representação fasorial, podemos escrever \\(v(t) = 𝕍 e^{j \omega t}\\), e assim:
Considerando apenas o fasor \\(𝕍\\), temos:

\\[
\begin{align}
    \frac{d 𝕍 e^{j \omega t}}{dt} &= j \omega 𝕍 e^{j \omega t} \\\\
    \int{𝕍 e^{j \omega t}} dt &= \frac{𝕍 e^{j \omega t}}{j \omega} + K
\end{align}
\\]

Quando analisarmos as grandezas de interesse nos circuitos excitados por apenas uma fonte senoidal, podemos considerar apenas o fasor \\(𝕍\\) e desprezar o termo \\(e^{j \omega t}\\), pois ele não afeta o valor da grandeza em questão.

</div>


---

## Transformada Fasorial, Domínio do Tempo e Domínio da Frequência

<div class="regular">

Quando analisamos nossas funções de onda tão somente pelas suas componentes senoidais (e/ou cossenoidais) lidamos com estas funções no domínio do tempo.

Quando nossa função é do tipo \\(v(t) = V_{m} \cos(\omega t + \phi)\\), sabemos que podemos representar \\(\cos(\omega t + \phi)\\) como a parte real do número complexo \\(e^{j(\omega t + \phi)}\\), ou seja, \\(v(t) = \Re(V_{m} e^{j(\omega t + \phi)}) = \Re(𝕍 e^{\omega t}) \\). E quando é do tipo seno, sabemos que podemos representar nossa função seno como a parte imaginária do número complexo \\(e^{j(\omega t + \phi)}\\), ou seja, \\(v(t) = \Im(V_{m} e^{j(\omega t + \phi)}) = \Im(𝕍 e^{\omega t}) \\).

Voltando ao começo da aula, a **parte real de** ou a **parte imaginária de** representam **TRANSFORMADAS FASORIAIS**. E existem as transformadas fasoriais inversas que produzem cossenos e senos a partir de números complexos.

Quando expressamos nossas funções como cossenos e senos, estamos no **domínio do tempo**. Mas quando aplicamos transformadas fasoriais à elas para encontrar números complexos que as produzam e fazemos nossas operações matemáticas com estes números complexos, pelo benefício da simplicidade da notação fasorial, mudamos para o **domínio da frequência**.

Veremos agora nos próximos slides identidades e relações trigonométricas (necessárias para a resolução do exemplo 9.5 e para transformar senos em cossenos e vice-e-versa) e por fim, veremos na resolução do próprio exemplo 9.5 como a representação fasorial, obtida após as transformadas fasoriais, simplifica (e muito) a resolução de problemas de circuitos elétricos excitados por fontes senoidais — circuitos de corrente alternada.

</div>


---

## Identidades Trigonométricas
### Pequena Revisão

<div class="small">

Por muitas vezes lidarmos com operações de números complexos (em suas representações polares ou retângulares) que produzem funções do tipo seno nas suas resultantes, precisamos de identidades trigonométricas para, quando necessário, convertermos as funções resultantes em funções do tipo cosseno, objetos da nossa disciplina, ou funções do tipo seno, quando necessário.

Assim, apresentamos a seguinte tabela de identidades:

<div style="text-align: center;">

**Identidades Trigonométricas**

</div>

<!-- _class: ttable -->
|             Função              |                            Equivalência                             |      Equivalência      |
|:-------------------------------:|:--------------------------------------------------------------------|------------------------|
|       \\(\sin(A \pm B)\\)       |                \\(\sin(A)\cos(B) \pm \cos(A)\sin(B)\\)              |                        |
|       \\(\cos(A \pm B)\\)       |                \\(\cos(A)\cos(B) \pm \sin(A)\sin(B)\\)              |                        |
|  \\(\sin(\omega t \pm 180°)\\)  |    \\(\sin(\omega t) \cos(180°) \pm \cos(\omega t) \sin(180°)\\)    | \\(- \sin(\omega t)\\) |
|  \\(\cos(\omega t \pm 180°)\\)  |    \\(\cos(\omega t) \cos(180°) \mp \sin(\omega t) \sin(180°)\\)    | \\(- \cos(\omega t)\\) |
|  \\(\sin(\omega t \pm  90°)\\)  |    \\(\sin(\omega t) \cos( 90°) \pm \cos(\omega t) \sin( 90°)\\)    |\\(\pm \cos(\omega t)\\)|
|  \\(\cos(\omega t \pm  90°)\\)  |    \\(\cos(\omega t) \cos( 90°) \mp \sin(\omega t) \sin( 90°)\\)    |\\(\mp \sin(\omega t)\\)|

</div>


---

## Fasores — Pequena tabela para conversão entre representações no domínio do tempo e no domínio da frequência

<div class="footnotesize">

A partir do que verificamos no slide anterior estabelecemos esta pequena tabela para conversão entre representações no domínio do tempo e no domínio da frequência:

<!-- _class: ttable -->
|              Domínio do tempo            |                                              |       Domínio da frequência       |
|:----------------------------------------:|:--------------------------------------------:|:---------------------------------:|
|         **Representação Temporal**       | **Conversão Para Representação Cossenoidal** |     **Representação Fasorial**    | 
| \\(v(t) = V_{m} \cos(\omega t + \phi)\\) |                 Não se Aplica                | \\(𝕍 = V_{m} \angle \phi\\)       |
| \\(v(t) = V_{m} \sin(\omega t + \phi)\\) |    \\(V_{m} \cos(\omega t + \phi - 90°)\\)   | \\(𝕍 = V_{m} \angle \phi - 90°\\) |
| \\(i(t) = I_{m} \cos(\omega t + \phi)\\) |                 Não se Aplica                | \\(𝕀 = I_{m} \angle \phi\\)       |
| \\(i(t) = I_{m} \sin(\omega t + \phi)\\) |    \\(I_{m} \cos(\omega t + \phi - 90°)\\)   | \\(𝕀 = I_{m} \angle \phi - 90°\\) |

Por fim, lembramos que um ângulo \\(\phi\\) em graus pode ser expresso em radianos como:

\\[ 
\phi_{\text{rad}} = \frac{\pi}{180} \phi_{°} 
\\]

E um ângulo \\(\phi\\) em radianos pode ser expresso em graus como:

\\[
\phi_{°} = \frac{180}{\pi} \phi_{\text{rad}}
\\]

Assim, agora dispomos de todas as ferramentas necessárias para realizar operações de números complexos através de fasores (domínio da frequência) como também, com suas funções senoidais (domínio do tempo) e portanto, podemos resolver o exemplo 9.5, que é o nosso próximo slide.

</div>


---

<!-- _class: lead -->
# Exemplo 9.5

## Soma de cossenos usando-se fasores.

Se \\(y_{1} = 20 \cos(\omega t - 30°) \text{ e } y_{2} = 40 \cos(\omega t + 60°)\\) expresse \\(y = y_{1} + y_{2}\\) como uma única função senoidal.

a) Resolva o problema usando identidades trigonométricas.

b) Resolva o problema usando o conceito de fasor.


---

<!-- _class: lead -->
## Soma de cossenos usando-se fasores

<center>
<iframe width="727" height="409" src="https://www.youtube.com/embed/fbPHS42Dc8A" title="Me Salva! SEN07 - Soma Fasorial" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</center>
