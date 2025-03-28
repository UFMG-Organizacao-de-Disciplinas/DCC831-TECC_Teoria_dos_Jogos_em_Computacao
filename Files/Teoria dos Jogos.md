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

## 18/03/2025 - Aula 2 [JV: Cheguei atrasado] - Slide: Aula 2 - Preferences/Modeling Rational Agents

### Modeling Human Behavior

- O que é um modelo (matemático)?
  - Descrição de sistemas usando conceitos e linguagem matemática
    - Ex.: Teoria de filas, grafos, etc.
  - Pode ajudar a explicar:
    - Sistemas
    - Efeitos em diferentes componentes
    - Fazer predições sobre comportamento

---

- O que é teoria dos jogos?
  - Estudo de modelos matemáticos de conflito e cooperação entre tomadores de decisão racionais inteligentes

---

- Como descrever conflitos entre agentes?

### Game Theory

- Modelo de um agente

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

#### Questionnaire R

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

- $x \succ y = (x \succsim y) and (not y \succsim x)$
- $x ~ y = (x \succsim y) and (y \succsim x)$

---

#### Shepard Tone

#### Fun Problem

- Preferência entre loterias

## 20/03/2025 - Aula X - Não teve e foi avisado

## 25/03/2025 - Aula 3

- Questionário Q e R:
  - Q: dados $X$ e $Y$
    - $X \succ Y$ (X é preferível a Y)
    - $Y \succ X$ (Y é preferível a X)
    - $X \sim Y$ (X é indiferente a Y)
  - R: dados $X$ e $Y$
    - R(x, y): $X \succsim Y?$ (X é pelo menos tão preferível a Y?)
      - Sim
      - Não

### Slide 2

#### Reminder: preferences

- DAG (Directed Acyclic Graph)
  - Há um arco de i a j se j é preferível ao i ($j \succ i$)
- Qual o mais preferível?
  - O que não tem arco de saída, ou tem menor quantidade de saída
- Qual o menos preferível?
  - O que não tem arco de entrada
- $k \succ f?$
  - Sim se houver caminho de k a f
  - Senão, não há resposta
- A relação de preferência é transitiva?
  - Sim

Área da IA: Value allignment: busca entender o que você quer.

#### The concept of Utility Representation

- Se o número de alternativas for pequeno, a relação de preferência pode ser uma lista ordenada de melhor pra pior.

---

...

---

- Prefiro o
  - carro mais rápido
  - jogador de basquete mais alto
  - presente mais caro
  - professor que dão notas maiores

---

- Então a definição acaba sendo
  - $x \succsim y$ se $V(x) \geq V(y)$, onde $V: X \to \mathbb{R}$
- No caso do jogador de basquete:
  - $X$: o jogador de basquete
  - $V(X)$: retorna a altura
- Perceba que $x \succsim y$ se $V(x) \geq V(y)$ é... porque
  - a relação de igualdade é transitiva e completa.

---

...

---

- Definição
  - Para dada função **estritamente crescente** $f: \mathbb{R} \to \mathbb{R}$
  - Considerando que $U(x)$ avalia o nível de preferência, ele representa $\succsim$.
  - $V(x) = f(U(x))$
  - Com isso, $V(x)$ também indica o nível de preferência com a mesma ordem

---

#### Existence of a Utility Representation

---

---

- Possiblidade de representações numéricas que carregam significados adicionais
  - a ser preferível a b mais do que c é preferível a d
  - $a \succsim b > c \succsim d$

---

- Lemma
  - Ele pulou por ser trivial

---

- Reminder
  - X é contável e infinito se há uma relação um-pra-um se há relação de X pros naturais
- ...

---

- Claim
  - Se X é contável, então qualquer relação em X pode ser limitado ao intervalo (-1, 1)

#### Preferências Lexicográficas

- São itens descritos e há dada uma preferência para cada um dos itens

---

- k-tupla
- Notações esquisitas. Não entendi direito

Mas basicamente é a ordenação do Notion. São definidos as categorias e ordens de preferência.

---

- Exemplo:
  - $X = [0, 1] \times [0, 1]$
  - Para que a preferência seja X, depois Y. Então...
  - ...

---

- Teorema: $\mathbb{Q} is dense in \mathbb{R}$
  - (Para qualquer intervalo em $\mathbb{R} por menor que seja, dá para preencher os itens de $\mathbb{Q}$)

---

A Preferência lexicográfica funciona quanto temos elementos finitos, mas não quando eles são reais.

## 27/03/2025 - Aula 4 - Choice: LNMT, chapter 3

### Slide Aula 3 - Utilidade

---

#### Reminder: continuous functions

---

$\vdots$

---

#### Continuity of Preferences

A ideia de preferências contínuas é de que em pequenas variações dos itens, a relação de preferência não muda. Ou seja, se $x \succsim y$, então $x + \delta \succsim y$ para um $\delta$ usualmente pequeno.

No caso de uma não-continuidade, ocorreria uma troca de preferência por menor que fosse a variação do item.

E isso apenas ocorre quanto consideramos itens contínuos, não os discretos.


- In economics, the set X is often an infinite subset of a Euclidean space
  - In $\mathbb{R}^1$
    - Ex: gold
  - In $\mathbb{R}^2$
    - Ex: Salário, tempo de férias por ano
  - In $\mathbb{R}^3$
    - Ex: Café, pão e leite

---

- Which one do you prefer?

---

- The basic intuition...

---

- Definition C1
  - A preference relation ($\succsim$) on X is continuous if whenever $a \succ b$ **there are** balls (neighborhood in the relevant topology) $B_a$ and $B_b$ around $a$ and $b$, respectively, such that **for all** $x \in B_a$ and $y \in B_b$, $x \succsim y$.

---

Imagem

---

- Definition C2
  - [JV: é mais abstrato, não precisa se preocupar]

---

---

- Claim:
  - The preference relation $\succsim$ on X satisfies C1 if and only if it satisfies C2.

---

- $\vdots$

---

- Remark #1
  - $\succsim$ on X is represented by a continuous function U, then $\succsim$ is continuous.
  - To see this, note that if $a \succ b$, then $U(a) > U(b)$
  - Let $\epsilon = (U(a)-U(b))/2$
  - by the continuity of U, there is a $\delta > 0$ such that for all x distanced less than $\delta$ from a, $U(x) > U(a) - \epsilon$, and for all y distanced less than $\delta$ from b, $U(y) < U(b) + \epsilon$.
  - Thus, for x and y whitin the balls of radius $\delta$ around a and b, respectively, $x \succ y$

Entendimento: se considerarmos aplicar uma função de utilidade a todos os pontos dentro do raio $\delta$ centrados em **a** e compararmos com todos os pontos dentro do raio $\delta$ centrados em **b**, então todos os valores de utilidade de **a** serão maiores que os de **b**. Logo, a relação de preferência se mantém: $a \succ b$

[JV: falar com ele no final da aula sobre o uso de deltas diferentes que seguiria sendo válido]

Segundo ele, o delta é encontrado entre pares. Aparentemente maximizando o delta em que ainda se mantém a relação de preferência.

---

- Remark #2

#### Debreu's Theorem

- Continuous preferences have a continuous utility representation
- Proof in the book [Muito chata]

### Slide Aula 4 - Choice

#### Choice Functions

...

---

- Where should I do my PhD in Computer Science?

---

...

---

- A **rational agent** considers only the set of alternatives available to him
  - If the alternatives appear in a list, he ignores:
    - The **order** in which they are presented
    - The **number of times** an alternative appears in the list
    - An alternative with a **default status**
- [JV: O agente racional ignorará, mesmo que nós não ignoremos]

---

- **X** = the set of all CS graduate programs in the world
- **A** = the set containing the items I can choose

---

- A **choice function** C assigns to each set A a unique element of A with...

---

- Ex.: C chooses the most...
  - Difficult
  - Close
  - Fun

---

- Where did you go for lunch today?
- Is this your favorite restaurant in the world?
- ...

---

- In some contexts, not all choice problems are relevant
- Therefore we allow that the agent's behavior be defined only on a set D of subsets of X
- We will refer to a pair (X, D) as context
- ...

---

- Agent's behavior as reponse to a questionnaire that contains questions of the following type, one for each $A \in D$:

"A escolha de Sofia"

#### Rational choice functions

- The induced choice function $C_{\succsim}$ assigns to every nonempty set $A \in D$ the $\succsim-best$ element of $A$
  - [JV Dúvida: por que é $\succsim$ e não $\succ$? Isso não acaba abrindo brecha para a existência de empates de preferência?]
    - Sim, mas ignore isso por enquanto

...

#### Rationalizing

- Condition $\alpha$:
  - We say that C satisfies condition $\alpha$ if for any two problems $A, B \in D$, if $A \subset B$ and $C(B) \in A$, then...
  - $C(A) = C(B)$

---

Exemplo de escolha que não satisfaça a condição $\alpha$:

- Second best

[JV: achei meio esquisito. Tenho que entender melhor o que quebra ou não essa condição]

---

---

- Proposition:
  - ...

---

### Falar no final da aula

- Correções
  - Tem um espaço a mais em "The **order** in which they are presented"
  - $A, B \in D$

[JV: falar com ele no final da aula sobre o uso de deltas diferentes que seguiria sendo válido]

planilha de materiais com link dos slides

Perguntar sobre as aulas dele e por que praticamente só teoria dos jogos?

SIGBOVIK

## 01/04/2025 - Aula 5 - Choice: LNMT, chapter 3

## 01/04/2025 - Aula 6

Aula	Data (D/M/A)	Assunto	Material
1	13/03/2025	Course at a glance: what problems are we trying to solve?	
2	18/03/2025	Preferences	LNMT, chapter 1
3	25/03/2025	Utility	LNMT, chapter  2
4	27/03/2025	Choice	LNMT, chapter 3
5	01/04/2025	Choice	LNMT, chapter 3
6	03/04/2025	Expected Utility	LNMT, chapter 7
7	08/04/2025	Risk Aversion	LNMT, chapter 8
8	10/04/2025	Introduction to Game Theory: global view, applications and examples. Formal definition of a game: payoff, strategies, players, pure strategy nash equilibrium, dominant strategies.	MAS, chapter 3; NCM, chapter 6
9	15/04/2025	Mixed strategies Nash equilibrium: definition, examples and evidences in the real world.	MAS, chapter 3; NCM, chapter 6
10	17/04/2025	Alternative solutions: iterated removal of strictly dominated strategies, minimax strategies, minimax theorem of zero sum games, best reponses, correlated equilibrium.	MAS, chapter 3; NCM, chapter 6
11	22/04/2025	Alternative solutions: iterated removal of strictly dominated strategies, minimax strategies, minimax theorem of zero sum games, best reponses, correlated equilibrium.	MAS, chapter 3; NCM, chapter 6
12	24/04/2025	Alternative solutions: iterated removal of strictly dominated strategies, minimax strategies, minimax theorem of zero sum games, best reponses, correlated equilibrium.	MAS, chapter 3; NCM, chapter 6
13	26/04/2025	Alternative solutions: iterated removal of strictly dominated strategies, minimax strategies, minimax theorem of zero sum games, best reponses, correlated equilibrium.	MAS, chapter 3; NCM, chapter 6
14	29/04/2025	The complexity of finding a Nash Equilibrium: zero sum games and PPAD	MAS, chapter 3; NCM, chapter 6
	01/05/2025	feriado	
15	06/05/2025	prova 1	
16	08/05/2025	The complexity of finding a Nash Equilibrium: Lemke-Howson	MAS, chapter 4
17	13/05/2025	The complexity of finding a Nash Equilibrium: Lemke-Howson	MAS, chapter 4
18	15/05/2025	The complexity of finding a Nash Equilibrium: n player games, removal of dominated strategies, and correlated equilibria	MAS, chapter 4
19	20/05/2025	The complexity of finding a Nash Equilibrium: n player games, removal of dominated strategies, and correlated equilibria	MAS, chapter 4
20	22/05/2025	Perfect Information Extensive-form games	MAS, chapter 5
21	27/05/2025	Perfect Information Extensive-form games	MAS, chapter 5
22	29/05/2025	Imperfect Information Extensive-form games	MAS, chapter 5
23	31/05/2025	Imperfect Information Extensive-form games	MAS, chapter 5
24	03/06/2025	Repeated games: repeated prisoner dilemma, finite and infinite repeated games, Folk's theorem, stochastic games	MAS, chapter 6.1
25	05/06/2025	Repeated games: repeated prisoner dilemma, finite and infinite repeated games, Folk's theorem, stochastic games	MAS, chapter 6.1
26	10/06/2025	Bayesian games	MAS, chapter 6.3
27	12/06/2025	Bayesian games	MAS, chapter 6.3
28	14/06/2025	Congestion games	MAS, chapter 6.4
	19/06/2025	feriado	
29	24/06/2025	Congestion games	MAS, chapter 6.4
30	26/06/2025	Prova 2	