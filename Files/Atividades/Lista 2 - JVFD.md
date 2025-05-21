# Lista 2 - 6.11 Exercises

## Conteúdos

- Equilíbrio de Nash
  - Estratégia Pura: [1, 3, 10b, 10c]
    - Encontrar todos os equilíbrios puros: [4b, 5, 6a, 6b, 8a, 12a, 13a, 13b, 15d]
  - Encontrar todos os equilíbrios: [6c, 7a, 7b, 9, 10a, 14a]
  - Estratégia Mista: [8b, 14b, 15c?, 15e?]
- Schelling's focal point [8c]
- "Social-Welfare maximizing": [2]
- Matriz de payoffs
  - Construir: [15a]
  - Avaliar: [15b]
- Dominância de estratégias
  - Dominante: [4a]
  - Dominada: [11]
  - Fracamente dominada: [12a]

## 1. Say whether the following claim is true or false, and provide a brief (1-3 sentence) explanation for your answer

**Claim:** If player $A$ in a two-person game has a dominant strategy $s_A$, then there is a pure strategy Nash equilibrium in which player $A$ plays $s_A$ and player $B$ plays a best response to $S_A$.

**Resposta:** Se considerarmos que a estratégia $S_A$ é estritamente dominante para o jogador $A$, logo, não haverá outra estratégia para o jogador $A$ que resulte em maior Payoff, isso, independente da escolha do jogador $B$. Sendo assim, o jogador $B$ deve escolher a melhor resposta para a estratégia $S_A$. Com isso, há um Equilíbrio de Nash de Estratégia Pura.

---

## 2. Consider the following statement

> In a Nash equilibrium of a two-player game each player is playing an optimal strategy, so the two player's strategies are social-welfare maximizing.

Is this statement correct or incorrect? If you think it is correct, give a brief (1-3 sentence) explanation for why. If you think it is incorrect, give an example of a game discussed in Chapter 6 that shows it to be incorrect (you do not need to spell out all the details of the game, provided you make it clear what you are referring to), together with a brief (1-3 sentence) explanation.

- **Resposta:** A afirmação é incorreta. Um exemplo disso é o Dilema do Prisioneiro, onde ambos os jogadores têm uma estratégia dominante de trair o outro, resultando em um equilíbrio de Nash. No entanto, essa escolha não maximiza o bem-estar social, pois ambos os jogadores teriam um resultado melhor se cooperassem. Portanto, a estratégia ótima para cada jogador não leva ao resultado socialmente ótimo.

- **Dúvidas:**
  - O que seria "social-welfare maximizing"? É o mesmo que "Pareto Dominante"?
  - A estratégia ótima é a que maximiza o payoff de cada jogador?

---

## 3. Find all pure strategy Nash equilibria in the game below. In the payoff matrix below the rows correspond to player $A$'s strategies and the columns correspond to player $B$'s strategies. The first entry in each box is player $A$'s payoff and the second entry is player $B$'s payoff

|   3   |    $B:L$     |    $B:R$     |
| :---: | :----------: | :----------: |
| $A:U$ |   1, **2**   | **3**, **2** |
| $A:D$ | **2**, **4** |     0, 2     |

- **Equilíbrio de Nash de Estratégia Pura:** $\{\{D, L\}, \{U, R\}\}$

- **Justificativa:**
  - $L$ Domina fracamente $R$ pois os payoffs de $L$ são pelo menos tão bons quanto os resultados de $R$; sendo assim, o jogador $B$ jogará $L$; Sabendo disso, o jogador $A$ escolherá a opção que lhe render maior payoff, dada a escolha de $L$, sendo essa a estratégia $D$.
  - E no caso do $U, R$, caso o $A$ jogue $U$, pro $B$ tanto faz se ele jogar $L$ ou $R$. E se $B$ jogar $R$, a melhor estratégia de $A$ é jogar $U$.

---

## 4. Consider the two-player game with players, strategies and payoffs described in the following game matrix

| 4     |    $B:L$     |  $B:M$   |  $B:R$   |
| :---- | :----------: | :------: | :------: |
| $A:t$ |   0, **3**   | **6**, 2 |   1, 1   |
| $A:m$ |   2, **3**   |   0, 1   | **7**, 0 |
| $A:b$ | **5**, **3** |   4, 2   |   3, 1   |

Figure 6.28: Payoff Matrix

### **(a)** Does either player have a dominant strategy? Explain briefly (1-3 sentences)

- **Resposta:** O jogador $A$ não tem uma estratégia dominante. Já o jogador $B$ tem uma estratégia dominante, que é $L$, pois essa estratégia domina estritamente as outras duas, $M$ e $R$, visto que seus payoffs são sempre maiores que as alternativas. Como então o jogador $B$ tenderá a jogar $L$, o jogador $A$ escolherá a melhor resposta para essa estratégia, que é $b$, mesmo que isso não seja uma estratégia dominante para si.

### **(b)** Find all pure strategy Nash equilibria for this game

- **Resposta:** O equilíbrio de Nash de estratégia pura é $\{\{b, L\}\}$.

## 5. Consider the following two-player game in which each player has three strategies

| 5     |   $B:L$   |    $B:M$     |  $B:R$   |
| :---- | :-------: | :----------: | :------: |
| $A:U$ |   1, 1    |     2, 3     | 1, **6** |
| $A:M$ | **3**, 4  | **5**, **5** | **2**, 2 |
| $A:D$ | 1, **10** |     4, 7     |   0, 4   |

Find all the (pure strategy) Nash equilibria for this game.

- **Resposta:** O equilíbrio de Nash de estratégia pura é $\{\{M, M\}\}$.

## 6. In this question we will consider several two-player games. In cach payoff matrix below the rows correspond to player $A$'s strategies and the columns correspond to player $B$'s strategies. The first entry in each box is player $A$'s payoff and the second entry is player $B$'s payoff

**(a)** Find all pure (non-randomized) strategy Nash equilibria for the game described by the payoff matrix below.

|  6a   |  $B:L$   |     $B:R$     |
| :---: | :------: | :-----------: |
| $A:U$ |  2, 15   |   4, **20**   |
| $A:D$ | **6**, 6 | **10**, **8** |

**(b)** Find all pure (non-randomized) strategy Nash equilibria for the game described by the payoff matrix below.

|  6b   |    $B:L$     |  $B:R$   |
| :---: | :----------: | :------: |
| $A:U$ | **3**, **5** | **4**, 3 |
| $A:D$ |     2, 1     | 1, **6** |

**(c)** Find _all_ Nash equilibria for the game described by the payoff matrix below.

|  6c   |    $B:L$     |    $B:R$     |
| :---: | :----------: | :----------: |
| $A:U$ |     1, 1     | **4**, **2** |
| $A:D$ | **3**, **3** |     2, 2     |

> Hint: This game has a both pure strategy equilibria and a mixed strategy equilibrium. To find the mixed strategy equilibrium let the probability that player $A$ uses strategy $U$ be $p$ and the probability that player $B$ uses strategy $L$ be $q$. As we learned in our analysis of matching pennies, if a player uses a mixed strategy (one that is not really just some pure strategy played with probability one) then the player must be indifferent between two pure strategies. That is the strategies must have equal expected payoffs. So, for example, if $p$ is not $0$ or $1$ then it must be the case that $q+4(1-q) = 3q+2(1-q)$ as these are the expected payoffs to player A from U and D when player $B$ uses probability $q$.

## 7. In this question we will consider several two-player games. In each payoff matrix below the rows correspond to player $A$'s strategies and the columns correspond to player $B$'s stratcgics. The first entry in cach box is player $A$'s payoff and the socond entry is player $B$'s payoff

**(a)** Find all Nash equilibria for the game described by the payoff matrix below,

|  7a   |  $B:L$   |    $B:R$     |
| :---: | :------: | :----------: |
| $A:U$ | **1**, 1 |   3, **2**   |
| $A:D$ |   0, 3   | **4**, **4** |

**(b)** Find all Nash equilibria for the game described by the payoff matrix below (include an explanation for your answer).

|  7b   |  $B:L$   |   $B:R$   |
| :---: | :------: | :-------: |
| $A:U$ | **5**, 6 | 0, **10** |
| $A:D$ | 4, **4** | **2**, 2  |

> Hint: This game has a mixed strategy equilibrium. To find the equilibrium let the probability that player $A$ uses strategy $U$ be $p$ and the probability that player $B$ uses strategy $L$ be $q$. As we learned in our analysis of matching pennies, if a player uses a mixed strategy (one that is not really just some pure strategy played with probability one) then the player must be indifferent between two pure strategies. That is, the strategies must have equal expected payoffs. So, for example, if $p$ is not $0$ or $1$ then it must be the case that $5q + 0(1 — q) = 4q + 2(1 — q)$ as these are the expected payoffs to player A from U and D when player $B$ uses probability $q$.

## 8. Consider the two-player game described by the payoff matrix below

|   8   |    $B:L$     |    $B:R$     |
| :---: | :----------: | :----------: |
| $A:U$ | **1**, **1** |     0, 0     |
| $A:D$ |     0, 0     | **4**, **4** |

### **(a)** Find all pure-strategy Nash equilibria for this game

Estratégias Puras que são Equilíbrios de Nash: $\{ \{U, L\}, \{D, R\} \}$

**Raciocínio:** olhando como A, se o B jogar L, não há escolha melhor do que U; Olhando como B, se o A jogar U, não há escolha melhor do que L.

---

### **(b)** This game also has a mixed-strategy Nash equilibrium; find the probabilities the players use in this equilibrium, together with an explanation for your answer

Para encontrar o equilíbrio de estratégia mista, precisamos igualar os payoffs esperados de cada jogador para cada estratégia. Primeiro consideremos a probabilidade dos payoffs esperados para o jogador 1

- $1$:
  - $Pay_{A:UL} \cdot P_{B:L} + Pay_{A:UR} \cdot P_{B:R} = Pay_{A:DL} \cdot P_{B:L} + Pay_{A:DR} \cdot P_{B:R}$
    - $Pay_{A:UL} = 1; Pay_{A:UR} = 0; Pay_{A:DL} = 0; Pay_{A:DR} = 4$
    - $P_{B:L} = x; P_{B:R} = 1-x$
    - $1 \cdot x + 0 \cdot (1-x) = 0 \cdot x + 4 \cdot (1-x)$
    - $x = 4(1-x)$
    - $x = 4 - 4x$
    - $5x = 4$
    - $x = \frac{4}{5}$
    - $x = 0.8$
- $2$:
  - $Pay*{B:UL} \cdot P*{B:

$A: x(U) + (1-x)(D)$

$B: y(L) + (1-y)(R)$

| 8b  | L           | R            |
| --- | ----------- | ------------ |
| U   | $UL_1,UL_2$ | $UR_1, UR_2$ |
| D   | $DL_1,DL_2$ | $DR_1, DR_2$ |

---

**(c)** Keeping in mind Schelling's focal point idea from Chapter 6, what equilibrium do you think is the best prediction of how the game will be played? Explain.

## 9. For each of the following two player games find all Nash equilibria. In each payoff matrix below the rows correspond to player $A$'s strategies and the columns correspond to player $B$'s strategies. The first entry in each box is player $A$'s payoff and the second entry is player $B$'s payoff

|  a)   |  $B:L$   |    $B:R$     |
| :---: | :------: | :----------: |
| $A:U$ | **8**, 4 | **5**, **5** |
| $A:D$ |   3, 3   |   4, **8**   |

|  b)   |   $B:L$   |   $B:R$   |
| :---: | :-------: | :-------: |
| $A:U$ | **0**, 0  | -1, **1** |
| $A:D$ | -1, **1** | **2**, -2 |

## 10. In the payoff matrix below the rows correspond to player $A$'s strategies and the columns correspond to player $B$'s strategies. The first entry in each box is player $A$'s payoff and the second entry is player $B$'s payoff

|  10   |    $B:L$     |  $B:R$   |
| :---: | :----------: | :------: |
| $A:U$ | **3**, **3** |   1, 2   |
| $A:D$ |   2, **1**   | **3**, 0 |

**(a)** Find all pure strategy Nash equilibria of this game.

**(b)** Notice from the payoff matrix above that Player $A$'s payoff from the pair of strategies $(U, L)$ is 3. Can you change player $A$'s payoff from this pair of strategies to some non-negative number in such a way that the resulting game has _no_ pure-strategy Nash equilibrium? Give a brief (1-3 sentence) explanation for your answer.

> Note that in answering this question, you should only change Player $A$'s payoff for this one pair of strategies $(U, L)$. In particular, leave the rest of the structure of the game unchanged: the players, their strategies, the payoff from strategies other than $(U, L)$, and $B$'s payoff from $(U, L)$.

**(c)** Now let's go back to the original payoff matrix from part **(a)** and ask an analogous question about player $B$. So we're back to the payoff matrix in which players $A$ and $B$ each get a payoff of 3 from the pair of strategies $(U, L)$.

Can you change player $B$'s payoff from the pair of strategies $(U, L)$ to some non-negative number in such a way that the resulting game has no pure-strategy Nash equilibrium? Give a brief (1-3 sentence) explanation for your answer.

> Again, in answering this question, you should only change Player $B$'s payoff for this one pair of strategies $(U, L)$. In particular, leave the rest of the structure of the game unchanged: the players, their strategies, the payoff from strategies other than $(U, L)$, and $A$'s payoff from $(U, L)$.

## 11. In the text we've discussed dominant strategies and noted that if a player has a dominant strategy we would expect it to be used. The opposite of a dominant strategy is a strategy that is dominated. The definition of dominated is

A strategy $s^{*}_{i}$ is _dominated_ if player $i$ has another strategy $s^{'}_{i}$ with the property that player $i$'s payoff is greater from $s^{'}_{i}$ than from $s^{*}_{i}$ no matter what the other players in the game do.

We do not expect a player to use a strategy that is dominated and this can help in finding Nash equilibria. Here is an example of this idea. In this game, $M$ is a dominated strategy (it is dominated by $R$) and player $B$ will not use it.

|  11   |    $B:L$     |  $B:M$   |  $B:R$   |
| :---: | :----------: | :------: | :------: |
| $A:U$ | **2**, **4** |   2, 1   | **3**, 2 |
| $A:D$ |     1, 2     | **3**, 3 | 2, **4** |

So in analyzing the game we can delete $M$ and look at the remaining game

|  11   |    $B:L$     |  $B:R$   |
| :---: | :----------: | :------: |
| $A:U$ | **2**, **4** | **3**, 2 |
| $A:D$ |     1, 2     | 2, **4** |

Now player $A$ has a dominant strategy ($U$) and it is easy to see that the Nash equilibrium of the 2-by-2 game is $(U, L)$. You can check the original game to see that $(U, L)$ is a Nash equilibrium. Of course, using this procedure requires that we know that a dominated strategy cannot be used in Nash equilibrium. [[Note]][Note5]

[Note5]: <> "This is actually true for any number of players. It would also help to know that if we iteratively remove dominated strategies (in any order) and analyze the reduced games we still find the Nash equilibria of the original game. This is also true, but it is a bit more complicated."

Consider any two player game which has at least one (pure strategy) Nash equilibrium. Explain why the strategies used in an equilibrium of this game will not be dominated strategies.

## 12. In Chapter 6 we discussed dominant strategies and noted that if a player has a dominant strategy we would expect it to be used. The opposite of a dominant strategy is a strategy that is dominated. There are several possible notions of what it means for a strategy to be dominated. In this problem we will focus on weak domination

A strategy $s^{*}_{i}$ _weakly dominated_ if player $i$ has another strategy $s^{'}_{i}$ with the property that:

- **(a)** No matter what the other player does, player $i$'s payoff from $s^{'}_{i}$ is at least as large as the payoff from $s^{*}_{i}$, and
- **(b)** There is some strategy for the other player so that player $i$'s payoff from $s^{'}_{i}$ is strictly greater than the payoff from $s^{*}_{i}$.

**(a)** It seems unlikely that a player would use a weakly dominated strategy, but these strategies can occur in a Nash equilibrium. Find all pure (non-randomized) Nash equilibria for the game below. Do any of them use weakly dominated strategies?

|  12a  |    $B:L$     |    $B:R$     |
| :---: | :----------: | :----------: |
| $A:U$ | **1**, **1** |   1, **1**   |
| $A:D$ |     0, 0     | **2**, **1** |

**(b)** One way to reason about the weakly dominated strategies that you should have found in answering the question above is to consider the following sequential game. Suppose that the players actually move sequentially, but the player to move second does not know what the player moving first chose. Player $A$ moves first, and if he chooses $U$, then player $B$'s choice does not matter. Effectively the game is over if $A$ chooses $U$ as no matter what $B$ does the payoff is (1, 1). If player $A$ chooses $D$, then player $B$'s move matters, and the payoff is (0, 0) if $B$ chooses $L$ or $(2, 1)$ if $B$ chooses $R$.

> Note that as $B$ does not observe $A$'s move the simultaneous move game with payoff matrix above is equivalent to this sequential move game.

In this game how would you expect the players to behave? Explain your reasoning.

> The players are not allowed to change the game. They play it once just as it is given above. You may reason from the payoff matrix or the story behind the game, but if you use the story remember that B does not observe $A$'s move until after the game is over.

## 13. Here we consider a game with three players, named 1, 2 and 3. To define the game we need to specify the sets of strategies available to each player; also, when each of the three players chooses a strategy, this gives a triple of strategies, and we need to specify the payoff each player receives from any possible triple of strategies played. Let's suppose that player 1's strategy set is $\{U, D\}$, players 2's strategy set is $\{L, R\}$ and player 3's strategy set is $\{l, r\}$

One way to specify the payoffs would be to write down every possible triple of strategies, and the payoffs for each, A different but equivalent way to interpret triples of strategies, which makes it easier to specify the payoffs, is to imagine that player 3 chooses which of two distinct two-player games players 1 and 2 will play If 3 chooses $l$ then the payoff matrix is

Payoff Matrix $l$:

|  $l$  |        $B:L$        |    $B:R$    |
| :---: | :-----------------: | :---------: |
| $A:U$ | **4**, **4**, **4** | 0, 0, **1** |
| $A:D$ |   0, **2**, **1**   | **2**, 1, 0 |

where the first entry in each cell is the payoff to player 1, the second entry is the payoff to player 2 and the third entry is the payoff to player 3.

If 3 chooses $r$ then the payoff matrix is

Payoff Matrix $r$:

|  $r$  |    $B:L$    |        $B:R$        |
| :---: | :---------: | :-----------------: |
| $A:U$ | **2**, 0, 0 |   1, **1**, **1**   |
| $A:D$ | 1, 1, **1** | **2**, **2**, **2** |

So, for example, if player 1 chooses $U$, player 2 chooses $R$ and player 3 chooses $r$ the payoffs are 1 for each player.

**(a)** First suppose the players all move simultaneously. That is, players 1 and 2 do not observe which game player 3 has selected until after they each chose a strategy. Find all of the (pure strategy) Nash equilibria for this game.

**(b)** Now suppose that player 3 gets to move first and that players 1 and 2 observe player 3's move before they decide how to play. That is, if player 3 chooses the strategy $r$ then players 1 and 2 play the game defined by payoff matrix $r$ and they both know that they are playing this game. Similarly, if player 3 chooses the strategy $l$ then players 1 and 2 play the game defined by payoff matrix $l$ and they both know that they are playing this game.

Let's also suppose that if players 1 and 2 play the game defined by payoff matrix $r$ they play a (pure strategy) Nash equilibrium for that game; and similarly, if players 1 and 2 play the game defined by payoff matrix $l$ they play a (pure strategy) Nash equilibrium for that game. Finally, let's suppose that player 3 understands that this is how players 1 and 2 will behave.

What do you expect player 3 to do and why? What triple of strategies would you expect to see played? Is this list of strategies a Nash equilibrium of the simultaneous move game between the three players?

## 14. Consider the two-player game with players, strategies and payoffs described in the following game matrix

|  14   |  $2:L$   |  $2:R$   |
| :---: | :------: | :------: |
| $1:U$ | 1, **1** | **4**, 0 |
| $1:D$ | **4**, 0 | 3, **3** |

**(a)** Find all of the Nash equilibria of this game.

**(b)** In the mixed strategy equilibrium you found in part **(a)**, you should notice that player 1 plays strategy $U$ more often than strategy $D$. One of your friends remarks that your answer to part **(a)** must be wrong because clearly for player 1 strategy $D$ is a more attractive strategy than strategy $U$. Both $U$ and $D$ give player 1 a payoff of 4 on the off-diagonal elements of the payoff matrix, but $D$ gives player 1 a payoff of 3 on the diagonal while $U$ only gives player 1 a payoff of 1 on the diagonal. Explain what is wrong with this reasoning.

## 15. Two identical firms - let's call them firm 1 and firm 2 must decide simultaneously and independently whether to enter a new market and what product to produce if they do enter the market. Each firm, if it enters, can develop and produce either product A or product B. If both firms enter and produce product A they each lose ten million dollars. If both firms enter and both produce product B, they each make a profit of five million dollars. If both enter and one produces A while the other produces B, then they each make a profit of ten million dollars. Any firm that does not enter makes a profit of zero. Finally, if one firm does not enter and the other firm produces A it makes a profit of fifteen million dollars, while if the single entering firm produces B it makes a profit of thirty million dollars

You are the manager of firm 1 and you have to choose a strategy for your firm.

**(a)** Set this situation up as a game with two players, firms 1 and 2, and three strategies for each firm: produce $A$, produce $B$ or do not enter.

**(b)** One of your employees argues that you should enter the market (although he is not sure what product you should produce) because no matter what firm 2 does, entering and producing product $B$ is better than not entering. Evaluate this argument.

**(c)** Another employee agrees with the person in part **(b)** and argues that as strategy $A$ could result in a loss (if the other firm also produces $A$) you should enter and produce $B$. If both firms reason this way, and thus enter and produce product $B$, will their play of the game form a Nash equilibrium? Explain.

**(d)** Find all the pure strategy Nash equilibria of this game.

**(e)** Another employee of your firm suggests merging the two firms and deciding cooperatively on strategies so as to maximize the sum of profits. Ignoring whether this merger would be allowed by the regulators do you think its a good idea? Explain.
