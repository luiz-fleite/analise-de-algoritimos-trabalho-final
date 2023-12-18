
<!-----



Conversion time: 1.845 seconds.


Using this Markdown file:

1. Paste this output into your source file.
2. See the notes and action items below regarding this conversion run.
3. Check the rendered output (headings, lists, code blocks, tables) for proper
   formatting and use a linkchecker before you publish this page.

Conversion notes:

* Docs to Markdown version 1.0$\beta$35
* Mon Dec 18 2023 05:04:11 GMT-0800 (PST)
* Source doc: trabalho_final_respostas
* Tables are currently converted to HTML tables.
----->


Universidade Federal do Pará

Instituto de Ciências Exatas e Naturais

Faculdade de Computação

Análise de Algoritmos

3ª Avaliação

Alunos:

* Luiz Antônio Lima de Freitas Leite - matrícula: 202204940008
* Max…
* Luiz Sérgio Samico…
* Wesley…

# Questão 1.

## Analise as afirmativas abaixo considerando que $\pi_1$ e $\pi_2$ são problemas de decisão e que $\pi_1$ é uma restrição de $\pi_2$. Em seguida, responda se cada uma das afirmativas é verdadeira ou falsa e justifique sua resposta.

### I. Se $\pi_1 \in P$ então $\pi_2 \in P$.

    RESPOSTA: VERDADEIRO,
            por que π1 sendo uma restrição de π2 (π2 $\propto$ π1) implica que a instância de π1 é um caso específico de π2 com algumas condições adicionais. Se já é possível resolver π1 em tempo polinomial, então também será possível resolver π2 em tempo polinomial, pois π2 engloba π1 e, portanto, incluirá a solução para π1.

### II. Se $\pi_2$ ∈ NP e $\pi_1$ ∈ NP-Completo, então $\pi_2$ ∈ NP-Completo.

        RESPOSTA: VERDADEIRO,
        pois para π2 ser NP-Completo deve satisfazer 2 condições: \
        Condição 1: π2 ∈ NP.

        Condição 2: Todo problema $\beta$ ∈ NP satisfaz $\beta$ $\propto$ π2.

        A primeira condição já foi dada, e a segunda condição é satisfeita por transitividade:

        Sabemos que π1 $\propto$ π2, pois π1 é restrição de π2, então:

        $\beta$ $\propto$ π1 e π1 $\propto$ π2 ⇒ $\beta$ $\propto$ π2

        Em resumo: “Sejam π1 e π2 problemas em NP. Se π1 for NP-Completo e
        π1 $\propto$ π2 , então π2 também é NP-Completo.”


### III. $\pi_1$ e $\pi_2$ são polinomialmente equivalentes.

    RESPOSTA: FALSO,
    pois apenas está definido que ambos os problemas são de decisão e π1 $\propto$ π2 , e para serem polinomialmente equivalentes é necessário que π2 $\propto$ π1 também, o que não pode ser afirmado sem informações adicionais.


### IV. Por serem problemas de decisão, é certo que $\pi_1$ e $\pi_2$ não pertencem à classe NP-Difícil.

    RESPOSTA: FALSO,
    pois a classe de problemas NP-Completo, por exemplo, é composta por problemas de decisão NP que ao mesmo tempo são NP-Difícil, portanto, se $\pi_1$ e π<sub>2 </sub>são NP-Completo eles são obrigatoriamente NP-Difícil.


## Questão 2. Analise as afirmativas abaixo considerando o problema de decisão da satisfatibilidade de fórmulas (SAT). Em seguida, responda se cada uma das afirmativas é verdadeira ou falsa e justifique sua resposta.
[ $[\pi_1$ $\propto$ $\]$ ]
### I. Se SAT está em P, então P = NP.

    RESPOSTA: VERDADEIRO,
    pois SAT é NP-Completo e satisfaz a propriedade de que todo problema $\beta$ ∈ NP satisfaz $\beta$ $\propto$ SAT. Então se SAT for resolvido em tempo polinomial, por transitividade, todos os problemas em NP poderão ser resolvidos em tempo polinomial também após serem transformados em SAT também em tempo polinomial.

### II. Se um problema de decisão π está em NP, então SAT é polinomialmente transformável em π.

    RESPOSTA: FALSO,
    pois mesmo que todo problema $\beta$ ∈ NP satisfaz $\beta$ $\propto$ SAT, o vice-versa não é garantido, portanto é incorreto afirmar SAT $\propto$ $\beta$.

### III. Um problema π está em NP-Difícil se e somente se SAT é polinomialmente transformável em π.

    RESPOSTA: VERDADEIRO, 
    pois para um problema π estar em NP-Difícil ele deve satisfazer a propriedade de que todo problema $\beta$ ∈ NP satisfaz $\beta$ $\propto$ π, e como SAT é NP-Completo, e por consequência também é NP, isso implica que SAT $\propto$ π deve ser verdadeiro para que π satisfaça essa propriedade dos NP-Difíceis.

### IV. Uma importante consequência do Teorema de Cook é que se existe um algoritmo de tempo polinomial para resolver SAT, então existe um algoritmo de tempo polinomial para resolver todos os problemas em NP.

        RESPOSTA: VERDADEIRO,
        pois SAT é NP-Completo e satisfaz a propriedade de que todo problema $\beta$ ∈ NP satisfaz $\beta$ $\propto$ SAT. Então se SAT for resolvido em tempo polinomial, por transitividade, todos os problemas em NP poderão ser resolvidos em tempo polinomial também após serem transformados em SAT também em tempo polinomial.

## Questão 3. Dado que $\pi_1$ e $\pi_2$ são problemas de decisão, indique se cada uma das afirmativas abaixo é verdadeira ou falsa. Em seguida, justifique sua resposta.

### I. Se $\pi_1$ ∈ NP-Completo e $\pi_2$ ∈ NP, então $\pi_1$ $\propto$ $\pi_2$.

    RESPOSTA: FALSO,
    pois mesmo que todo problema $\pi_2$ ∈ NP satisfaz $\pi_2$ $\propto$ $\pi_1$, o vice-versa não é garantido, portanto é incorreto afirmar $\pi_1$ $\propto$ $\pi_2$.

### II. Não é possível ter uma heurística de custo polinomial para um problema NP-Completo que, para qualquer dado de entrada, garanta obter a solução ótima do problema.

    RESPOSTA: VERDADEIRO,
    pois, se fosse encontrado um algoritmo de tempo polinomial que resolva um problema NP-Completo para todas as entradas, isso equivaleria a mostrar que P (problemas solúveis em tempo polinomial) é igual a NP (problemas cujas soluções podem ser verificadas em tempo polinomial), mas até agora essa questão permanece um problema em aberto na teoria da complexidade computacional. Até que essa questão seja resolvida, acredita-se que não existem heurísticas polinomiais que garantam soluções ótimas para todos os casos de problemas NP-Completo.

### III. Considere que $\pi_1$ ∈ NP-Completo. Caso fosse descoberto um algoritmo polinomial para resolver $\pi_1$, então todos os problemas em NP também poderiam ser resolvidos em tempo polinomial.

    RESPOSTA: VERDADEIRO,
    pois sendo $\pi_1$ NP-Completo ele satisfaz a propriedade de que todo problema $\beta$ ∈ NP satisfaz $\beta$ $\propto$ $\pi_1$. Então se $\pi_1$ for resolvido em tempo polinomial, por transitividade, todos os problemas em NP poderão ser resolvidos em tempo polinomial também após serem transformados em $\pi_1$ também em tempo polinomial.

### IV. Se P = NP, então todo problema NP-Difícil pode ser resolvido em tempo polinomial.

    RESPOSTA: FALSO,
    pois, por exemplo:

    É verdade que se $\pi_1$ é restrição de $\pi_2$ , ou seja,  $\pi_2$ $\propto$ $\pi_1$, e π1 é resolvido em tempo polinomial, então π2 também é resolvido. Entretanto, o vice-versa não é garantido.

    Portanto ainda que para todo problema $\beta$ ∈ P=NP e π ∈ NP-Difícil, é verdade que $\beta$ $\propto$ π, resolver $\beta$ não garante a resolução de π.


### V. Suponha que $\pi_1$ e $\pi_2$ pertencem à classe NP-Completo. Isso implica que existe uma transformação polinomial no tempo de um problema para outro mesmo se P ̸= NP.

    RESPOSTA: VERDADEIRO,
    pois atualmente não se sabe se P /= NP, mas já é possível observar que os problemas NP-Completo são polinomialmente equivalentes entre si.

## Questão 4. Uma cobertura de vértices de um grafo G = (V, E) é um subconjunto V <sup>′</sup> ⊆ V de k vértices, tal que se (u, w) ∈ E então u ∈ V <sup>′</sup> ou w ∈ V <sup>′</sup> . Isto posto, considere o problema de decisão π descrito abaixo para responder os itens a seguir.

### Dados de entrada: Um grafo G e um inteiro k > 0.
### Decisão: G possui uma cobertura de vértices de tamanho ≤ k?
### a) Mostre se o problema π pertence, ou não, à classe NP.

-------------
    RESPOSTA:  
    Para provar que π pertence a NP é necessário verificá-lo:

    FASE 1: Exibição e justificativa da resposta “sim”.

    Dado o grafo G e k = x: 
    [Grafo G]

    justificativa para a cobertura de vértices de tamanho menor que x:

    [conjunto com menos de x vértices que cubra todo o grafo G]

    FASE 2: verificação da resposta “sim” em tempo polinomial:

    pseudocódigo:
```
VERIFICA(G,V',k)
    // primeiro testa o tamanho de V'
    se |V'| > k:
        retorna "FALSO"
    // depois verifica se V' cobre todas as arestas
    teste = E // conjunto teste temporário
    para cada v em V':
        para cada e em teste: // "e" é aresta
            se v está em e:
                remove e de teste
    se |teste| == 0: retorna "VERDADEIRO"
    senão: retorna "FALSO"

complexidade de tempo:
O(|V'| + |V'| * E)
termo mais dominante
O(|V'| * E)
como V não pode ser maior que K:
O(k * E)
```



### b) Sabe-se que o problema da satisfatibilidade de fórmulas (SAT) é polinomialmente transformável no problema π. Então, é possível afirmar que π ∈ NP-Completo? Por quê?

    RESPOSTA: Sim, 

    pois para ser NP-Completo deve satisfazer 2 condições: \
    Condição 1: π ∈ NP.

    Condição 2: Todo problema $\beta$ ∈ NP satisfaz $\beta$ $\propto$ π.

    A primeira condição já foi dada, e a segunda condição é satisfeita por transitividade:

    $\beta$ $\propto$ SAT e SAT $\propto$ π ⇒ $\beta$ $\propto$ π

    Em resumo: “Sejam π1 e π2 problemas em NP. Se π1 for NP-Completo e

    π1 $\propto$ π2 , então π2 também é NP-Completo.”

## Questão 5. Considere o problema de decisão π descrito abaixo.

### Dados de entrada: Dois grafos G<sub>1</sub> = (V<sub>1</sub>, E<sub>1</sub>) e G<sub>2</sub> = (V<sub>2</sub>, E<sub>2</sub>), com |V<sub>1</sub>| = |V<sub>2</sub>|.
### Decisão: Existe uma função f : V<sub>1</sub> → V<sub>2</sub>, tal que (u, w) ∈ E<sub>1</sub> se e somente se (f(u), f(w)) ∈ E<sub>2</sub>, para todo u, w ∈ V<sub>1</sub>?

Mostre se o problema π pertence, ou não, à classe NP.

--------------------------
    RESPOSTA:
    Para provar que π pertence a NP é necessário verificá-lo:

    FASE 1: Exibição e justificativa da resposta “sim”.

    Dado o grafo G1 e G2: \
    [Grafo G1] [Grafo G2]

    justificativa para função que transforma G1 em G2:

    [Conjunto contendo as transformações dos vértices que compõe as arestas]

    FASE 2: verificação da resposta “sim” em tempo polinomial:

    pseudocódigo:
```
VERIFICA(G1, G2, f())
    // primeiro testa as cardinalidades de V1 e V2
    se |V1| != |V2|:
        retorna "FALSO"
    teste1 = {} // conjunto de teste temporário
    teste2 = E2 // conjunto de teste temporário
    // depois aplica a função f() nos elementos de V1
    para cada (u, w) em E1:
        // adiciona a aresta com os vértices transformados por f()
        teste1 = teste1 + (f(u), f(w))
    // em seguida verifica se G1 tornou-se equivalente a G2
    para cada (u1, w1) em teste1:
        para cada (u2, w2) em teste2:
            se (u1, w1) == (u2, w2):
                remove (u1, w1) de teste1
                remove (u2, w2) de teste2
                pula para o próximo elemento de teste1
    se |teste1 + teste2| == 0: retorna "VERDADEIRO"
    senão: retorna "FALSO"

complexidade de tempo:
O(|V1| + |E1| + |E1| * |E2|)
termo mais dominante
O(|E1| * |E2|)
```

## Questão 6. Essa questão é composta por 2 (dois) problemas. Observe que todos os algoritmos usados para resolver os problemas devem ser eficientes, ou seja, não é permitido o uso de algoritmos não-polinomiais em nenhuma parte da solução apresentada.

## Problema 1

        A Segunda Guerra Mundial iniciou-se no dia 1 de setembro de 1939, quando a Polônia foi subitamente atacada pela Alemanha. O Estado-Maior polonês se reuniu de imediato para decidir sobre as movimentações de tropas que deveriam efetuar, de modo a fazer frente à invasão alemã.


        As forças polonesas foram informadas que o ataque alemão se daria em três frentes distintas, com nomes de código $\beta$<sub>1</sub>, $\beta$<sub>2</sub> e $\beta$<sub>3</sub>. Chegou-se à conclusão que seria necessário transportar duas divisões de combate para $\beta$<sub>1</sub>, uma divisão para $\beta$<sub>2</sub> e uma outra para $\beta$<sub>3</sub>. A Polônia dispunha nessa altura de cinco divisões de combate nas cidades mais próximas da fronteira atacada, duas aquarteladas na cidade α<sub>1</sub>, duas em α<sub>2</sub> e uma aquartelada em α<sub>3</sub>. Essas divisões poderiam ser transportadas para os locais em perigo, contudo, a força aérea alemã já sobrevoava a Polônia, e a movimentação das divisões teria que ser feita com o menor risco humano possível.

        Após uma rápida inspeção do mapa do território, fez-se o esquema da Figura 1, onde as estradas que poderiam ser utilizadas pelas divisões de combate polonesas são apresentadas. Observe que o valor da aresta representa a distância em quilômetros.

Figura 1: Esquemático do território.


        Os generais poloneses precisavam decidir de que aquartelamento deviam seguir as divisões necessárias em $\beta$<sub>1</sub>, $\beta$<sub>2</sub> e $\beta$<sub>3</sub>. O objetivo era a minimização das perdas humanas, relacionado diretamente com o perigo de bombardeamento.


        Então, durante a reunião decisiva, o general polonês Edward disse: “O perigo de bombardeamento das divisões em movimento pode ser considerado como diretamente proporcional à distância entre cada cidade α e cada frente $\beta$. Nesse caso, devem-se usar essas distâncias como o perigo que uma divisão corre ao ser transportada de α<sub>i</sub> para $\beta$<sub>i</sub>”. Em seguida, o general Jerzy ordenou: “A divisão que sobrar fica no aquartelamento respectivo”.


        Tarefa: Siga as instruções dos generais Edward e Jerzy, e informe quais foram as decisões tomadas pelas forças armadas polonesas. Explique detalhadamente, por meio de um relatório técnico, a estratégia e os algoritmos usados para resolver o problema.

---
     RESPOSTA:

## Problema 2

        Uma indústria deve fabricar um lote composto por 3 (três) peças: duas em PVC (peças A e B) e uma em aço inoxidável (peça C). As peças A e B devem ser torneadas e depois rosqueadas, mas a peça C deve apenas ser torneada. Depois de trabalhadas, as peças A e 

* devem ser montadas e então acopladas à peça B. Finalmente, as peças prontas devem ser embaladas e armazenadas.

    Algumas dessas tarefas podem ser feitas simultaneamente, mas outras dependem de tarefas anteriores. Uma forma de codificar isso é por meio de uma tabela de precedências (vide Tabela 1). Note que ao lado de cada tarefa encontram-se as tarefas das quais ela depende imediatamente e a duração da tarefa em minutos.

Tabela 1: Tabela de Precedências.

<table>
  <tr>
   <td colspan="3" >
    Tarefa (ou atividade)
   </td>
   <td>
    Antecedentes
   </td>
   <td>
    Duração (min)
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td colspan="2" >
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
    1.
   </td>
   <td colspan="2" >
    Preparar os tornos
   </td>
   <td>–
   </td>
   <td>8
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td colspan="2" >
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
    2.
   </td>
   <td colspan="2" >
    Preparar as embalagens
   </td>
   <td>–
   </td>
   <td>8
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td colspan="2" >
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
    3.
   </td>
   <td colspan="2" >
    Cortar e distribuir o PVC
   </td>
   <td>–
   </td>
   <td>10
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td colspan="2" >
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
    4.
   </td>
   <td colspan="2" >
    Cortar e distribuir o aço
   </td>
   <td>–
   </td>
   <td>12
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td colspan="2" >
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
    5.
   </td>
   <td colspan="2" >
    Tornear a peça A
   </td>
   <td>1,3
   </td>
   <td>8
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td colspan="2" >
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
    6.
   </td>
   <td colspan="2" >
    Tornear a peça B
   </td>
   <td>1,3
   </td>
   <td>11
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td colspan="2" >
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
    7.
   </td>
   <td colspan="2" >
    Tornear a peça C
   </td>
   <td>1,4
   </td>
   <td>15
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td colspan="2" >
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
    8.
   </td>
   <td colspan="2" >
    Rosquear a peça A
   </td>
   <td>5
   </td>
   <td>9
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td colspan="2" >
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
    9.
   </td>
   <td colspan="2" >
    Rosquear a peça B
   </td>
   <td>6
   </td>
   <td>7
   </td>
  </tr>
  <tr>
   <td colspan="2" >
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td colspan="2" >
    10.
   </td>
   <td>
    Montar as peças A e C
   </td>
   <td>7,8
   </td>
   <td>4
   </td>
  </tr>
  <tr>
   <td colspan="2" >
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td colspan="2" >
    11.
   </td>
   <td>
    Montar a peça B
   </td>
   <td>9,10
   </td>
   <td>6
   </td>
  </tr>
  <tr>
   <td colspan="2" >
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td colspan="2" >
    12.
   </td>
   <td>
    Embalar e armazenar
   </td>
   <td>2,11
   </td>
   <td>7
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

        Tarefa: Explique, por meio de um relatório técnico, a estratégia e os algoritmos usados para encontrar:

* O tempo mínimo, isto é, o tempo antes do qual não é possível terminar o conjunto de tarefas;
* As tarefas críticas ou de folga nula, ou seja, aquelas que não toleram atrasos;
* As tarefas que podem sofrer atrasos com as respectivas folgas.

