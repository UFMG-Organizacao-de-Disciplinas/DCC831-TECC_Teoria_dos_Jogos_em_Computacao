# Lista 1 - Revisar Q5

Teoria dos Jogos em Computação

**Professor:** Pedro Olmo Stancioli Vaz de Melo

## Utility

### 1. Give an example of preferences over a countable set in which the preferences cannot be represented by a utility function that returns only integers as values

#### Resposta 1

Considerando o conjunto dos números racionais $\mathbb{Q}$, que são contáveis. Se formos tentar comparar dois números racionais $q_1$ e $q_2$, podemos ter $q_1 \succ q_2$ se $q_1 > q_2$. E se, tentarmos usar uma função de utilidade $u: \mathbb{Q} \rightarrow \mathbb{Z}$, teríamos que $u(q_1) > u(q_2)$, o que não é possível, isso porque como $\mathbb{Z} \subset \mathbb{Q}$, logo não existe uma função de utilidade que possa mapear todos os números racionais em números inteiros, já que existem infinitos números racionais entre dois números inteiros. Portanto, não é possível representar as preferências sobre um conjunto contável com uma função de utilidade que retorna apenas valores inteiros.

---

### 2. A farmer wants to dig a well in a square field. The preferences of the farmer on the possible locations are lexicographic

> i.e:
>
> - If $x_1 < x_2$ then $(x_1, y_1) \succ (x_2, y_2)$ for all $y_1, y_2$.
> - If $x_1 = x_2 = x$, then $(x, y_1) \succ (x, y_2)$ iff $y_1 < y_2$.
>
> - First, assume that the field has dimensions $[0, 1000] \times [0, 1000]$ and construct a linear utility function that represents this relation. Second, construct a utility function assuming that the field has dimensions $[0,\infty) \times [0,\infty)$. For both cases, assume that the well location must have integer coordinates.

#### Resposta 2

**Resposta:** Queremos uma função de utilidade que represente que, quanto menor os valores de $X$ e $Y$, melhor a localização do poço. Além disso, tem-se por primeira ordem de desempate o valor de $X$ e, por segunda ordem de desempate, o valor de $Y$.

Intuitivamente, podemos considerar que para determinado $X$, mesmo com o maior valor de $Y$, sua função de utilidade será sempre menor que a de um $X + 1$ e $Y$ mínimo. Matematicamente: $u(X, \max{(Y)}) < u(X + 1, \min{(Y)})$.

Precisamos então que $X$ seja multiplicado por um valor tal que garanta a veracidade de nossa intuição, para tanto, consideremos que: $u(X, Y) = -\alpha X - Y$, onde $\alpha > \max{(Y)}$.

**Parte 1:** Para o caso das dimensões $[0, 1000] \times [0, 1000]$, podemos consideramos então que $\max{(Y)} = 1000$ e, portanto, se $\alpha > 1000$, podemos considerar o menor valor natural de $\alpha = 1001$. Sendo assim, temos que a função de utilidade é dada por: $u(X, Y) = -1001X - Y$.

|    $X$ |    $Y$ |  $u(X, Y)$ |
| -----: | -----: | ---------: |
|    $0$ |    $0$ |        $0$ |
|    $0$ |    $1$ |       $-1$ |
|    $0$ | $1000$ |    $-1000$ |
|    $1$ |    $0$ |    $-1001$ |
|    $1$ | $1000$ |    $-2001$ |
|    $2$ |    $0$ |    $-2002$ |
|  $999$ | $1000$ | $-1000999$ |
| $1000$ |    $0$ | $-1001000$ |
| $1000$ | $1000$ | $-1002000$ |

Essa equação poderia ser modificada de duas formas:

1. Poderia-se limitar o valor de retorno aos números naturais.
2. Poderia-se definir uma função de utilidade que retornasse valores entre 0 e 1.

Mas deixemos assim mesmo.

**Parte 2:** Agora, para o caso das dimensões $[0, \infty) \times [0, \infty)$, podemos considerar que $\max{(Y)} = \infty$ e, portanto, se $\alpha > \infty$... Bom, $\infty + 1 = \infty$, e uma função de utilidade $u(X, Y) = -\infty X - Y$ acaba não sendo condizente. Sendo assim, não é possível definir uma função de utilidade que represente essa relação.

Outra análise mais conceitual a se fazer é que essa função de utilidade é chamada de função de utilidade lexicográfica, e ela apenas é válida para conjuntos finitos.

---

### 3. Is the statement "if both $U$ and $V$ represent $\succsim$, then there is a strictly monotonic function $f : \mathbb{R} \rightarrow \mathbb{R}$ such that $V(x) = f(U(x))$" correct?

> - **Tip:** consider $V(x) = x$ and $U(x) = \begin{cases} x, & \text{se } x \leq 0 \\ x + 1, & \text{se } x > 0 \end{cases}$

#### Resposta 3

Consideramos então que temos $U$ e $V$ como funções de utilidade que representam a mesma relação de preferência $\succsim$. Para confirmar a afirmação, precisamos mostrar que existe uma função estritamente monótona (ou seja, que sempre cresça ou decresça) $f$ que converta os valores de $U$ em valores de $V$.

Seguindo a sugestão dada, consideremos as funções $U$ e $V$ que têm a mesma relação de preferência $\succsim$:

$U(x) = \begin{cases} x, & \text{se } x \leq 0 \\ x + 1, & \text{se } x > 0 \end{cases}$

$V(x) = x$

Poderíamos então alterar a função $U$ para representar a função $V$:

$U(x) = \begin{cases} V(x), & \text{se } x \leq 0 \\ V(x) + 1, & \text{se } x > 0 \end{cases}$

Então, os únicos casos em que $U$ se diferencia de $V$ são quando $x > 0$. Para esses casos, podemos definir a função $f$ como:

$f(x) = \begin{cases} x, & \text{se } x \leq 0 \\ x - 1, & \text{se } x > 0 \end{cases}$

Então, aplicando a função $f$ em $U'$, temos:

$f(U(x)) = \begin{cases} f(V(x)), & \text{se } x \leq 0 \\ f(V(x) + 1), & \text{se } x > 0 \end{cases}$

$f(U(x)) = \begin{cases} V(x), & \text{se } x \leq 0 \\ (V(x) + 1) - 1, & \text{se } x > 0 \end{cases}$

$f(U(x)) = \begin{cases} V(x), & \text{se } x \leq 0 \\ V(x), & \text{se } x > 0 \end{cases}$

$f(U(x)) = V(x)$

Porém, percebe-se que, $f(x)$ não é uma função estritamente monótona, isso no intervalo $[0, 1]$, visto que $f(0) = f(1) = 0$.

Concluimos então que, a afirmação não é verdadeira, visto que para que a $f(U(x))$ conseguisse se igualar a $V(x)$, a função $f$ precisaria ser não estritamente monótona.

---

#### 4. Can a continuous preference relation be represented by a discontinuous utility function?

##### Resposta 4

Sim. A função de utilidade $U$ apresentada na questão anterior exemplifica exatamente esse fato. Embora ela seja descontínua em $x = 0$, ela ainda representa uma relação de preferência contínua.

---

### 5. Show that in the case of $X = \mathbb{R}$, the preference relation that is represented by the discontinuous utility function $u(x) = floor(x)$ is not a continuous relation

> $floor(x)$: the largest integer $n$ such that $x \geq n$

#### Resposta 5

Não consegui entender e dizer com convicção que isso é verdade. Trocando uma ideia com o GPT, entendi que pode ter relação com limites e conjuntos fechados, mas ainda assim as explicações me soaram esquisitas.

---

## Choice

### 6. The following are descriptions of decision-making procedures. Discuss whether the procedures can be described in the framework of the choice model discussed in this course and whether they are compatible with the "rational man" paradigm. In other words, can I construct a utility function $u(x)$ based solely on the set of alternatives $x \in X$ according with these procedures? Explain why (e.g. with an example)

Para essa questão, consideremos que $C_{\succsim}(A)$ representa a função que encontra o melhor dos elementos possíveis pertencentes ao conjunto $A = \{u(x) | x \in X\}$.

#### 1. The decision maker chooses an alternative in order to maximize another person’s suffering

##### Resposta 6.1

Sim, é compatível. Isso pois sua função de utilidade pode ser representada como $u(x) = -v(x)$, onde $v(x)$ é a função de utilidade do outro indivíduo, ou seja, quanto menor for $v(x)$, maior seria o sofrimento. Assim, o agente racional irá escolher a alternativa que maximiza a função de utilidade negativa do outro indivíduo.

#### 2. The decision maker asks his two children to rank the alternatives and then chooses the alternative that is the best on average (you can use your own definition of "best on average")

##### Resposta 6.2

Sim, é compatível. Isso pois visa maximizar a média das funções de utilidade dos filhos. A função de utilidade do agente racional pode ser representada como $u(x) = \frac{f_1(x) + f_2(x)}{2}$, onde $v_1(x)$ e $v_2(x)$ são as funções de utilidade dos filhos.

#### 3. The decision maker has an ideal point in mind and chooses the alternative that is closest to it

##### Resposta 6.3

Sim, é compatível. Isso porque a função de utilidade do agente racional pode ser representada como $u(x) = -d(x, x')$, onde $d(x, x')$ é a distância entre o ponto ideal $x'$ e o ponto $x$. Assim, o agente racional irá escolher a alternativa que minimiza a distância entre o ponto ideal e o ponto escolhido.

#### 4. The decision maker looks for the alternative that appears most often in a list of alternatives

##### Resposta 6.4

Não é compatível. Isso porque a função de utilidade do agente depende de outra variável, sendo esse o conjunto de alternativas.

#### 5. The decision maker has an ordering in mind and always chooses the median element

##### Resposta 6.5

Não é compatível. Isso porque a função de utilidade do agente depende de outra variável, sendo esse o conjunto dos valores ordenados.

### 7. Consider the following choice procedure: a decision maker has a strict ordering $\succsim$ over the set $X$ and assigns to each $x \in X$ a natural number $class(x)$ to be interpreted as the "class" of $x$. Given a choice problem $A$, he chooses the best element in $A$ from those belonging to the most common class in $A$ (i.e., the class that appears in $A$ most often). If there is more than one most common class, he picks the best element from the members of $A$ that belong to a most common class

**Entendendo o enunciado:** temos um conjunto ordenado por preferência onde cada um dos elementos está arbitrariamente definido como pertencente a uma classe. Considera-se que a classe de menor número é a preferível. O seu critério para escolha de "melhor" elemento é pegar o melhor elemento da classe preferível, e em caso de empate, pegar o melhor elemento dentre as classes empatadas.

#### 7.1 Is this procedure consistent with the "rational man" paradigm?

##### Resposta 7.1

Não. Isso porque a escolha do agente racional não depende apenas da classe, mas sim de que forma o conjunto de escolhas está definido. Então se tivermos $A = \{x_1, x_2, x_3, x_4\}$ e $class(x_1) = class(x_2) = 1, class(x_3) = class(x_4) = 2$, então $C({x_1, x_2, x_3, x_4}) = x_1$, mas se $C({x_1, x_3, x_4}) = x_3$. Assim violando a condição $\alpha$ que afirma que para dos conjuntos $A, B \in D$, se $A \subset B$ e $C(B) = A$, então $C(A) = C(B)$.

#### 7.2 Define the relation: $xPy$ if $x$ is chosen from $\{x, y\}$. Show that the relation $P$ is a strict ordering (complete, asymmetric, and transitive)

- **Completo:** Para todo $x, y \in X$, temos que $xPy$ ou $yPx$.
- **Assimétrico:** Para todo $x, y \in X$, temos que se $xPy$ então não é verdade que $yPx$.
- **Transitivo:** Para todo $x, y, z \in X$, temos que se $xPy$ e $yPz$, então $xPz$.

Se todos os três critérios forem satisfeitos, então a relação $P$ é uma ordem estrita.

---

## Expected Utility

### 8. Which lottery do you prefer?

> - $L = (0.25z_1, 0.25z_2, 0.25z_3, 0.25z_4)$ OR
> - $L' = (0.15z_1, 0.50z_2, 0.15z_3, 0.20z_4)$
>
> Suppose, by continuity: $z_2 \sim z'_2 = (0.6z_1, 0.4z_4)$ and $z_3 \sim z'_3 = (0.2z_1, 0.8z_4)$

#### Resposta 8

Nessa questão de continuidade, seria o mesmo que considerarmos que o prêmio de $z_2$ e $z'_2$ têm o mesmo valor esperado que uma loteria $(0.6z_1, 0.4z_4)$ e $z_3$ e $z'_3$ têm o mesmo valor esperado que uma loteria $(0.2z_1, 0.8z_4)$. Então, para simplificar, podemos substituir esses dois pares por suas respectivas loterias equivalentes com o intuito de reduzir o número de variáveis.

Consideremos que os prêmios $(z_1, z_2, z_3, z_4)$ seguem a seguinte ordem de preferência: $z_1 \succ z_2 \succ z_3 \succ z_4$.

- Equivalência de loterias $L \sim L^{ \sim }$.

  - **Cálculos:**

    - $L^{ \sim } =$
      - $(0.25z_1, 0.25(0.6z_1 + 0.4z_4), 0.25(0.2z_1 + 0.8z_4), 0.25z_4)$
      - $(0.25z_1, 0.15z_1 + 0.10z_4, 0.05z_1 + 0.20z_4, 0.25z_4)$
      - $(0.25z_1 + 0.15z_1 + 0.05z_1, 0.10z_4 + 0.20z_4 + 0.25z_4)$
      - $(0.45z_1, 0.55z_4)$
    - $L'^{ \sim } =$
      - $(0.15z_1, 0.50(0.6z_1 + 0.4z_4), 0.15(0.2z_1 + 0.8z_4), 0.20z_4)$
      - $(0.15z_1, 0.30z_1 + 0.20z_4, 0.03z_1 + 0.12z_4, 0.20z_4)$
      - $(0.15z_1 + 0.30z_1 + 0.03z_1, 0.20z_4 + 0.20z_4 + 0.12z_4)$
      - $(0.48z_1, 0.52z_4)$

- **Critério:** Utilidade esperada: $E(L) = \sum_{i=1}^n p_i u(z_i)$

  - **Cálculos:**
    - $E(L^{ \sim }) = 0.45 u(z_1) + 0.55 u(z_4)$
    - $E(L'^{ \sim }) = 0.48 u(z_1) + 0.52 u(z_4)$
  - **Resultado:**
    - $\begin{cases}
      L^{ \sim } \succ L'^{ \sim } & \text{if } E(L^{ \sim }) > E(L'^{ \sim }) \\
      L'^{ \sim } \succ L^{ \sim } & \text{if } E(L^{ \sim }) < E(L'^{ \sim }) \\
      L^{ \sim } \sim L'^{ \sim } & \text{if } E(L^{ \sim }) = E(L'^{ \sim }) \\
      \end{cases}$

- **Critério:** preferência pelo mais provável: $L \succ L' \rightarrow \max_z L(z) > \max_z L'(z)$

  - **Cálculos:**
    - $\begin{cases}
      L \succ L' & \text{if } \max_z L(z) > \max_z L'(z) \\
      L' \succ L & \text{if } \max_z L(z) < \max_z L'(z) \\
      L \sim L' & \text{if } \max_z L(z) = \max_z L'(z) \\
      \end{cases}$
    - $\max_z L(z) > \max_z L'(z)$
      - $z_1 > z_2: verdadeiro$
      - **Explicação:** o mais provável de $L$ é preferível ao mais provável de $L'$.
      - **Resultado:** $L \succ L'$.
    - $\max_z L^{\sim}(z) > \max_z L'^{\sim}(z)$
      - $z_4 > z_4: falso$
      - **Explicação:** o mais provável de $L^{\sim}$ é tão preferível quanto o mais provável de $L'^{\sim}$.
      - **Resultado:** Como os mais prováveis de $L^{\sim}$ e $L'^{\sim}$ são equivalentes, podemos considerar que $L^{\sim} \sim L'^{\sim}$. Ou, se considerarmos que $p(L^{\sim}(\max_z L^{\sim}(z))) > p(L'^{\sim}(\max_z L'^{\sim}(z)))$, podemos considerar que $L^{\sim} \succ L'^{\sim}$.

---

### 9. T or F. Justify or give a counterexample

#### 9.1 A lottery $p$ is preferred to $q$ because the expected utility $U(p)$ is greater than the expected utility $U(q)$

##### Resposta 9.1

#### 9.2 Suppose that $A \succ B \succ C \succ D$ and that the vNM utilities of these prizes satisfy $v(A) + v(D) = v(B) + v(C)$, then $(\frac{1}{2}B, \frac{1}{2}C)$ should be preferred to $(\frac{1}{2}A, \frac{1}{2}D)$ because, although they have the same expected utility, the former has the smaller utility variance

##### Resposta 9.2

#### 9.3 Suppose that $A \succ B \succ C \succ D$ and that the vNM utility function has the property that $v(A) - v(B) \succ v(C) - v(D)$, then the change from $B$ to $A$ is more preferred than the change from $D$ to $C$

##### Resposta 9.3

### 10. Verify whether each of the following preference relations over lotteries satisfy (or not) von Neumann and Morgenstern axioms (I and C). Consult the book "Lecture Notes in Microeconomic Theory" by Ariel Rubinstein, Pages 95 and 96, for more details

#### 10.1. The worst case (the decision maker evaluates lotteries by the worst possible case)

##### Resposta 10.1

#### 10.2. Increasing the probability of a "good" consequence

##### Resposta 10.2

## Risk Aversion

### 11. Adam lives in the Garden of Eden and eats only apples. Time in the garden is discrete ($t = 1, 2, \dots$) and apples are eaten only in discrete units. Adam possesses preferences over the set of streams of apple consumption. Assume that

> 1. Adam likes to eat up to 2 apples a day and cannot bear to eat 3 apples a day.
> 2. Adam is **impatient**. He would be delighted to increase his consumption on day $t$ from 0 to 1 or from 1 to 2 apples at the expense of an apple he is promised a day later $t+1$.
> 3. In any day in which he does not have an apple, he prefers to get 1 apple immediately in exchange for 2 apples tomorrow.
> 4. Adam expects to live for 120 years.
>
> Show that if (poor) Adam is offered a stream of 2 apples starting in day 4 for the rest of his expected life, he would be willing to exchange that offer for 1 apple right away.
>
> _Tips:_
>
> - (2) means that one single apple is promised to Adam on day $t+1$
> - initial stream offered to Adam can be represented by $(0,0,0,2,2,...,2,2)$
> - evolve it due to Adam’s preferences

#### Resposta 11

#### 12. Given the pairs of lotteries in tables 1 and 2, in each case, which one do you prefer? Explain considering the First-Order Stochastic Domination concept

##### 12.1 **Table 1:** (a) or (b)?

| chance % | 90  | 6    | 1     | 3     |
| -------- | --- | ---- | ----- | ----- |
| (a)      | $0$ | $45$ | $30$  | $-15$ |
| (b)      | $0$ | $45$ | $-10$ | $-15$ |

###### Resposta 12.1

##### 12.2 **Table 2:** (c) or (d)?

| chance % | 40  | 35   | 15   | 10    |
| -------- | --- | ---- | ---- | ----- |
| (c)      | $0$ | $10$ | $50$ | $200$ |
| (d)      | $0$ | $25$ | $40$ | $180$ |

###### Resposta 12.2

#### 13. A gambling house charges $15 for the lottery below

| prize | $0$    | $36$   | $64$   |
| ----- | ------ | ------ | ------ |
| $p$   | $0.50$ | $0.30$ | $0.20$ |

> Will a person, whose utility function over money is $u(x) = \frac{5}{4}\sqrt{x}$, pay to play $p$? Justify your answer.

##### Resposta 13
