# P2

- Questão da prova: Lemke Howson
- Forma extensiva
- questão com Beta(?)

## Lemke Howson: algoritmo - [Áudio P1][P1]

- Calcula utilidades esperadas
- Jogador linha, pega todas as utilidades esperadas
- Gera as equações em função da Slack Variable
- Mantém a utilidade que desejamos alcançar como 1, e o resto será 1 - as outras utilidades esperadas
- Temos os sistemas de equações lineares e escolhemos qual queremos
- Passamos da equação pra base
- Ao passarmos pra base, reescreve as outras equações em função disso

### Lemke Howson: algoritmo (continuação) - [Áudio P2][P2]

- Fazemos isso até todos os labels serem representados pelo sistema
- Que é quando todos os labels estiverem na base, assim encontrando um equilíbrio de Nash
- Então zera tudo do lado direito, e as probabilidades soma e normaliza.

## Jogos na Forma Extensiva: Jogos sequenciais - [Áudio P3][P3]

- É um jogo na forma sequencial, que é diferente da simultaneidade da forma normal
- Podemos transformar um no outro.

### Jogos na Forma Extensiva: _Non-credible Threats_ e _sub-perfect equilibrium_ - [Áudio P4][P4]

- Dá para encontrar equilíbrios de Nash que não são críveis (Non-Credible Threats)
- É quando um jogador em um nó mais profundo escolhe uma ação que não maximiza sua utilidade, mas que ameaçada os jogadores anteriores.
- Um caso clássico é o da competição de empresas.
  - A empresa A ameaça a empresa B de entrar no mercado, mas na verdade não entraria, pois não é lucrativo.
- Essa definição não é muito razoável, pois o jogador não toma a ação que maximiza sua utilidade.
- Temos então a definição de sub-perfect equilibrium:
  - Analisamos cada sub-game fazendo o backward induction, e verificamos cada subgame do mais profundo para o mais raso.
  - Basicamente fazendo com que cada jogador escolha sua melhor resposta.
  - O sub-perfect equilibrium é um equilíbrio de Nash mas nem todo equilíbrio de Nash é sub-perfect equilibrium.

### Jogos na Forma Extensiva: _imperfect information_ e _information set_ [Áudio P5][P5]

- E quando o jogo não tem perfect-recall? (O jogo é de imperfect information)
  - Ou seja, o jogador não sabe qual ação o outro jogador tomou.
- Com isso podemos converter todos os Jogos da forma normal para a forma extensiva.
- Information Set: conjunto de nós em que as escolhas são indistinguíveis para o jogador, mesmo que os payoffs sejam diferentes.

### Jogos na Forma Extensiva: coligações, _payoffs_ futuros e traição - [Áudio P6][P6]

- Ao modelar agentes reais, os jogos presentes tendem a ter mais valor que os jogos futuros. Então teremos um fator $\beta$ que é o desconto do futuro e que tendendo ao tempo $\infty$, $\beta$ se torna 0.
- As empresas podem fazer uma coligação para maximizar seu lucro cooperativo.
- Porém, pode-se calcular o ganho de desvio, isso porque não sabemos qual que é o momento em que o jogo encerrará.

<!-- Links -->

[P1]: 20250630-Rangel-Lemke_Howson-P1-2min09s.opus
[P2]: 20250630-Rangel-Lemke_Howson-P2-0min34s.opus
[P3]: 20250630-Rangel-Lemke_Howson-P3-0min36s.opus
[P4]: 20250630-Rangel-Lemke_Howson-P4-2min11s.opus
[P5]: 20250630-Rangel-Lemke_Howson-P5-1min48s.opus
[P6]: 20250630-Rangel-Lemke_Howson-P6-2min31s.opus
