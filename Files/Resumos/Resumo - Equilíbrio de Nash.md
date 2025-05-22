# Resumo - Equilíbrio de Nash

## Conteúdo

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

## Definições

### Equilíbrio de Nash

- **O que é Equilíbrio de Nash?**

  - Situação em que nenhum jogador pode melhorar seu resultado ao mudar sua estratégia, dado que os outros jogadores mantêm suas estratégias inalteradas.

- **O que é o Equilíbrio de Nash Puro?**

  - Situação em que os jogadores escolhem estratégias puras, ou seja, não há aleatoriedade nas escolhas.

- **O que é o Equilíbrio de Nash Misto?**
  - Situação em que os jogadores podem escolher estratégias mistas, ou seja, aleatoriedade nas escolhas.

### Dominância de Estratégias

- **O que é uma estratégia dominante?**
  - Uma estratégia que sempre resulta em um payoff maior ou igual, independentemente das escolhas dos outros jogadores.

### Pareto Dominância

- **Qual a diferença entre Estratégia Dominante e Pareto Dominante?**
  - Uma estratégia dominante é aquela que sempre resulta em um payoff maior ou igual, independentemente das escolhas dos outros jogadores. Já a Pareto dominante é uma situação em que não é possível melhorar o resultado de um jogador sem piorar o resultado de outro.

---

Exemplo de matriz de payoffs pro dilema dos prisioneiros

| 1x2 | 2:A    | 2:B    |
| --- | ------ | ------ |
| 1:A | -1, -1 | -10, 0 |
| 1:B | 0, -10 | -5, -5 |

- B: Estratégia dominante
- BB: é um Equilíbrio de Nash Puro
- AA $P_\succ$ (Pareto domina) BB

- Pro jogador 1:
  - Reward: AA
  - Sucker: AB
  - Temptation: BA
  - Punishment: BB

## O resto

- Maxmin and minmax strategies
  - **Maxmin:** Maximizar o mínimo payoff próprio possível
  - **Minmax:** Minimizar o máximo payoff possível do oponente
    - Em jogo de soma zero, minimizar o payoff do oponente tende a aumentar o próprio payoff
- Minimax regret
  - **Regret:** Diferença entre o payoff obtido e o payoff que poderia ter sido obtido se o jogador tivesse escolhido a melhor estratégia possível, dado o que os outros jogadores escolheram.
  - **Max Regret:** A máxima diferença entre o payoff obtido e o payoff que poderia ter sido obtido. (Basicamente a diferença entre o maior payoff e o menor payoff de toda a matriz? Dentre as escolhas dos outros jogadores?)
  - **Minimax Regret:** Minimizar o máximo arrependimento possível
- **Removal of dominated strategies:** Sempre remover estratégias estritamente dominadas
- Correlated Equilibrium
- Trembling-hand perfect equilibrium
- ξ-Nash equilibrium
