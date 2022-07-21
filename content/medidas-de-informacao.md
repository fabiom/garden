---
title: "Medidas de Informação"
alias: informação
---

Existem várias definições quantitativas de informação, mas a maioria delas é formulada utilizado teoria de probabilidade. A intuição por trás disso é que informação é algo que reduz incerteza, e podemos descrever incerteza como um conceito probabilístico.

## Tipos

Existem três tipos de medidas de informação. São eles:

1. **Informação entrópica:** fornece a quantidade de informação contida em uma [[variavel-aleatoria|variável aleatória]] ou [[distribuicao-de-probabilidade|distribuição de probabilidade]], medindo a quantidade de incerteza ou de surpresa obtidas no resultado de um experimento.

2. **Informação paramétrica:** mede a informação fornecida sobre um parâmetro desconhecido por um experimento aleatório.

3. **Informação relativa:** expressa a quantidade de informação fornecida pelos dados para discriminar a favor de uma distribuição em detrimento de uma outra. Pode ser vista, assim, como uma medida de dissimilaridade entre distribuições.

## Propriedades
Podemos listar algumas propriedades desejadas para medidas de informação. No entanto, nem todas são satisfeitas pelas medidas usadas na prática. Sejam $X$ [[variavel-aleatoria|variável aleatória]], e $T(X)$ uma [[funcao-mensuravel|função mensurável]]. Vamos denotar uma medida de informação de qualquer tipo por $I$, e a informação de $X$ por $I_X$. Algumas boas propriedades desejadas de medidas da informação são: \[1\]

1. Não-negatividade: $I_X \ge 0$.

2. Algum tipo de aditividade:
	- Forte: $$I_{X,Y} = I_X + I_Y,$$ se $X$ e $Y$ são [[independentes]].
	- Fraca: $$I_{X,Y} = I_X + I_{Y|X}.$$
	- Subaditividade: $$I_{X,Y} \le I_X + I_Y.$$
	- Superaditividade: $$I_{X,Y} \ge I_X + I_Y.$$

3. Desigualdade [[probabilidade-condicional|condicional]]: $I_Y \ge I_{Y|X}.$

4. Máxima informação: $I_X \ge I_{T(X)}$ (ver [[desigualdade de processamento de dados]]).

5. Invariância por suficiência: $I_{X} = I_{T(X)}$ se, e somente se, $T$ é [[estatistica-suficiente|estatística suficiente]].

6. Convexidade: Se $\alpha \in [0,1]$, $f_1,f_2$ são funções [[funcao-densidade|densidade]], e definimos $X_\alpha \sim f_\alpha$, onde $f_\alpha = \alpha f_1 + (1-\alpha)f_2$, então
$$
I_{X_\alpha} \le \alpha I_{X_1} + (1-\alpha)I_{X_2}.
$$


## Medidas de informação usuais
Algumas das medidas de informação utilizadas são:

- Informação entrópica:
	- [[Entropia de Shannon]]
	- [[Entropia de Hartley]]
	- [[Entropia de Tsallis]]
	- [[Entropia de Rényi]]
- Informação paramétrica:
	- [[Informação de Fisher]]
- Informação relativa:
	- [[Entropia relativa]]
	- [[Entropia relativa simetrizada]]
	- [[Distância de Hellinger]]
	- [[Distância de Fisher-Rao]]
	- [[Divergência de Cauchy-Schwarz]]


## Referências
\[1\] K. Ferentinos, T. Papaioannou - [*New parametric measures of information*](https://core.ac.uk/download/pdf/82659216.pdf)