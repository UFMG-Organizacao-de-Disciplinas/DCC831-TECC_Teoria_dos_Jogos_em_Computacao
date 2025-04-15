# Lista 1

Teoria dos Jogos em Computação

**Professor:** Pedro Olmo Stancioli Vaz de Melo

## Utility

1. Dê um exemplo de preferências sobre um conjunto enumerável no qual as preferências não possam ser representadas por uma função utilidade que retorne apenas valores inteiros.

2. Um fazendeiro quer cavar um poço em um campo quadrado. As preferências do fazendeiro sobre os possíveis locais são lexicográficas, ou seja:

- Se $x_1 < x_2$ então $(x_1, y_1) \succ (x_2, y_2)$ para todo $y_1, y_2$.

- Se $x_1 = x_2 = x$, então $(x, y_1) \succ (x, y_2)$ se, e somente se, $y_1 < y_2$.

Primeiro, assuma que o campo tem dimensões $[0, 1000] \times [0, 1000]$ e construa uma função utilidade linear que representa essa relação. Segundo, construa uma função utilidade assumindo que o campo tem dimensões $[0,\infty) \times [0,\infty)$. Para ambos os casos, assuma que a localização do poço deve ter coordenadas inteiras.

3. A afirmação "se ambas $U$ e $V$ representam $\succeq$, então existe uma função estritamente monótona $f : \mathbb{R} \rightarrow \mathbb{R}$ tal que $V(x) = f(U(x))$" está correta?

*Dica:* considere $V(x) = x$ e

$$
U(x) =
\begin{cases}
x, & \text{se } x \leq 0 \\
x + 1, & \text{se } x > 0
\end{cases}
$$

4. Uma relação de preferência contínua pode ser representada por uma função utilidade descontínua?

5. Mostre que, no caso de $X = \mathbb{R}$, a relação de preferência que é representada pela função utilidade descontínua $u(x) = \text{floor}(x)$ não é uma relação contínua.  
*floor(x):* o maior inteiro $n$ tal que $x \geq n$

---

## Choice

6. As seguintes são descrições de procedimentos de tomada de decisão. Discuta se os procedimentos podem ser descritos no contexto do modelo de escolha discutido neste curso e se são compatíveis com o paradigma do "homem racional". Em outras palavras, é possível construir uma função utilidade $u(x)$ baseada apenas no conjunto de alternativas $x \in X$ de acordo com esses procedimentos? Explique por quê (ex: com um exemplo).

a. O tomador de decisão escolhe uma alternativa para maximizar o sofrimento de outra pessoa.

b. O tomador de decisão pede a seus dois filhos que ranqueiem as alternativas e então escolhe a alternativa que é a melhor em média (você pode usar sua própria definição de “melhor em média”).

c. O tomador de decisão tem um ponto ideal em mente e escolhe a alternativa mais próxima dele.

d. O tomador de decisão procura a alternativa que aparece com mais frequência em uma lista de alternativas.

e. O tomador de decisão tem uma ordenação em mente e sempre escolhe o elemento mediano.

7. Considere o seguinte procedimento de escolha: um tomador de decisão possui uma ordenação estrita $\succeq$ sobre o conjunto $X$ e atribui a cada $x \in X$ um número natural $\text{class}(x)$ a ser interpretado como a "classe" de $x$. Dado um problema de escolha $A$, ele escolhe o melhor elemento de $A$ entre aqueles que pertencem à classe mais comum em $A$ (isto é, a classe que aparece com mais frequência em $A$). Se houver mais de uma classe mais comum, ele escolhe o melhor elemento entre os membros de $A$ que pertencem a uma das classes mais comuns com maior número de classe.

a. Este procedimento é consistente com o paradigma do "homem racional"?

b. Defina a relação: $xPy$ se $x$ é escolhido de $\{x, y\}$. Mostre que a relação $P$ é uma ordenação estrita (completa, assimétrica e transitiva).

---

## Expected Utility

8. Qual loteria você prefere?

- $L = (0.25z_1, 0.25z_2, 0.25z_3, 0.25z_4)$ ou  
- $L' = (0.15z_1, 0.50z_2, 0.15z_3, 0.20z_4)$

Suponha, por continuidade: $z_2 \sim z'_2 = (0.6z_1, 0.4z_4)$ e $z_3 \sim z'_3 = (0.2z_1, 0.8z_4)$

9. Verdadeiro ou falso. Justifique ou forneça um contraexemplo.

a. Uma loteria $p$ é preferida a $q$ porque a utilidade esperada $U(p)$ é maior que a utilidade esperada $U(q)$.

b. Suponha que $A \succ B \succ C \succ D$ e que as utilidades de vNM desses prêmios satisfaçam $v(A) + v(D) = v(B) + v(C)$, então $(\frac{1}{2}B, \frac{1}{2}C)$ deve ser preferida a $(\frac{1}{2}A, \frac{1}{2}D)$ porque, embora tenham a mesma utilidade esperada, a primeira tem menor variância.

c. Suponha que $A \succ B \succ C \succ D$ e que a função utilidade de vNM tenha a propriedade que $v(A) - v(B) \succ v(C) - v(D)$, então a mudança de $B$ para $A$ é mais preferida do que a mudança de $D$ para $C$.

10. Verifique se cada uma das seguintes relações de preferência sobre loterias satisfaz (ou não) os axiomas de von Neumann e Morgenstern (I e C). Consulte o livro *Lecture Notes in Microeconomic Theory* de Ariel Rubinstein, páginas 95 e 96, para mais detalhes.

a. O pior caso (o tomador de decisão avalia loterias pelo pior caso possível).

b. Aumento da probabilidade de uma consequência “boa”.

---

## Risk Aversion

11. Adão vive no Jardim do Éden e come apenas maçãs. O tempo no jardim é discreto ($t = 1, 2, \dots$) e maçãs são comidas apenas em unidades discretas. Adão possui preferências sobre o conjunto de fluxos de consumo de maçã. Assuma que:

a. Adão gosta de comer até 2 maçãs por dia e não suporta comer 3 maçãs por dia.

b. Adão é impaciente. Ele ficaria feliz em aumentar seu consumo no dia $t$ de 0 para 1 ou de 1 para 2 maçãs à custa de uma maçã prometida para um dia depois, $t + 1$.

c. Em qualquer dia em que ele não tenha uma maçã, ele prefere receber 1 maçã imediatamente em troca de 2 maçãs amanhã.

d. Adão espera viver por 120 anos.

Mostre que, se (pobre) Adão for oferecido um fluxo de 2 maçãs a partir do dia 4 pelo restante de sua vida esperada, ele estaria disposto a trocar essa oferta por 1 maçã agora.  
*Dicas:*

- (b) significa que uma única maçã é prometida a Adão no dia $t+1$  
- fluxo inicial oferecido a Adão pode ser representado por $(0, 0, 0, 2, 2, \dots, 2)$  
- evolua isso conforme as preferências de Adão

12. Dadas as duplas de loterias nas Tabelas 1 e 2, em cada caso, qual você prefere? Explique considerando o conceito de *First-Order Stochastic Domination*.

**Tabela 1:** (a) ou (b)?

| chance % | 90 | 6 | 1 | 3 |
|----------|----|---|---|---|
| (a)      | $0$ | $45$ | $30$ | $-15$ |
| (b)      | $0$ | $45$ | $-10$ | $-15$ |

**Tabela 2:** (c) ou (d)?

| chance % | 40 | 35 | 15 | 10 |
|----------|----|----|----|----|
| (c)      | $0$ | $10$ | $50$ | $200$ |
| (d)      | $0$ | $25$ | $40$ | $180$ |

13. Uma casa de apostas cobra $15 pela loteria abaixo:

| prêmio | $0$ | $36$ | $64$ |
|--------|-----|------|------|
| $p$    | $0.50$ | $0.30$ | $0.20$ |

Uma pessoa cuja função utilidade sobre dinheiro é $u(x) = \frac{5}{4}\sqrt{x}$ pagaria para jogar $p$? Justifique sua resposta.
