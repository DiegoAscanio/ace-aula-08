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
