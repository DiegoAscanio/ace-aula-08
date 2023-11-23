## O Conceito de Fasor - Transformada Fasorial Inversa

<div class="regular">

Até o momento fizemos a transformada fasorial da função senoidal \\(v_{s}(t)\\), entretanto, é possível fazer o processo inverso, transformar uma representação fasorial \\(\\mathbf{V}\\) em uma função senoidal \\(v_{s}(t)\\), ou seja, escrever para um fasor a expressão de sua funão senoidal equivalente.

Consideremos o fasor \\(\\mathbf{V} = {100} \angle {-26°} \\).

Como escolhemos usar a função cosseno como função senóide para tensão, temos que sua representação senoidal é:

\\[v_{s}(t) = 100 \cos(\omega t - 26°)\\]

Somente com as informações contidas na representação fasorial não é possível deduzir o valor de \\(\omega\\), pois, ele contém somente as informações de amplitude e de fase. A ação de converter a transformada fasorial para sua expressão no domínio do tempo é denominada de **transformada inversa fasorial** e é representada pela equação:

\\[
Ƒ^{-1} \\{ V_{m} e^{j \phi} \\} = ℜ  \left\\{ V_{m} e^{j \phi} e^{j \omega t} \right\\} \tag{7}
\\]

</div>
