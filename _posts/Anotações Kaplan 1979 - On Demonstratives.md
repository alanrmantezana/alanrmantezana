## Kaplan

*Abstract*

Descreve-se como a intensão (conteúdo) é determinado pelo caráter do sentido.

## Mundos possíveis e Contexto

Propõe-se primeiramente o desenvolvimento de um índice com coordenadas $i = \langle w, t,p,a\rangle$ onde $w$ é um mundo, $t$ é o instante, $p$ é o lugar, $a$ é o agente . 

Considere

>[!example] (1) I am here now.

(1) só será verdadeira nos $i$s em que, no mundo $w$, o agente $a$ esteja no lugar $p$ no momento de fala $t$. Só assim é possível falar em *utterances* (asserção, proferimento), condicionando os índices $i$.

<span style="color:#00b0f0">Deve-se, portanto, **restringir as possibilidades de índices pra representação de contextos**.</span>

>[!note]
>Isso vai descambar no condicionamento de $\mathscr{F}$ nas LD-estruturas.

>[!important] Proposta *Contextos como mundos*
>Uma sentença $\Phi$ será logicamente verdadeira (válida) se for válida para todos os índices.
> 
 $\Box \Phi$ será verdadeiro num dado índice se $\Phi$ for logicamente verdadeiro.

Ainda assim não parece ser uma solução satisfatória considerando o exemplo

> (1) I am here now

Será falso quando houver um índice $i$ tal que $a$ não esteja em $p$ no momento $t$ no mundo $w$. <span style="color:#00b0f0">Ainda assim, parece que esta sentença não poderia ser enunciada falsamente.</span> **Uma lógica dos demonstrativos deve explicar isso.**

<span style="color:#00b0f0">Se consideramos a regra de que uma fórmula é verdadeira se é verdadeira para todos os índices, temos a generalização</span>

> $\Box$ I am here now
> 

(1), todavia, não é uma verdade lógica para ser passível de necessitação (e.g. eu poderia estar em outro lugar).

>[!warning] Contextos não são mundos
>**Kaplan afirma que isso demanda esclarecimentos sobre a analogia entre o tratamento de contextos e o tratamento de mundos possíveis.**

----- 
## Analiticidade e Necessidade

>[!attention]
>**Kaplan bifurca o conceito de sentido em conteúdo e caráter**

>[!important] Definição. (Conteúdo)
> Aquilo que é dito (compreendido) com relação ao proferimento (*utterance*) de uma sentença em algum contexto específico. 


**Exemplo**. "Eu apanhei no videogame ontem" foi expresso por mim hoje pela manhã. O que foi dito, o que foi compreendido, o sentido, a proposição, o pensamento, é o conteúdo com relação a um contexto que me envolve numa certa data.

>[!important] **Definição (Caráter, Meaning)**. 
>O caráter é o componente do sentido de uma frase, de um pensamento, que determina a partir do contexto um conceito individual que vai determinar a extensão.

**Exemplo**. "Ontem eu chorei na smartfit". "Eu" é associado a um caráter que, a partir de um contexto $c$ onde eu estou chorando na smartfit, atribui um conceito individual $f$ que designa rigidamente a mim mesmo. 

>[!important] Kaplan sugere que contextos diferentes produzem proposições diferentes.

Sobre (1), pode-se afirmar que

>[!attention]
>(a) Quando dita, expressa diferentes proposições em todos os contextos.
> (b) Em quase todos os contextos expressa uma proposição contingente.
> (c) Em todos os contextos, quando dita, trata-se de uma proposição verdadeira (no mundo em que foi dito).

Eventualmente, ele chega à conclusão de que (1) é uma verdade analítica, mas não uma verdade lógica.

>[!question] Em qual contexto (1) expressa uma proposição necessária? 
> Em outras palavras, existe um contexto onde para todo instante $t$ e todo mundo $w$ (1) é verdadeiro? Algo que necessariamente está posicionado em algum lugar?

>[!important]
> Ao caráter (meaning) é devida a sua analiticidade. Ao conteúdo é devida a sua necessidade.

**O autor fala sobre como isso pode lançar luz sobre as relações entre analiticidade e necessidade levantadas por Kripke**^[seria bom reler o Kripke, ou o texto que eu baixei]. Finalmente ele começa a explanação do sistema formal.

---
## Logic of Demonstratives (LD)

### Símbolos

A lógica contém dois tipos de variáveis. De indivíduos $\alpha$ e de lugares $\beta$ . 
A lógica contém um tipo de predicado: o de colocação $\pi$.
Há $i,p$-funtores que, para uma fórmula, devolvem ou indivíduos ou posições da fórmula.
A lógica contém operadores de lógica de primeira ordem com identidade.
- Variáveis de indivíduos $\alpha$;
- Variáveis de lugares $\beta$;
- Predicado de colocação $\pi$;
- funções que devolvem lugares ou indivíduos $i,p-\eta$;
- Conectivos proposicionais $\lor,\wedge,\rightarrow,\neg$;
- Quantificadores $\forall, \exists$;
- Identidade $=$
- Artigo definido *the*
- Demonstrativo *dthat*
- Operadores modais aléticos $\Box, \Diamond$
- Operadores modais temporais $P, G, F$;
- Operadores da Lógica dos Demonstrativos $N,A,Y$;
- Individual constant ($0$-$0$ place $i$-functor): $I$;
- Position constant ($0$-$0$ place $p$-functor): $Here$;

>[!note] Predicados de colocação devem conter em si as sentenças expressas.
>Dessa forma, $\phi\alpha_{i},\beta_{p}$ pode significar algo como $\alpha$ que está em $\beta$ profere $\phi$.

>[!question] Como distinguir *utterances* de *sentenças num contexto*?


São termos: 
- variáveis de indivíduos $\alpha$
- variáveis de posição $\beta$
- $i$-termos: $\alpha$, $\alpha\Phi$
- $p$-termos: $\beta$, $\beta\Phi$
- $i,p$-funtores.
- fórmulas
São fórmulas $\Phi$:
$$\Phi ::= \langle \pi\alpha_1,...,\alpha_n,\beta_1,...,\beta_{m} | \eta\alpha_1,...,\alpha_n,\beta_1,...,\beta_{m}| \neg\Phi|\Phi\lor\Psi|\Phi\wedge\Psi|\Phi\rightarrow\Psi| \forall\alpha\Phi|\exists\alpha\Phi|\alpha=\alpha| \beta = \beta$$
$$\text{the }\alpha \Phi| \text{dthat }\alpha \Phi | \Box\Phi|\Diamond\Phi|\text{P}\Phi|\text{G}\Phi|\textnormal{F}\Phi| \text{N}\Phi| \text{A}\Phi| \text{Y}\Phi\rangle$$

---

## Semântica

**Definição 1. (Estrutura LD)**. Uma estrutura $\mathfrak{A}$ com 6 conjuntos não-vazios: o conjunto de contextos $\mathscr{C}$, o conjunto de agentes $\mathscr{U}$, o conjunto de lugares $\mathscr{P}$, o conjunto de instantes no tempo $\mathscr{T}=\mathbb{N}$, o conjunto de mundos $\mathscr{W}$ e uma função $\mathscr{F}$. 

$$\mathfrak{A} = \langle \mathscr{C},\mathscr{W},\mathscr{U},\mathscr{P},\mathscr{T},\mathscr{F}\rangle$$
$$\mathscr{C} = \{\langle w,a,p,t\rangle | w\in \mathscr{W},a\in \mathscr{U},p\in \mathscr{P},t\in \mathscr{T}\}$$
O **conjunto de instantes $\mathscr{T}$ é comum a todos os mundos**, assim como o **conjunto de posições $\mathscr{P}$**. 

>[!question] Qual a necessidade dessa suposição? 
>Seria para simplificação? É meio kantiano/newtoniano?

**Definição 2. ($\mathscr{F}_{\pi}$ interpretação).** Para um predicado de lugar $\pi$, a função $\mathscr{F}_{\pi}$ é tal que atribui, dado um mundo $w$ e dado um instante de tempo $t$, um subconjunto de $\mathscr{U}^{m}\times\mathscr{P}^{n}$.

>[!note] Dado um momento em um mundo, agentes e posições se combinam para formar posicionamentos, ou praticamente estados de coisas linguisticamente relevantes.

**Definição 3. ($\mathscr{F}_{\eta}$ interpretação)**. Para um $i$-funtor $\eta$, a função $\mathscr{F}_{\eta}$ atribui, dado um subconjunto de $\mathscr{U}^{m}\times\mathscr{P}^{n}$, um subconjunto de $\mathscr{U}$ acrescido de $\emptyset$.

**Definição 4. ($\mathscr{F}_{\eta}$ interpretação)**. Para um $p$-funtor $\eta$, a função $\mathscr{F}_{\eta}$ atribui, dado um subconjunto de $\mathscr{U}^{m}\times\mathscr{P}^{n}$, um subconjunto de $\mathscr{P}$ acrescido de $\emptyset$.

>[!question]
>Por que há a necessidade de um elemento indefinido na definição acima?
>
>R: Descrições definidas sem referentes. Sentenças em um contexto *sem proferimento*. Um "eu" escrito numa parede.

**Definição 5. ($\mathscr{F}_{\text{exists}}$ interpretação)** um indivíduo pertence ao conjunto dos agentes se, e somente se, existe um $t \in \mathscr{T}$, um $w \in \mathscr{W}$ tal que $\mathscr{F}_{\text{exists}}: w,t \rightarrow \langle i\rangle$. 

>[!attention] *Algo existe no modelo se existiu em algum instante em algum mundo*.

>[!note] Corresponde ao $1-0$ *place predicate*: exist.
>$1-0$ correspondem às aridades.

**Fato 6. ($\mathscr{F}_{\text{located}}$ interpretação) Se $c \in \mathscr{C}$, então $\langle c_{a}, c_{p} \rangle \in \mathscr{F}_{\text{located}}(c_{t},c_{w}).$ 

>[!attention] *Se há um contexto onde alguém está em algum lugar, isso ocorre em um instante, em um mundo.*


>[!note]
>Corresponde ao 1-1 *place predicate*: located. 


**Fato 7. ($\mathscr{F}_{\text{located}}$)**. Se $\langle i,p \rangle \in \mathscr{F}_{\text{located}}(t,w)$, então $\langle i \rangle \in \mathscr{F}_{exists}(t,w)$. *Se alguém está em algum lugar, em um instante, em um mundo, então este alguém existe no instante e no mundo.*

>[!attention] *1-1 place predicate located* implica *1-0 place predicate: exist*.

**Verdade e Denotação**

$\models^{\mathfrak{A}}_{cftw} \Phi$ significa que $\Phi$ é verdadeiro em um contexto $c$, dada uma $\mathscr{V}$-atribuição $f$ na estrutura $\mathfrak{A}$ em um instante $t$ e um mundo $w$.

 $|\alpha|_{cftw}$ significa a denotação de $\alpha$ em um contexto $c$ a partir de uma $\mathscr{V}$-atribuição $f$ na estrutura $\mathfrak{A}$ em função de um instante $t$ e um mundo $w$.


>[!tip] CoFee ToWer
>A *context*, a *function*, a *time*, a *world*. CoFee ToWer!!!

**Atribuição bissortida**

$f \in \{f_{i}\cup f_{p}: f_{i}\in\mathscr{U}^{\mathscr{V}_{i}} \text{and} f_{p} \in \mathscr{P}^{\mathscr{V}_{p}}\}$

**Regra para quantificadores substitucionais**

$f^{\alpha}_{x} = (f - \{\langle\alpha, f(\alpha)\rangle\})\cup\{\langle\alpha, x\rangle\}$

**Condições de verdade**

Considere
$\hat\alpha := \alpha_{1},...,\alpha_{n}$.

1.  $|\alpha|_{cftw} = f(\alpha)$
2.  $\models^{\mathfrak{A}}_{cftw} \pi \hat\alpha\hat\beta$ iff $\langle|\hat\alpha|_{cftw}, |\hat\beta|_{cftw}\rangle \in \mathscr{F}_{\pi}(tw)$.
3. Se $\eta$ não é $I$ nem $Here$ , então 
	1. $|\eta\hat\alpha,\hat\beta|_{cftw} = \mathscr{F}_{\eta}(tw)(\langle\hat\alpha,\hat\beta\rangle)$, se nenhuma variável é indefinida. 
	2. Vazio, caso contrário.
4. $\models_{cftw} \phi \wedge \psi$ *sse* $\models_{cftw} \phi$ *e* $\models_{cftw} \psi$;
	1. Analogamente para outros conectivos proposicionais.
5. Se $\alpha \in \mathscr{V}$, então $\models_{cftw} \forall \alpha \phi$ sse $\forall i \in \mathscr{U}$  $\models_{cf^{\alpha}_{i}tw} \phi$; 
	1. analogamente para o existencial e para variáveis de lugar
6. Se $\alpha \in \mathscr{V}_{i}$, então $|\text{the } \alpha_{cftw} \phi| =$
	1. O único $i \in \mathscr{U}$ tal que $\models_{cf^{\alpha}_{i}tw}\phi$;
	2. $\emptyset$, caso contrário.
		1. De forma semelhante para lugar;
7. $\models_{cftw} \alpha = \beta$ *sse* $|\alpha|_{cftw} = |\beta|_{cftw}$;
8. Modais
	1. $\models_{cftw} \Box\phi$ *sse* $\forall w' \in \mathscr{W}$, $\models_{cftw'}\phi$;
	2. $\models_{cftw} \Diamond\phi$ *sse* $\exists w' \in \mathscr{W}$, $\models_{cftw'}\phi$;
9. Tense
	1. $\models_{cftw} F\phi$ *sse* $\exists t'$ t.q. $t < t'$ $\models_{cft'w}\phi$;
	2. $\models_{cftw} P\phi$ *sse* $\exists t'$ t.q. $t > t'$ $\models_{cft'w}\phi$;
	3. $\models_{cftw} G\phi$ *sse* $\models_{cf(t-1)w}\phi$;
10. Demonstratives
	1. $\models_{cftw} N\phi$ se, e somente se, $\models_{cfc_{T}w} \phi$ ;
	2. $\models_{cftw} A\phi$ se, e somente se, $\models_{cftc_{w}} \phi$ ;
	3. $\models_{cftw} Y\phi$ se, e somente se, $\models_{cf(c_{T}-1)w} \phi$;
11. $|\text{dthat } \alpha|_{cftw} = |\alpha|_{cfc_{T}c_{w}}$;
12. $|I|_{cftw} = c_{A}$;
13. $|Here|_{cftw} = c_{P}$;


>[!note]
>Na definição de $\eta$, a variável pode ser indefinida. Nesse caso, o valor da fórmula será indefinido. Isso não se dá por meio da atribuição $f$ de valor às variáveis, mas sob o jugo da função $\mathscr{F\eta}$.
>
>O valor indefinido também serve para descrições definidas que falham, como na definição 6.
>
>$I$ e $Here$ são constantes para indivíduos $c_{A}$ e para posições $c_{P}$, respectivamente.

No caso, os demonstrativos não são cegos às propriedades do contexto, e é onde mais vale o <span style="color:#00b0f0">CoFee ToWer</span>. As n-uplas da estrutura formam esses objetos que serão referentes e componentes de um contexto.

---
### Conteúdo e Verdade

O conteúdo de uma sentença é aquilo que é expresso em um determinado contexto por uma frase. Enunciados realizados em diferentes contextos expressam diferentes proposições. 

>[!important]
>**O conteúdo de uma sentença é a proposição expressa quando dita em um contexto.**

<span style="color:#00b0f0">Em primeiro lugar, é necessário distinguir um *proferimento* de uma *frase num contexto*.</span> A primeira pertence à teoria dos atos de fala. <span style="color:#00b0f0">A segunda é uma noção semântica.</span> Dois *proferimentos* não podem ser realizados no mesmo contexto (*há um só agente*), ainda assim, 

>[!important]
>é conveniente para uma lógica dos demonstrativos que se possa realizar inferências num mesmo contexto. **Assim, uma sentença $\phi$ não precisa ser *proferida* no instante, no mundo do seu contexto pelo agente do seu contexto, para que seja verdadeira.** 

>[!question] Sentence in a context em LD
>Eu não compreendo. Para que serve o contexto então? Ou melhor, o $c_{A}$. Esse é o caso em que o agente é indefinido? Quando saber quando algo é proferido ou não? Ele afirma que a verdade de $\phi$ não depende do proferimento de $c_{A}$ em $c$. Daí acho que vem a noção de conteúdo.

>[!important] Conteúdo
>Em segundo lugar, geralmente não se pensa em uma proposição como tendo seu valor de verdade dependendo de um instante $t$ ou um mundo $w$. Para esta noção de proposição de $\phi\text{-in-}c$, temos a noção de *Conteúdo de* $N\phi$ em $c$.

Seja $\Gamma$ um termo ou uma fórmula, escreve-se $\{\Gamma\}^{\mathfrak{A}}_{cf}$ para o conteúdo de $\Gamma$ na estrutura $\mathfrak{A}$ sob a atribuição $f$ no contexto $c$.

**Definição.** (*Conteúdo*) 
1. Se $\phi$ é uma fórmula, então $\{\phi\}_{cf}^{\mathfrak{A}}$ é 
	1. uma função que atribui para todo $t \in \mathscr{T}$ e para todo $w \in \mathscr{W}$ , o valor Verdadeiro se  $\models^{\mathfrak{A}}_{cftw}\phi$,
	2. e Falso caso contrário.
2. Se $\alpha$ é um termo, então $\{\alpha\}_{cf}^{\mathfrak{A}}$ é uma função que atribui para todo $t \in \mathscr{T}$ e para todo $w \in \mathscr{W}$  $|\alpha|_{cftw}^{\mathfrak{A}}$.

>[!important]
>O conteúdo é a função o que, ou atribui a uma sentença a Verdade a todos os instantes, para todos os mundos; ou Falsidade, caso contrário. 
>
>O conceito individual é uma função que atribui o mesmo indivíduo para todos os instantes para todos os mundos.


>[!note]
> Em 10, talvez parte da crítica de Crossley & Humberstone esteja errada. Kaplan considera o mundo em questão em que $A\Phi \equiv \Phi$ como o mundo do contexto, do *utterance*. Um jeito de analisar isso talvez seja [[estudar com cuidado a semântica do operador de Kaplan]].

**Exemplo.**

==**Volta-se à observação de que sentenças que contém demonstrativos expressam proposições diferentes em diferentes contextos.**== A proposição expressa num contexto é denominada o conteúdo de uma expressão no dado contexto. ==O conteúdo de uma sentença é, à grosso modo, **a proposição que a frase expressaria se dado contexto fosse o caso**.==

>[!note]
>Acrescenta-se aqui um elemento: se um dado contexto fosse o caso, ou atual. Tal mesmo como se falasse de um minimundo atual.

$$\models^{\mathfrak{A}}_{cftw}\phi \text{ if, and only if, }\{\phi\}^{\mathfrak{A}}_{cf}(tw)= \text{True}$$
O autor complementa, afirmando que $\phi$ proferida em um contexto $c$ com relação a um instante $t$ em um mundo $w$ seria verdadeiro *sse* $\phi\text{-proferido-em-}c$ fosse Verdadeira dado que $w$ fosse atual e $t$ fosse agora.

>[!note]
>Acho que aqui ele está precisificando essa associação com um instante $t$ e um mundo $w$. Ele afirma que o *estar com relação a* um instante $t$ e mundo $w$ é **supor a atualidade de $t$ e $w$ como contexto de avaliação**.
>


---
### Contexto e Verdade

**Definição. (Verdade em um Contexto)** $\phi$ é verdadeiro em um contexto $c$ (em uma estrutura $\mathfrak{A}$) se, e somente se, para toda atribuição de variáveis $f$, $\{\phi\}_{cf}^{\mathfrak{A}}(c_{T}, c_{W}) = \text{True}$. 

Essa quantificação sobre a função de atribuição de variáveis parece o tipo de coisa que fará com que "Eu estou aqui" seja verdadeiro. Ficaria mais claro escrevendo:
	Para $c$, $f_{i}$, para todo $|\alpha|_{cf_{i}}$,
$$\{\pi\alpha\}_{cf}^{\mathfrak{A}}(c_{T}, c_{W}) = \text{True}.$$
>[!question]
>A função $f$ é o conceito individual?


**Definição.** (LD-Válido). $\models^{\mathfrak{A}}_{LD} \phi$  *se, e somente se,* $\phi$ é verdadeiro em todo contexto $c$ em cada LD-estrutura $\mathfrak{A}$. 

>[!example] Teoremas
> 1. $\models (\text{dthat }\alpha = \alpha)$;
> 2. $\models_{cfc_{T}c_{W}} N(Located(I,Here))$; (vdd em virtude do fato 7 )
> 3. $\models Exist(I)$

>[!example] Não teoremas
>$\sim\models \Box(\text{dthat }\alpha = \alpha)$;
> $\sim\models_{cfc_{T}c_{W}} \Box N(Located(I,Here))$; (explicar essa)
> $\sim\models \Box Exist(I)$

> Esses operadores quantificam sobre mundos que não carregam relação nenhuma com o contexto. O contexto não está sob o escopo dos mundos. Por isso pode-se avaliar em função de $c$, quantificar sobre os $w \in \mathscr{W}$, sem considerar os $c_{A},c_{P},c_{T},c_{W}$. Na verdade, os contextos parecem estar acima dos mundos.

>[!important] Operadores Demonstrativos são Quantificadores
>Eles se ligam às variáveis de índivíduo e posição.

>[!important] Definição Variável Ligada
>Se $\alpha_{1},...,\alpha_{n}$ são as variáveis de $\phi$ em ordem alfabética, o fechamento de $\phi = AN\forall\alpha_{1},...,\alpha_{n}\phi$.

Uma fórmula $\phi$ é fechada se é equivalente ao *fechamento* de $\phi$ como na definição acima

>[!question] Qual é a função do assignment aqui?

**Definição.** (Conteúdo Estável). Seja $\Gamma$ um termo ou fórmula. Seu conteúdo é estável em um contexto $c$ se, e somente se, para toda atribuição de variáveis $f$, $\{\Gamma\}^{\mathfrak{A}}_{cf}$ é uma função constante; i.e. para todo instante $t, t'$ e para todo mundo $w, w'$, $\{\Gamma\}^{\mathfrak{A}}_{cf}(tw)=\{\Gamma\}^{\mathfrak{A}}_{cf}(t'w')$.

>[!summary]
> Fixa-se o contexto. A proposição expressa, o conteúdo, tem valor de verdade fixo pra todo $t$ em qualquer mundo $w$. Claramente uma proposição fregeana, eterna, é exemplo disso. Consideremos, todavia, com "Eu estou aqui". Aí, pelas regras semânticas, não se afeta.



