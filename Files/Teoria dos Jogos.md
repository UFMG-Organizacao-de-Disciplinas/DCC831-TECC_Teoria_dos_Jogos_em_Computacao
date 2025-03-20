# Teoria dos Jogos em Computação - Professor: Pedro Olmo Stancioli Vaz de Melo

## 13/03/2025 - Aula 1

- "Pode mudar completamente o seu jeito de pensar"
- "O lado ruim é que você fica um pouco mais cínico sobre o mundo"
- "Não existe altruísmo. E se existe, é porque ele te fará bem"

- Esse curso é sobre modelagem, porém não necessariamente sobre teoria dos jogos.
  - Conseguir traduzir para conceitos formais problemas reais

- Um competidor deve abrir sua loja ao lado de uma loja franquiada?
- Formas de modelar
  - Competidor:
    - Não abrir a loja: (5, 1)
    - Abrir a loja
      - Chain Store:
        - Coopera: (2,2)
        - Agressiva: (0,0)

A primeira parte do curso falará apenas sobre tomada de decisão. Na segunda, teremos os jogos.

- A teoria dos jogos estudam configurações onde múltiplos jogadores (agentes) têm:
  - Diferentes preferências (funções de utilidade)
  - Diferentes ações que podem tomar

Ao longo do curso, ele distribuirá pontos. Ele dará Game Points aos jogadores que ganharem os jogos. Eles entram como pontos de participação mas, dependendo dá pra se tornar ponto extra caso extrapole os pontos e participação.

- Jogo 1: Escolha um número entre 0 e 100. O que chegar mais perto da média, ganha.
  - 3 números 5;
  - A média foi 42; O rapaz que botou 37 ganhou
- Jogo 2: Escolha o número mais próximo da metade da média
  - O pulo do gato é que a tendência desse jogo é que chega a ser 0.
  - Porque queremos a metade da média. Então deve ser só um número entre 0 a 50; Mas nesse caso, trabalharemos apenas entre 0 a 25; e 0 a 12; e assim por diante.
- Jogo 3: (dois ganhadores) O número que chegar mais próximo à amplitude (maior diferença); O número que chegar mais próximo da média.
  - A média foi próximo de 15 e a amplitude foi perto de 98;

A recompensa de um jogo muitas vezes acaba sendo externa ao contexto do jogo.

Bounded Rationality: pode-se considerar que os agentes trabalharão com limites de racionalidade; talvez por limite de conhecimento; por limite de cognição; etc.

---

[Lembrar de pegar a caneta com o Caio.]

- The action of an agent can influence the action of the others?
  - Se não tiver, não é jogo
- What are the possible Payoffs for each agent?
- Each agent's utility...
- Game theory studies how agents can rationally form beliefs over what other agents will do, and (hence) how agends should act.
  - Useful fora cting as well as predicting behavior of others
- TCP Backoff game
  - Question: should you send your packets using correctly-implemented TCP (which has a "backoff" mechanism) or using a defective implementation (which doesn't)?
  - Esse é um exemplo de jogo de dois jogadores.
  - E é um exemplo da aplicação do dilema dos prisioneiros.
  - [Ele listou algumas perguntinhas interessantes sobre essa dinâmica]

Principais: John Nash e Von Neumann

<http://ncase.me/trust/>

- Onde a teoria dos jogos é aplicada?
  - Economia: Leilões, trocas, preço/quantidade de configuraçõs
  - Ciência política
  - Biologia
  - Filosofia
  - Ciência da Computação:
    - Computer Networks
    - Robotics
    - Computer Vision
    - ...
    - Information Retrieval
    - Distributed Computing
    - Machine Learning
  
- Lei seca: gato e rato

- Types of games:
  - sum zero
  - Cooperation
  - Repeated games
  - Bayesian and Imperfect information games
  - Congestion games
  - Learning and teaching
  - Coalitional games

Chris Moneymaker

Talvez façamos alguns seminários 

- Pre requisitos
  - Inglês
  - Matemática discreta
  - Teoria dos conjuntos básica
  - Teoria da probabilidade básica
  - Noções de algoritmos

- Notas
  - 2 provas
    - Em sua maioria são questões de modelagem
  - Projeto de turma | Listas de exercício | Paticipação | Seminário
    - Projeto de turma
      - Tentativa de fazer um trabalho original aos tópicos relacionados ao curso
      - Teórico ou experimental
      - Criatividade é bem vinda
    - Seminário
  - PD Competition: cada um fazer uma competição de programação com dilema de prisioneiros.
  - Grading
    - 2 provas (25+25)
    - 1 seminário ou projeto de turma (20)
    - 3 listas de exercícios (?)
    - Participação (?)

- Livros
  - Lecture Notes in Microeconomics theory
  - Multiagent systems: Yoav shoham
  - A Course in game theory
  - Games and decision making
  - The compleat Stategyst
  - Networks crowds and markets
  - Alogirthmic Game Theory "Esse livro é pra gente maluca"
  - Games and Decisions - R Duncan
  - Prisoner's Dilemma - William Poundstone
- Cursos
- Papers
  - Freakonomics

---

Goals

- Aprender a modelar cenários de conflitos
- ...
- Tarefa para Domingo

Quem não tem acesso ao moodle: <pedroolmo@gmail.com>

## Aula 2 - 18/03/2025 [JV: Cheguei atrasado]

...

...

...

---

Não tive acesso ao Moodle, e esqueci de pedir. Logo não respondi uma das questões dele.

### Slide???

#### Eazy Questions

#### Procedures that cause violations of transitivity

- Agregation of considerations as a source of intransitivity
  - X = {a, b, c} and the individual has three primitive considerations in mind (eg: price, taste, quality)
  - The individual finds an alternative x better than an alternative y if a majority of considerations supports x
  - If three considerations rank the alternatives as:
    - $A >_1 B >_1 C$
    - $B >_2 C >_2 A$
    - $C >_3 A >_3 B$
  - Com isso:
    - entre A e B: A>B;
    - entre B e C: B>C;
    - entre C e A: C>A;

---

- The use of similarities as an obstacle to transitivity
  - In some cases, an individual may express indifference in a comparison between two elements that are too "close" to be distinguishable
  - Let X be the set...
  - ...

---

#### Preferências

- Definition 1
  - ...

#### A discussion of transitivity

- Is this definition weak?
  - f(y, z) = I [JV: I = indiferente]

#### QUestionnaire R

...

---

...

#### Reminder: relation [JV: ele pulou]

#### Reminder

- $\succsim$: Pelo menos tão bom quanto
- Completude: $x \succsim y$ ou $y \succsim x$ ou $x \sim y$
- Transitividade: $x \succsim y$ e $y \succsim z$ então $x \succsim z$

---

Questionário Q: $\succ$

- $x \succy = (x \succsim y) and (not y \succsim x)$
- $x ~ y = (x \succsim y) and (y \succsim x)$

---

#### Shepard Tone

#### Fun Problem

- Preferência entre loterias

## Aula 3 - 20/03/2025
