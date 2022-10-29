# <font face="宋体">高等数学I - 笔记
##### Connor 2020.10.30
---
## 映射
#### 映射的定义
* $有集合X,Y,映射f$
* $X为f的定义域,记作D_f$
* $Y为f的值域,即X中所有元素的像的集合,记作R_f$
#### 映射的要素
* $D_f = X$,$R_f \subset Y 或 R_f = Y$
* $\forall x \in X, \exist y=f(x)唯一$
* $而\forall y \in R_f, y的原像不一定唯一$
#### 特殊映射
* $若R_f = Y,则称f为X到Y的满射$
* $若\forall x_1\ne x_2 \in X,f(x_1)\ne f(x_2),则称f为X到Y的单射$
* $若f为X到Y的满射和单射,则称f为X到Y的一一映射或双射$
#### 逆映射
$若f为X到Y的单射,即f:X\to R_f,则有g:R_f\to X$<br>$也就是说\forall y\in R_f,f(y) = x,称g为f的逆映射$
#### 复合映射
$若有\quad g:X\to Y_1\quad f:Y_2\to Z\quad Y_1\subset Y_2\quad则有\quad f\circ g:X\to Z$<br>$(f\circ g)(x) = f(g(x)),x\in X$
$注意:$<br>$f与g的复合有顺序$<br>$f\circ g \ne g \circ f$<br>$f \circ g有意义 \ne g \circ f有意义$

