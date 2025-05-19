# Teoria dos Jogos em Computação - Professor: Pedro Olmo Stancioli Vaz de Melo - PG2 - DCC831 - Falar sobre SIGKDD

## 13/03/2025 - Aula 01

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

## 18/03/2025 - Aula 02 [JV: Cheguei atrasado] - Slide: Aula 2 - Preferences/Modeling Rational Agents

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

## 20/03/2025 - Aula XX - Não teve e foi avisado

## 25/03/2025 - Aula 03

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

## 27/03/2025 - Aula 04 - Choice: LNMT, chapter 3

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

Second best procedure

---

### Falar no final da aula

- Correções
  - Tem um espaço a mais em "The **order** in which they are presented"
  - $A, B \in D$

[JV: falar com ele no final da aula sobre o uso de deltas diferentes que seguiria sendo válido]

planilha de materiais com link dos slides

Perguntar sobre as aulas dele e por que praticamente só teoria dos jogos?

SIGBOVIK

## 01/04/2025 - Aula 05 - Choice: LNMT, chapter 3

### Rationalizing (Aula 05)

### Dutch Book Arguments

- **Claim**

  - Um agente econômico que não age de acordo com uma função de escolha por maximização não sobreviverá.

- Example

  - Macaco:
    - C({a, c}) = a
    - C({a, b}) = b
    - C({b, c}) = c

- "Money pump argument":
  - Se fulaninho paga uma quantia $\epsilon$ para trocar de A pra B, de B pra C e de C pra A, então ele acaba entrando num loop infinito de pagamentos.

---

...

---

#### What is an alternative

- Assuma o seguinte
  - C({A, B}) = A; C({steak tartare, chicken}) = chicken
  - C({A, B, C}) = B; C({steak tartare, chicken, frog legs}) = steak tartare
- Uma situação em que algo assim faria sentido seriam informações extras sobre o contexto das opções. Exemplo: se um restaurante tem a opção C, então isso torna mais valioso o item A.
- Então, na prática, a situação prática é:
  - $C({A_{\neg C}, B}) = A_{\neg C}$
  - $C({A_{C}, B, C}) = A_{C}$
- E nesse caso, não há violação. Afinal, as opções são distintas entre si.

#### Choice Functions as Internal Equilibria

- What is your favorite movie?

---

Quando há indiferença relacionado ao item máximo, acaba meio que havendo um bug na hora da escolha do mesmo.

Para solucionar isso, ao invés da função de escolha retornar um item, retornará agora um subconjunto que não seja vazio.

---

- $C_{\succsim}(A) = {x \in A | x \succsim y \forall y \in A}$

A Condição $\alpha$ fala especificamente de um item.

---

- **The Weak Axiom of Revealed Preference (WA):**
  - We say that $C$ satisfies WA if whenever $x, y \in A \cap B, x \in C(A)$, and $y \in C(B)$, it is also true that X...
    - $x \in C(B)$
  - The Weak Axiom Trivially...
    - Condition $\alpha$
    - Condition $\beta$

#### The Satisfying Procedure

- How do you proceed when you have yo buy a laptop?

---

- Consider the following "decision scheme"
  - Define as possibilidades
  - Define um threshold de satisfação ($v*$)
  - ...

Foi mencionado sobre esse caso em que ordena-se por valor. Porém, num caso específico, aceita-se um valor maior do que o esperado. Ou seja, não é o primeiro que satisfaz o $v*$ que foi escolhido. Isso se dá porque na verdade o critério de escolha era outro. Era uma outra função de pesos e é isso que causa a ordenação.

#### Choice Functions as Internal Equilibria (Round 2)

- Who would you pick to be your teammate?

O dilema aqui é a falta de contexto que o agente racional poderia ter, assim fazendo com que se torne mais influenciável pelo framing da pergunta.

---

f: frame

Exemplo: a alternativa default ou a ordem das alternativas

---

foi falado sobre uma potencial nova escolha baseada num framing extra colocado às escolhas.

### Psychological Motives Not Included Within the Framework

- ...

...

#### Framing

- An outbreak of diseas is expected to cause 600 deaths in the US

...

---

- Tversky and Kahnemann (1986)

#### Simplifying the choice problem and the use of similarities

- Which roulette do you prefer, a or b?

---

...

## 03/04/2025 - Aula 06 - Expected Utility | LNMT, chapter 7

### Slide: Choice

#### Ainda falando de Choices

#### Psychological Motives Not Included Within the Framework (Aula 06)

##### Simplifying the choice problem and the use of similarities (Aula 06)

#### Reason-Based Choice

- Derp must choose between two universities
  - C({A, B}) = A
  - C({A, B, C}) = B

Por que houve essa mudança:

JV: Ele pode ter mudado o critério de escolha. Ao adicionar o C, ele passou a considerar os critérios $C_3$ e $C_4$ além das preferências $C_1$ e $C_2$ pre-existentes.

Outra: Como ele sabe que várias alternativas o aceitaram, então ele pode considerar que ele é um bom candidato. Logo, ele independe da escolha de universidade.

Existe uma razão interna e subjetiva do agente racional que faz com que ele mude de escolha.

---

Paretto dominância: opções que são objetivamente maiores que outras. Ou seja, não há como ser pior em todos os critérios.

No caso das opções:

- $A = (7, 4)$ poderia ser denominada $C+ = (7, 4)$
- $B = (4, 7)$
- $C = (6, 3)$

---

Conclusão dele: é difícil de conseguir um resultado consistente.

#### Mental Accounting

Ele diz ser muito parecido com o outro, porém com uma conta.

Explicação 1: Como o rapaz perdeu o ticket e precisa comprar dnv, é como se o valor do ticket dobrasse. No segundo caso, a perda do dinheiro nada tem relação com o dinheiro.

Explicação 2: A pessoa já tinha pre-escolhido ir, então acaba tendendo a querer continuar indo ver o filme.

A tendência é que no primeiro caso menos gente diga sim do que o pessoal do segundo caso.

Conclusão dele: é difícil de conseguir um resultado consistente.

---

- The decision makers may conduct...

#### Modeling Choice Procedures

- There is a large body of evidence...

Aqui todas as escolhas têm uma opção padrão.

---

Ao adicionar mais informações podem ser irrelevantes ao tomador de decisão, mas acabam influenciando a escolha.

---

- $c(A, a) = b; c({a_1, a_2, \dots, a_n}, default=a_k) = b | a, b \in A$

---

---

Define-se que $C(A, a)$ será o $\succ$-melhor item de A, considerando que ele será pelo menos tão bom quanto a.

...

---

- Pareto ótimo: Não há nenhuma opção que a **pareto domine**
- Pareto dominância: opções que são objetivamente maiores que outras. Ou seja, não há como ser pior em todos os critérios.

---

- **Buridan's donkey** is a paradox about a donkey that is equally hungry and thirsty, and is placed exactly in the middle of two identical bales of hay and two identical buckets of water. The donkey cannot decide which one to go to first, and thus it dies of hunger and thirst.

---

A **Default bias**

---

Weak Axiom + Default Tendency

##### A Default Bias

###### The Weak Axiom (WA)

Meio confuso isso daqui

###### Default Tendency (DT)

Me parece a mesma coisa que o Default Bias. Não captei legal.

### Slide: aula 5 - Expected Utility

#### Finally, Games

- One-person games :(

#### Lotteries

- To every action there is a consequence...

Escolhas têm consequências.

A correspondência entre ações e consequências são estocásticas

A escolha da ação é vista como se os prêmios fossem as consequências

---

- Z é o conjunto de prêmios (consequências)
- Z é finito.
- A loteria é uma distribuição de probabilidades sobre os prêmios em que a soma das probabilidades iguala a um.

---

## 08/04/2025 - Aula 07 - Risk Aversion | LNMT, chapter 8

### Slide: Expected Utility (Aula 07)

#### Lotteries (Aula 07)

Antes os prêmios eram determinísticos. Agora são probabilísticos

| Escolha | Color      | White | Red | Green | YelloW |
| :-----: | ---------- | ----: | --: | ----: | -----: |
|    A    | Chance (%) |   ... | ... |   ... |    ... |
|    A    | Value      |   ... | ... |   ... |    ... |
|    B    | Chance (%) |   ... | ... |   ... |    ... |
|    B    | Value      |   ... | ... |   ... |    ... |

---

Mas e quando os prêmios não são tão facilmente comparáveis?

---

- $[z]$ é uma loteria degenerada, quando $p(z) = 1$
- Loteria com dois prêmios: $\alpha x \oplus (1 - \alpha) y$

---

- Denote $L(Z)$ ...

Uma relação de preferência degenerada é quando os valores dos prêmios são irrelevantes.

##### Preferências sobre loterias

- Pensemos sobre preferências razoáveis no espaço $L(Z)$
  - O que torna uma loteria maior que outra?

---

- Preference for uniformity
  - O tomador de decisão prefere loterias menos dispersas, onde a dispersão é medida por:
    - $\sum_{Z} (p(z) - \frac{1}{|Z|})^2$
      - Ex.: $Z_1, Z_2, Z_3$ com $p(z) = 1/3$ para cada um deles
      - $(p(Z_1)-\frac{1}{3})^2 + (p(Z_2)-\frac{1}{3})^2 + (p(Z_3)-\frac{1}{3})^2$
    - Dúvida: "Por que não tirar a entropia ao invés da distância?"
      - Resposta: poderia também.
  - Um caso desse seria se uma pessoa quer que suas músicas sejam tocadas aleatoriamente uniformemente, ao invés de haver uma chance grande de recorrentemente ir para uma mesma música.

Nesse caso de preferência por uniformidade $A \succ B$, onde

| Opção |          X |  Red | Green | Yellow | Blue |
| :---: | ---------: | ---: | ----: | -----: | ---: |
|   A   | Chance (%) | 0.25 |  0.25 |   0.25 | 0.25 |
|   B   | Chance (%) | 0.75 |  0.50 |   0.20 | 0.05 |

---

- Preference for most likelihood
  - The decision maker prefers $p \succ q$ if $\max_Z p(z) > \max_Z q(z)$
    - Ou melhor: deseja-se tornar mais previsível o resultado.
    - Ex.: Weather conditions before going out
  - Pega a maior das probabilidades de um, a maior das probabilidades do outro, e vê qual é maior.

---

- The size of the support
  - The decision maker evaluates each lottery by the number of prizes that can be realized with positive probability.
    - $supp(p) = \{z|p(z)>0 \}$
    - Exemplo aluno 1: RPG. Preferir um D20 ao invés de um D6
    - Exemplo aluno 2: Máquina de garra em shopping que tiver maior variedade de prêmios
    - Exemplo Professor: questões com o menor número de alternativas numa prova de múltipla escolha.
  - Obs.: A preferência por tamanho do suporte pode tanto ser pelo maior suporte quanto pelo menor suporte.

---

- Increasing the probability of a "good" outcome
  - The set $Z$ is partitioned into two disjoints sets $G$ and $B$ (Good and Bad), and between two lotteries the decision maker preferes the lottery that yields "good" prizes with higher probability
    - Example:
      - Choosing a route from city A to city B

---

- The worst case
  - The decision maker evaluate lotteries by the worst possible case
  - He attaches a number ...
  - Example
    - Algoritmos de ordenação

---

- Comparing the most likely prize
  - ...
  - Ex.: ...
- Entre o mais provável de um e o mais provável de outro, qual dos prêmios tiver maior valor, é escolhido.

---

- Lexicographic preferences:
  - Prêmios ordenados de $Z_1, \dots, Z_k$, e a loteria $p$ é preferível à $q$ se
    - $(p(Z_1)) \dots$
  - Ex.: Escolha entre cursos próximos

---

- Expected Utility
  - A number $v(z)$ é agregado a cada prêmio, e a loteria $p$ é avaliado de acordo com ao seu valor esperado $v$, de acordo com $\sum_Z p(Z)v(Z)$
  - $p \succsim q if \dots$

---

- The richness of examples calls for the classification of preference relations
- ...

---

- ...
  - Requisito de consistência
  - Procedural aspect of decision making

---

- What are...

##### von Neumann and Morgenstern Axiomatization

- Six Axioms are usually presented
  1. ...
  2. ...
  3. ...
  4. ...
  5. ...
  6. ...

###### An Axiomatic treatment of utility

...

---

- Assumption 1: ...

- Compound Lotteries

- $\oplus_{k=1}^{k} \alpha_k p^k$

Loterias de loterias

```mermaid
flowchart LR
X(())
X -->|| P1
```

- Assumption 2: reduction of compound lotteries

  - Agrega todas as possibilidades das loterias em um só nível através das multiplicações das probabilidades.

- Assumption 3: Continuity
  - Each prize $z_i$ is indiferent to some lottery ticket involving $z_1$ (the best prize) and $z_rr$ (the worst)
  - There exists a number $p$ such that $z_i$ is indifferent to $[pz_1, (1-p)z_r]$
  - And for $Z = \{$1, $0.01, 💀\}$?

Essa parte pode ser quebrada ser os valores forem muito discrepantes

- Assumption 4: ...
- Assumption 5: transitivity
  - Preference and indifference among lotteries (or lottery tickets) are transitive...

---

- From these...

---

- **Assumption 6:** Monotonicity
  - Uma loteria $[p(z_1), (1-p)z_r]$ is preferred or indifferent to $[p'z_1, (1-p')z_r]$ if and only if $p > p'$

---

...

Accept the existence of single-dimensional utility functions whose expected values...

...

---

- I: Independence
  - ...
- C: Continuity

## 10/04/2025 - Aula 08 - Introduction to Game Theory: global view, applications and examples. Formal definition of a game: payoff, strategies, players, pure strategy nash equilibrium, dominant strategies. | MAS, chapter 3; NCM, chapter 6

### Slide: Risk aversion

#### Risk Aversion

---

- $u(Win, Draw) = ok$
- $u(Lose) = grr$

---

Péssima utilidade caso perca. Ótima caso ganhe.

---

Nessa aula, tentaremos converter os prêmios em dinheiro. Premissa essa que é difícil.

---

Se eu apostar uma determinada quantidade de dinheiro no time oposto, então eu igualo a minha satisfação da vitória com a satisfação de ganhar dinheiro da aposta.

- $u(Win, Draw) - x = u(Lose) + (r-1)x$

Esse equilíbrio só funciona se tu conseguir mensurar adequadamente a alegria da vitória do time em dinheiro.

Exemplo: "Quanto tu tá disposto a pagar para garantir a vitória?"

Outra limitação são as odds. O pior caso é se seu time é o azarão.

---

---

#### Lotteries with monetary prize

Nem sempre mensurar é tão trivial.

A relação de preferências entre as loterias é dada pela equação da Expected Utility: $Eu(p) = \sum_{\mathcal{z} \in Z} p(z) u(z)$

---

Tá sendo feito um experimento por aumento de risco.

E também, o equilíbrio entre o aumento do risco, mas uma relacionado aumento também do Expected Utility.

---

Pro dinheiro, chega um ponto em que o aumento do dinheiro recebido chega num cap de utilidade.

"Há algum valor $X_1" que me faça escolher a loteria p ao invés da q?"

Obs.: a p seria a com chance de não ganhar nada. A q seria a com chance de ganhar $X_1$

- St. Petersburg Paradox

---

Se a utilidade for linear, então num St. Petersburg Paradox, seria esperado que o jogador perdesse tudo. E essas seriam as pessoas neutras à risco.

---

Daniel Bernoulli.

O valor de um item, não necessariamente tem relação ao seu preço, mas sim à sua utilidade.

Nos leilões é exatamente isso. É basicamente checar qual é a pessoa que dá maior valor à determinado item.

---

A utilidade de ganhar dinheiro adicional é menor quando se é rico.

---

##### How to measure?

- Linear: neutra a risco
- Curva superior: avessa a risco
- Exponencial: gosta do risco

Primeiro precisamos converter o valor do prêmio em dinheiro. Depois devo fazer uma função de utilidade sobre o dinheiro.

Está meio confuso a diferença entre a utilidade esperada do prêmio, e a utilidade esperada do dinheiro convertido pelo item do prêmio.

---

A conversão do item em dinheiro varia de pessoa pra pessoa.

Valor esperado da loteria é a multiplicação das possibilidades pelos dinheiros convertidos.

- $u(A) \equiv u(\$20)$
- $u(B) \equiv u(\$80)$

Se a pessoa é neutra a risco $E(p) = Eu(p)$.

A utilidade esperada: $Eu(p) =$ probabilidade vezes $u(\$20)$ somado às outras porbabolidades de valores.

Quem for neutro a risco: $E(p) = CE(p) = \$65$

O averso ao risco: $u(E(p)) > Eu(p)$

Se analisarmos a derivada da loteria no ponto da curva de utilidade, tende-se a preferir...

---

Risk averse: $E(p) > CE(p) < \$65$

---

Risk seeking: O dinheiro cada vez vale mais.

##### Claim

vonNeuman = vNM.

Função estritamente côncava:

$f((1 - \alpha)x + \alpha y) > (1 - \alpha)f(x) + \alpha f(y)$

Consideremos que $f()$ é minha função de utilidade.

Estou buscando um valor intermediário entre f(x) e f(y)

$(1 - \alpha)x + \alpha y$ são valores no eixo x entre $x$ e $y$.

$f((1 - \alpha)x + \alpha y)$ são meus valores na curva entre $x$ e $y$

já $(1 - \alpha)f(x) + \alpha f(y)$ seriam os valores no eixo $y$ entre $f(x)$ e $f(y)$. E com isso eu poderia fazer uma reta que sempre estaria abaixo da curva.

$u(E(p)) > Eu(p)$: Risk aversion definition.

## 15/04/2025 - Aula 09 - Mixed strategies Nash equilibrium: definition, examples and evidences in the real world. | MAS, chapter 3; NCM, chapter 6

### Slide: Risk aversion - Aula 09

#### Risk Aversion - Aula 09

| **Probabilidade** | **Prêmio** |
| ----------------: | ---------: |
|               0.5 |         $0 |
|               0.5 |       $100 |

$E(p) = Esperança = 0.5 \* 0 + 0.5 \* 100 = 50$

$Eu(p) = 0.5 \* u(0) + 0.5 \* u(100)$

Onde $u()$ é a função de utilidade.

Se $u()$ for uma função linear, tanto faz utilizar $E(p)$ quanto $Eu(p)$, porém, quando há aversão a risco ou propensão a risco, os valores acabam se alterando.

- Se neutra a risco:
  - $u(E(p)) = Eu(p)$
  - $E(p) = CE(p)$

Existem n situações em que pessoas podem se tornar Risk Seeker. Como por exemplo

- Se propensa a risco:
  - $u(E(p)) > Eu(p)$ <!-- Copilot -->
  - $E(p) > CE(p)$ <!-- Copilot -->

---

- $u(x) = \ln(x)$
- $p = 0.5 * \$20 \oplus 0.5 * \$100$

[Imagens muito úteis e ilustrativas]

Risk Premium: Diferença entre o valor esperado e o valor que a pessoa está disposta a pagar para não correr o risco.

---

Derivada primeira: positiva se o valor tá crescendo.

Derivada segunda: negativa se a taxa com que tá crescendo reduz com o tempo.

- $r_i(x) = -u ''_i(x) / u'_i(x)$
- $r(x)$ is called coefficient...

---

- Relative risk aversion coefficient **rw**
  - $rw(x) = x r(x)$

---

- Absolute Risk Aversion VS Relative Risk aversion

##### Invariance to Wealth

- u must be exponential or linear

##### First-Order Stochastic Domination

Calcula-se o acumulado de todas as probabilidades de se ganhar um valor maior ou igual a determinado valor. E então, compara-se as loterias.

Caso haja pelo menos um acumulado que não seja maior que o outro, então não daria para definir que uma delas é dominada.

### Slide: Class #7 - Parte 1, Introduction on Non Cooperative [...](https://example.com)

#### Motivation

Interferência entre os jogadores.

---

- Internet
  - Trading Agent: "Loop infinito de aumento de preço"

---

#### Game Theory - Aula 09

#### Self-Interested Agents

- Significado
  - Causar dano? Não necessariamente
  - Se preocupa apenas consigo? Não, porque o interesse do agente pode ser ajudar os outros.

---

- Cada agente tem sua própria descrição do mundo que gosta.
- Ele sempre busca agir para gerar esses estados que gosta.

---

- A função de utilidade dá um nível de felicidade aos agentes.
- A incerteza é o que gera essa percepção de loterias

##### Example: friends and enemies

- c: 100
- m: 50
- h: 50

Na prova ele gosta de colocar alguém avessa ao risco.

Nos exemplos usualmente serão pessoas neutras a risco.

## 17/04/2025 - Aula 10 - Alternative solutions: iterated removal of strictly dominated strategies, minimax strategies, minimax theorem of zero sum games, best reponses, correlated equilibrium. | MAS, chapter 3; NCM, chapter 6

### Slide: Não sei qual

...

#### What is a game?

##### Example 1

- Possible outcomes
  - Exam
    - Study: 92
    - Don't study: 80
  - Presentation
    - Both work: 100
    - Only one works: 90
    - No one works: 84

---

Nada fora da matriz é importante pra tomada de decisão.

Curiosamente, existem vários nomes diferentes para os payoffs

---

- A set of Players
- A set of possible strategies
  - [JV] Tudo o que o agente pode fazer.
- A set of payoffs
  - Todos os resultados possíveis para as escolhas possíveis.

#### Games in Normal Form

- Tupla: $(N, A, u)$
  - N: conjunto finito com n jogadores indexados por i
  - A: conjunto de todas as possíveis ações finitas
  - Cada vetor $a = (a_1, \dots, a_n) \in A$ é uma action profile
  - $u = u_1, \dots, u$ são os resultados obtidos por cada um dos jogadores

---

- Programa do 7 e meio do Silvio Santos
  - Participantes acumulam dinheiro ao longo da trivia
  - No final dois líderes dos grupos jogam o dilema do prisioneiro:
    - dois meios: todos os 10 jogadores ganham 1/10 do acumulado
    - dois 7's: Ninguém ganha
    - um meio, um 7: Quem escolheu 7, ganha tudo

#### Reasoning about Behavior in a Game

- ...

---

- Todos os jogadores conhecem toda a estrutura do jogo.
- Muitos estudos sobre informações incompletas.

---

- Racionalidade
  - cada jogador deve maximizar seu próprio payoff
  - Para todo jogador escolher a estratégia ótima, às vezes é necessário muito tempo e/ou muito raciocínio

##### Reasoning about Behavior in the Exam-or-Presentation Game

Em todo caso, é melhor escolher exame.

#### Strictly dominating strategy

É aquela que dá o melhor resultado pros dois jogadores.

No caso do jogo anterior, o problema é que, embora em todos os casos aparentemente escolher Exame seja melhor, ainda assim, esse estado é paretto dominado por outro (onde ambos escolhem presentation)

#### The Prisoner's Dilemma

- Nash Bargaining Solution
  - Viram o valor de venda e compra de um carro na concessionária
  - Ao invés de fazer o negócio com a concessionária, eles pegaram metade da diferença, então cada uma ganha/deixa de perder metade desse delta.

---

- Honor among thieves

| X      |  Sticks |  Cheats |
| ------ | ------: | ------: |
| Sticks |  (B, A) | (0, AB) |
| Cheat  | (AB, 0) |  (A, B) |

Estratégia dominante: cheat.

---

- **Flood Dresher's Experiment**
  - Armen Alchian VS John D. Williams

| X              | JW (Cooperate) | JW (Defect) |
| -------------- | -------------: | ----------: |
| AA (Cooperate) |     (..., ...) |     (-1, 2) |
| AA (Defect)    |     (..., ...) |    (0, 1/2) |

---

Nem sempre é fácil sincronizar as escolhas

---

Uma grande dificuldade é balancear a cooperação com os interesses individuais.

---

Dilema dos Prisioneiros Iterado: estratégia: tit for tat

Rock of dove

- Exemplos:

  - Jogadores: EUA vs URSS
  - Ações: Criar ou não Bomba Atômica
  - Payoffs: guerra fria, etc.

- Real-world situations
  - Performance enhancing drugs in sports
  - Armed race
  - Lixo na rua

## 22/04/2025 - Aula 11 - Alternative solutions: iterated removal of strictly dominated strategies, minimax strategies, minimax theorem of zero sum games, best reponses, correlated equilibrium. | MAS, chapter 3; NCM, chapter 6

Faltei

## 24/04/2025 - Aula 12 - Alternative solutions: iterated removal of strictly dominated strategies, minimax strategies, minimax theorem of zero sum games, best reponses, correlated equilibrium. | MAS, chapter 3; NCM, chapter 6

## 29/04/2025

### Best Response

- Definindo as estratégias dos outros jogadores, será a melhor resposta para um determinado conjunto de estratégias dos outros jogadores.
- $s_i*$: é a melhor estratégia a ser feita
- $s_{-i}$: As estratégias de todos os outros tirando o indivíduo em questão
- $s_i$ é a estratégia do jogador $i$
- $S_i$: é o conjunto de estratégias disponíveis para o jogador $i$

---

- Strategy Profile: são estratégias tomadas pelos jogadores.
- Action Profile: Um action profile é um strategy profile; Uma ação é uma ação única tomada, ou então, um conjunto de ações tomadas.

---

A melhor resposta é a que me gera maior payoff.

---

- Best Responses are unique?

---

- Best Response is **not** a solution concept

#### Nash Equilibrium

- O Equilíbrio de Nash ocorre quando todos os jogadores estão jogando as melhores escolhas dadas as outras estratégias escolhidas pelos jogadore.s

##### Jogo dos 3 clientes

|  X  |  A  |  B  |  C  |
| :-: | :-: | :-: | :-: |
|  A  | 4,4 | 0,2 | 0,2 |
|  B  | 0,0 | 1,1 | 0,2 |
|  A  | 0,0 | 0,2 | 1,1 |

Esse jogo acaba sendo uma loteria, mas cujas probabilidades são definidas pelas estratégias dos jogadores.

Equilíbrio de Nash: (A, A)

##### Defining Nash Equilibrium

- Se uma escolha pareto domina todas as outras, ela é um Equilíbrio de Nash

##### Pure Strategy Nash Equilibrium

|  X  |   C    |     D      |
| :-: | :----: | :--------: |
|  C  | -1, -1 |   -4, 0    |
|  D  | 0, -4  | **-3, -3** |

|   X   | Left | Right |
| :---: | :--: | :---: |
| Left  |  1   |   0   |
| Right |  0   |   1   |

|  X  |  B   |  F   |
| :-: | :--: | :--: |
|  B  | 1, 2 | 0, 0 |
|  F  | 0, 0 | 2, 1 |

Jogos de soma zero não tem equilíbrio de nash em estratégias puras?

|   X   | Heads | Tails |
| :---: | :---: | :---: |
| Heads |   1   |  -1   |
| Tails |  -1   |   1   |

A soma dos payoffs é zero no jogo de soma zerlo

---

- How to find

---

Pergunta de prova: Equilíbrio de Nash Estrito

Equilíbrio de Nash Fraco: existe ao menos uma resposta equivalentes de equilíbrio.

##### Fun Game

|  X  |   L    |   R    |
| :-: | :----: | :----: |
|  T  | 80, 40 | 40, 80 |
|  B  | 40, 80 | 80, 40 |

|  X  |      L      |   R    |
| :-: | :---------: | :----: |
|  T  | **320, 40** | 40, 80 |
|  B  |   40, 80    | 80, 40 |

|  X  |     L      |   R    |
| :-: | :--------: | :----: |
|  T  | **44, 40** | 40, 80 |
|  B  |   40, 80   | 80, 40 |

## 26/04/2025 - Aula 13 - Alternative solutions: iterated removal of strictly dominated strategies, minimax strategies, minimax theorem of zero sum games, best reponses, correlated equilibrium. | MAS, chapter 3; NCM, chapter 6

### Mixed Strategies

- Análise de chutes de penalti: Esquerda, Direita, Centro
  - $u_i (s) =$ empirical probability of winning

| Kicker/Goalie | Left (p) | Right (1-p) |
| ------------: | -------: | ----------: |
|      Left (q) | .58, .42 |    .95, .05 |
|   Right (1-q) | .93, .07 |    .70, .30 |

O equilíbrio de Nash na estratégia mista é encontrado ao se igualar os payoffs de esquerda e direita para determinada probabilidade:

$$
\begin{cases}
  u_1(l) = p \cdot 0.58 + (1 - p) \cdot 0.95 \\
  u_1(r) = p \cdot 0.93 + (1 - p) \cdot 0.70
\end{cases}
$$

- Então, para $p=0.38$, conseguimos $q=0.42$

|      X       | Goalie Left | Goalie Right | Kicker Left | Kicker Right |
| :----------: | :---------: | :----------: | :---------: | :----------: |
|  Nash Freq.  |     .42     |     .58      |     .38     |     .62      |
| Actual Freq. |     .42     |     .58      |     .40     |     .60      |

---

- Do people randomize well over time?
- And under pressure?
- Minimax é uma estratégia pra jogos de soma zero.

---

- Equilíbrio de Nash em pedra papel tesoura:
  - $R = 1/3$
  - $P = 1/3$
  - $S = 1/3$
- No experimento chinês, os jogadores que perceberam a maior tendência a manter, ganhavam.

---

- Nas estratégias mistas:
  - Os jogadores recebem combinações lineares entre seus valores de utilidade
  - E no geral são sempre por preferência de loterias

### Slide: Mixed Strategies Part 2

#### Maxmin and minmax

##### Maxmin

- Maxmin: o jogador tenta maximizar o seu payoff mínimo

  - $arg max_{s_i} \min_{s_i} u_i(s_i, s_{-i})$
  - $max_{s_i} \min_{s_i} u_i(s_i, s_{-i})$

Obs.: esse Arg serve pra retornar o $s_i$, nesse caso a estratégia. Enquanto que o max retorna o valor.

- Wife x Husband: Pro caso da esposa,...

- Jogo de soma zero com dois jogadores, dá pra encontrar o melhor caso. Já de soma geral, Progração Linear resolve.

- O maxmin é uma das estratégias da pras pessoas muito aversas ao risco.
  - Porém ao não se considerar o payoff do adversário, pode-se acabar que a escolha do maxmin não geraria bons resultados.

O Maxmin só se importa com os payoffs do jogador

##### Minmax

- Minmax: o jogador tenta minimizar o payoff máximo do adversário

No minmax aí já deve-se considerar os outros jogadores.

##### In 2 players zero sum games

##### Theorem (Julia Robinson)

- Se houver uma estratégia pura que tenta sempre ser melhor que a estratégia mista observada, no final acaba-se tendo duas estratégias mistas

Não necessariamente um maxmin para ambos não é um equilíbrio de Nash

## 29/04/2025 - Aula 14 - The complexity of finding a Nash Equilibrium: zero sum games and PPAD | MAS, chapter 3; NCM, chapter 6

## 01/05/2025 - Aula XX - feriado

## 06/05/2025 - Aula 15 - prova 1 - Acabou não sendo prova

### Slide: Mixed Strategies

#### Maxmin and minmax strategies

- Let's play another game

| X   | L      | R      |
| --- | ------ | ------ |
| T   | 100, 2 | 0.9, 5 |
| B   | 2, 1   | 1, 0   |

Esquerda: priorizar ganhar 100 do T, enquanto que o B não tem muitos valore; A diferença entre TR e RB
Direita: priorizar ganhar 5 do R, enquanto que o L não tem muito valor

- Maxmin
  - esquerda: B, pois maximza o menor valor;
  - direita: L, pois maximiza o mínimo.

Qual foi o atrator do T? O grande valor do 100, em comparativo com o 2, 1 e 0.9;

Qual o nome desse fenômeno: fear of missing out. Arrependimento de ter escolhido um lado que não deu tanto payoff caso tivesse sido escolhido. (Expliquei meio mal mas é por aí)

#### Regret

- É o nível de arrependimento de um jogador por tomar uma ação $a_i$

Aqui ele considera que o arrependimento é o máximo que poderia ser ganho menos o que pode ganhar pela escolha da $a_i$

Já o arrependimento máximo é o maior dentre todos os possíveis arrependimentos para todas as ações possíveis.

Dúvida: mas se alguém foi averso ou propenso ao risco, essa avaliação absoluta desses valores já não faria sentido. O que seria feito nesse caso?

Resposta: pra isso, consideraríamos que a matriz de payoff é modificada para refletir a utilidade de quem é propenso ou averso ao risco.

- arg min max (max regret)
  - max regret: para cada célula da matriz, calcula a diferença pro maior ganho possível que o jogador poderia ter ganho
  - Max (max regret):

Dúvida: Por que não pode existir regret negativo?

Resposta: porque quando ele calcula $\max_{a_{i}' \in A_i}$ ele não considera que será uma ação diferente da já escolhida, então o escolhido estará na conta.

Quem não joga minimax regret: esportes radicais.

Falha estratégica: não considera a tomada de ação do outro jogador.

#### Removal of dominated strategies

Outro jogo: no jogo um jogador tem uma escolha estritamente dominante.

F1 e F2: low-priced e upscale

A ideia é que podemos remover estratégias estritamente dominadas para facilitar a decisão

- Dominância estrita: é quando todos os payoffs de um jogador são maiores
- Dominância fraca: quando existe pelo menos uma decisão em que os payoffs são iguais
- Dominante: quando uma estratégia domina todas as outras.
- Estritamente dominada: uma que é pior que todas as outras.
- Uma estratégia que é dominante em relação a todas as outras, quer dizer que ela é um equilíbrio de Nash?
  - Sim
- E uma estritamente dominante também gera equilíbrio de Nash?
  - Sim.
- E ela é pareto ótima?
  - Não.

---

Mais jogo

Estratégia (U, B) domina estratégia M

|  X  |   L    |  C   |   R   |
| :-: | :----: | :--: | :---: |
|  U  |  3, 1  | 0, 3 | 0, 0  |
|  M  |  1, 5  | 1, 1 | 10, 0 |
|  B  | 0, 1/2 | 4, 2 | 5, 0  |

R é estritamente dominada por L e C;

Construção da estratégia mista:

- $U_1^p (L) = 3p$
- $U_1^p (C) = 4-4p$
- ...

Remoções

- R; M; L; U

[Embora eu e o Leonardo não concordemos que faria sentido usar estratégia mista, logo não deveria ser removida a opção M]

---

A ordem de remoção de estratégias estritamente dominantes

- Propriedade XYZ

Porcos jogam...

| Small / Large | Press | Wait  |
| ------------- | ----- | ----- |
| Press         | 1, 5  | -1, 9 |
| Wait          | 4, 4  | 0, 0  |

Small Wait: domina; Remove Small Press.

Entre o grande esperar e pressionar, o grande apertaria.

## 08/05/2025 - Aula 16 - The complexity of finding a Nash Equilibrium: Lemke-Howson | MAS, chapter 4

### Battle of Sexes: replay

Questão clássica de prova: "Qual o p e q que tornam a escolha equilibrada?"

- s = (2/3, 1/3); u(s) = (2/3, 2/3)
- s = (p, q); u(s) = (u(p), u(q)) # Eu acho

| Wife x Husband | Opera | Football |
| -------------- | ----- | -------- |
| Opera          | 2, 1  | 0, 0     |
| Football       | 0, 0  | 1, 2     |

Coroa: os dois vão ópera; Futebol: os dois vão futebol. Não parece ter algum outro motivo para eles fazerem diferente.

Ele considera que o único objetivo do agente racional é maximizar o seu próprio payoff.

"Não há incentivo pra não cooperar"

O uso da moeda é um mecanismo externo ao jogo para que opções possam ser removidas. "To ensure fairness".

"A ideia da estratégia mista é para que o outro se torne indiferente ao que fazer"

### Correlated Equilibrium (Equilíbrio Correlacionado)

História: Animais competindo por comida; Estratégia Hawk é agressiva, Estratégia Dove é pacífica; Se ambos passivos, igualmente; Se um agressivo, um passivo, o agressivo pega mais que o passivo; Se ambos agressivos, destroem a comida.

- P1 (Linhas) x P2 (Colunas)

| X   | H    | D                |
| --- | ---- | ---------------- |
| H   | d, d | b, a             |
| D   | a, b | (a+b)/2, (a+b)/2 |

- $a > b$
- $a + b = c$
- $d \leq 0$
- Onde:
  - $a$: Valor de comida maior
  - $b$: Valor de comida menor
  - $C$: Valor da comida completa
  - $d$: Valor do dano por se machucarem

Perguntei se faz sentido parametrizar.

Equilibrio de nash: para cada um, o preferível é escolher o H.

Hawk e Dove é tipo o dilema dos prisioneiros, porém:

Hawk e Dove também é chamado de Game of Chicken, Ou Snowdrift. Exemplo: Carro vs Carro no trânsito.

- Prisioneiros: T > R > S > P
- Hawk e Dove: T > R > P > S

A intuição é que se forem jogar, não faz sentido confrontar a agressividade com agressividade.

Uma coisa interessante a se observar é que para estratégia pura, o equilibrio de nash não vai variar independente de quais os valores pra esse jogo, dado que as regras do enunciado sejam respeitadas. Mas mudaria para as estratégias mistas.

Outro caso:

| X   | H    | D      |
| --- | ---- | ------ |
| H   | 3, 3 | 1, 5   |
| D   | 5, 1 | -2, -2 |

Existiam 3 cartas: DD, DH e HD

A carta foi D, D; Eu só sabia que cairia D pra mim. Eu escolhi D, ele escolheu H.

Com isso eu ganhei 1 e ele 5.

O que eu deveria ter feito era deixar ele falar primeiro. Eu me mostrei passivo demais logo de primeira, com isso o confortei a ser agressivo.

---

Equilíbrio correlacionado não é ter um controle central que indique o que fazer. Mas sim, considerar que existe uma distribuição de aleatoriedade que trará algum grau de equilíbrio ao jogo.

Um clássico exemplo de equilíbrio correlacionado é o Sinal de Trânsito. O agressivo até pode ultrapassar o sinal e ter o benefício de não parar.

---

#### Formalizando o Equilíbrio correlacionado (CERTAMENTE QUESTÃO DE PROVA)

- Dado um n-agente $G = (N, A, u)$ e um equilíbrio correlacionado é uma tupla $(v, \pi, \sigma)$
  - Onde:
    - $v$ é uma tupla com variáveis aleatórias com domínios D
    - $\pi$ é a distribuição conjunta sobre $v$
    - $\sigma$ é um vetor de mapeamento. $\sigma_i : D_i \to A_i$

Queremos mostrar que a utilidade esperada de acordo com todos os mapeamentos seguindo o mapeamento, vai ser maior ou igual da sua utilizddade perada usando o $\sigma'$

Ou seja, há equilíbrio correlacionado se a utilidade esperada de seguir o que é indicado é maior do que não seguir o que for indicado.

Ex.: mostrar que receber D e trocar pra H tende a dar menor utilidade esperada

- $D_1 = \{d, h\}, D_2 = \{d, h\}$
- $v_1 = [2/3, 1/3], v_2 = [2/3, 1/3]$
- $\pi = Matriz:$

- $\sigma_1 = Matriz:$

- $\sigma' = Matriz:$

Nesses casos aqui, se alguém com D mudar pra H, corre o risco de perder valor. Se tem H e mudar pra D, também.

"Calcular equilíbrio correlacionado é mais fácil do que calcular equilíbrio de Nash"

## 13/05/2025 - Aula 17 - The complexity of finding a Nash Equilibrium: Lemke-Howson | MAS, chapter 4

### Correlated Equilibrium (CE) [Cheguei atrasado]

- Não existe um único Equilíbrio Correlacionado

### Traveler's Dilemma

- Os dois jogadores trouxeram urna de um país exótico. Eles têm o mesmo objeto e mesmo valor. Porém a companhia aérea quebrou. A companhia disse que precisaria saber o valor real para ressarcir. No máximo custa 300, mas vocês precisam me dizer o valor real.
- Um valor inteiro entre 180 e 300 pra empresa ressarcir.
- Ela teme mentira. Ela só considerará o valor menor.
- Quem colocou o menor valor terá uma recompensa de R=5; O outro perderá 5. Se forem iguais, os dois recebem a mesma quantidade.

- Escolhas:

  - R=5
    - (Luciana, Antônio) = (300, 240); Ganhos: (235, 245)
  - R=100
    - (Luciana, Antônio) = (200, 290); Ganhos: (300, 100)

- Ele tem um equilíbrio de Nash?
  - R:5
  - $A_i = \{ 180, \dots, 300\}$
  - (300, 300), porque um conseguiria melhorar ao reduzir em 1
  - (180, 180): Seria um equilíbrio porque não há melhoria ao mudar sua ação
- Se $R=180$, acaba ficando mais evidente que deve-se jogar 180.
- Quando $R=5$, essa diferença é praticamente irrisória.
- "Essa escolha de (180, 180) não parece ser uma ação de equilíbrio"

#### Qual o plot do Traveler's Dilemma?

- Um dos jogadores pode querer maximizar a recompensa por falar um valor menor.

### $\epsilon$-Nash Equilibrium

Ele aceita uma variação do valor de equilíbrio.

- É um $\epsilon$-Nash Equilibrium se todas as utilidades...
- Exemplo pro jogo:
  - $300 \geq 299 + R - \epsilon$
  - $\epsilon \geq R-1$
- Serve para multiagentes quando queremos tolerar pequenas variações

| X   | L                           | R        |
| --- | --------------------------- | -------- |
| L   | 1, 1                        | 0, 0     |
| R   | $$1+\frac{\epsilon}{2}, 1$$ | 500, 500 |

Matéria da prova até $\epsilon$-Nash Equilibrium; A lista 2 vai só até aqui tbm

---

### Computing Solution Concepts of Normal-Form Games

- Buscou-se encontrar equilíbrio em multijogadores de soma geral.
- Todos são exponenciais no pior caso.
- Classe mais básica:
  - NE in two-player, zero sum games
  - Pode ser resolvido com Programação Linear
  - Cada vértice das restrições vai gerar uma solução. Queremos encontrar qual dos vértices tem maior valor de função objetivo.
  - Se formular o problema como Programação Linear, qualquer solver resolve.
  - Um jogo de soma zero com vários jogadores é tão complexa quando jogos de soma geral.

#### Jogo

- $G = (\{1, 2\}, A_1 \times A_2, (u_1, u_2))$
- Solucionando:
  - Minimizar: $U^{*}_1$
  - Subject to:
    - $\sum_{k \in A_2} u_1 (a^j_1, a^k_2) \cdot \leq U^*_1; \forall j \in A_1$
      - Pra todas as ações do jogador 2
      - Essa primeira parte antes do "$\leq$" é o cálculo de uma utilidade esperada.
    - Basicamente tá falando que $u_1(a^j_1, a^k_2) \cdot \leq U^{*}_{1}; \forall k \in A_2$
  - As outras variáveis são as ações.
  - É um minimax do ponto de vista do Jogadpr2

---

| Kicker/Goalie | Left | Right |
| ------------: | ---- | ----- |
|          Left | .58, |       |
|         Right |      |       |

Convertendo pra soma zero:

| Kicker/Goalie | Left | Right |
| ------------: | ---- | ----- |
|          Left | .58, |       |
|         Right |      |       |

- Minimize $X_3$ (geralmente a última variável)
  - 0.08 X_1

---

- Código Python: $f: x_1 \cdot 0, x_2 0 \cdot x_3 0$
- Resultado: utilidade esperada do jogador 1. Boa questão pra prova: interpretar o resultado.

---

E pro jogador 1?
Iremos maximizar.
F = -F
A = -F
Chama a função do solver.

Se a variável de folga for maior que zero é porque há espaço entre a utilidade esperada da ação e o U_i

## 15/05/2025 - Aula 18 - The complexity of finding a Nash Equilibrium: $n$ player games, removal of dominated strategies, and correlated equilibria | MAS, chapter 4

- [JV] Cheguei atrasado

### Qual é a complexidade de se encontrar o equilíbrio de Nash?

- Por que é tão complexo?
- Se fixarmos as ações, os jogadores, e as estratégias puras;
- Problemas:
  - Por enquanto falando de estratégias puras
    - Nem sempre é garantido que há, então no pior caso testam-se todas.
    - Se fixar a quantidade de ações e aumentar a quantidade de jogadores, aumenta exponencialmente a quantidade de tabelas de ações
    - Se fixar a quantidade de jogadores e aumentarmos a quantidade de ações
  - Em estratégias mistas
    - No meu entendimento, teríamos meio que $\mathbb{R}^{|Ações\ Jogador_1|} \times \mathbb{R}^{|Ações\ Jogador_2|}$
- Por que podemos definir que não é NP-Completude?
  - Podemos resumir a um problema de decisão: Resposta = Sim ou Não.
  - Equilíbrio de Nash não é decisão, é busca.
    - "Todo jogo tem pelo menos um equilíbrio de Nash. Já problemas NP-Completo nem sempre tem soluções"

---

| Aspect                | NP  | PPAD |
| --------------------- | --- | ---- |
| Problem Type          |     |      |
| Solution Verification |     |      |
| Existence of Solution |     |      |
| Canonical Example     |     |      |

---

- Theorem (Gilboa and Zemel, 1989)
  1. NP-Completo
     1. pelo menos 2 nash?
     2. X
     3. X
     4. X
     5. X
     6. X
  2. PPAD: "Polynomial Parity Arguments on Directed graphs"
     - G é um grafo com $2^n$ vértices
     - Duas funções
       - $P(id)=id|\epsilon$: todo nó indica qual é seu pai (pode ser nenhum)
       - $C(id)=id|\epsilon$: todo nó indica qual é seu filho (pode ser nenhum)
       - Com isso, entende-se que cada nó apenas tem no máximo um filho e um pai.
     - $\{0\}^n$ não é filho de ninguém: ele é a fonte
     - A solução sempre estará nas fontes e sumidouros diferentes do $\{0\}^n$
     - Algoritmo simples: parta de
     - Dúvida pendente: por que uma fonte diferente do $\{0\}^n$ pode ser um equilíbrio de Nash?

---

### Support of a Mixed Strategy

- Theorem: relação entre estratégias mistas e estratégias puras e suportes (ver slide)

#### Encontrando o suporte

| X   | d   | e   |
| --- | --- | --- |
| a   |     |     |
| b   |     |     |
| c   |     |     |
|     |     |     |

Possíveis suportes: $\{ \{a,b\}\{d,e\}; \{a,c\}\{d,e\}; \{b,c\}\{d,e\} \}$

- E pq não "$\{a,b,c\}\{d,e\}$"?

---

Faremos então um cálculo para encontrar uma probabilidade para estratégia mista tal que eu torne a jogada do outro jogador indiferente à minha escolha.

## 20/05/2025 - Aula 19 - The complexity of finding a Nash Equilibrium: n player games, removal of dominated strategies, and correlated equilibria | MAS, chapter 4

### 22/05/2025 - Aula 20 - Perfect Information Extensive-form games | MAS, chapter 5

### 27/05/2025 - Aula 21 - Perfect Information Extensive-form games | MAS, chapter 5

### 29/05/2025 - Aula 22 - Imperfect Information Extensive-form games | MAS, chapter 5

### 31/05/2025 - Aula 23 - Imperfect Information Extensive-form games | MAS, chapter 5

### 03/06/2025 - Aula 24 - Repeated games: repeated prisoner dilemma, finite and infinite repeated games, Folk's theorem, stochastic games | MAS, chapter 6.1

### 05/06/2025 - Aula 25 - Repeated games: repeated prisoner dilemma, finite and infinite repeated games, Folk's theorem, stochastic games | MAS, chapter 6.1

### 10/06/2025 - Aula 26 - Bayesian games | MAS, chapter 6.3

### 12/06/2025 - Aula 27 - Bayesian games | MAS, chapter 6.3

### 14/06/2025 - Aula 28 - Congestion games | MAS, chapter 6.4

### 19/06/2025 - Aula XX - feriado

### 24/06/2025 - Aula 29 - Congestion games | MAS, chapter 6.4

### 26/06/2025 - Aula 30 - Prova 2
