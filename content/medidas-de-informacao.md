---
title: "Medidas de Informação"
alias: informação
---

Existem várias definições matemáticas de informação, mas a maioria delas é formulada utilizado teoria de probabilidade. A intuição por trás disso é que informação é algo que reduz incerteza, e podemos descrever incerteza como um conceito probabilístico.

Sejam $X$ [[variavel-aleatoria|variável aleatória]], e $T(X)$ uma [[funcao-mensuravel|função mensurável]]. Vamos denotar uma medida de informação qualquer por $I$, e a informação de $X$ por $I_X$. Algumas boas propriedades que costumam ser desejadas de medidas da informação são: [1](#Referências)
1. Não-negatividade: $I_X \ge 0$ --- informação é positiva ou nula.
2. Algum tipo de aditividade:
	- Forte: $I_{X,Y} = I_X + I_Y$ se $X$ e $Y$ são [[independentes]].
	- Fraca: $I_{X,Y} = I_X + I_{Y|X}$.
	- Subaditividade: $I_{X,Y} \le I_X + I_Y$ --- se a informação conjunta de duas coisas é no máximo a soma das informações de cada uma individualmente (a desigualdade é importante, pois pode haver infromação repetida em $X$ e $Y$, que é contada duas vezes quando somamos $I_X$ e $I_Y$).
	- Superaditividade: $I_{X,Y} \ge I_X + I_Y$ --- se existe [[dip|sinergia]], pode ser que o todo tenha mais informação que cada parte individualmente.
3. Desigualdade [[probabilidade-condicional|condicional]]: $I_Y \ge I_{Y|X}$.
4. Máxima informação: $I_X \ge I_{T(X)}$ --- processar dados não aumenta informação.
5. Invariância por suficiência: $I_{X} = I_{T(X)}$ se, e somente se, $T$ é [[estatistica-suficienteestatística suficiente]].
6. Convexidade: Se $\alpha \in [0,1]$, e $f_1,f_2$ são as funções [[funcao-densidade|densidade]] então
$$
I_X \left( \alpha f_1 + (1-\alpha)f_2 \right) \le
\alpha I_X(f_1) + (1-\alpha)I_X(f_2)
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
- Informação não-paramétrica:
	- [[Entropia relativa]]


### Referências
[1]: K. Ferentinos, T. Papaioannou - [*New parametric measures of information*](https://core.ac.uk/download/pdf/82659216.pdf)