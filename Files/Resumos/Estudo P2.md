# P2

- Questão da prova: Lemke Howson
- Forma extensiva
- questão com Beta(?)

## LCP (linear complementarity problem): Lemke Howson

- Soma das utilidades esperadas somadas a uma variável de folga (r) é igual a U^{\*}
  - Faz isso pro P1 e P2
- Soma das probabilidades das estratégias de P1 e P2 é igual a 1
- As folgas e as probabilidades são maiores ou iguais a zero
- folga vezes probabilidade são iguais a zero

## Áudios Rangel

### Lemke Howson: algoritmo - [Áudio P1][P1]

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
- Temos então a definição de _sub-perfect equilibrium_:
  - Analisamos cada sub-game fazendo o _backward induction_, e verificamos cada subgame do mais profundo para o mais raso.
  - Basicamente fazendo com que cada jogador escolha sua melhor resposta.
  - O _sub-perfect equilibrium_ é um equilíbrio de Nash mas nem todo equilíbrio de Nash é _sub-perfect equilibrium_.

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
