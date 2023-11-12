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

</style>

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>


# Análise de Circuitos Elétricos
## Aula 08 - Análise do Regime Permanente Senoidal
 
Prof. M.Sc. Diego Ascânio Santos (ascanio@cefetmg.br)

Aula baseada sobre o material do professor Dr. Emerson Gonçalves de Melo (emerdemelo@usp.br - DEMAR EEL USP), da professora Drª. Thabatta Moreira Alves de Araújo (thabatta@cefetmg.br - DIGDDV) e da Khan Academy.

CEFET-MG DIGDDV - Divinópolis, 2023.


---

## Roteiro

1. Fonte senoidal. 
2. Resposta senoidal.
3. O conceito de Fasor
4. Elementos passivos no domínio da frequência.
5. As leis de Kirchhoff no domínio da frequência.
6. Associações em série e em paralelo e transformações \\(\Delta\\) - Y.
7. Equivalentes de Thévenin e de Norton.
8. Transformadores.
9. Diagramas fasoriais.


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
