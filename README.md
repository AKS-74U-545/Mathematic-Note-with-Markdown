# <font face="宋体">高等数学I - 笔记
##### Connor 2020.10.30
---
##目录
[映射](#映射)
[函数](#函数)
[数列的极限](#数列的极限)
[函数的极限及其性质](#函数的极限及其性质)
[无穷大与无穷小](#无穷大与无穷小)
[极限运算法则](#极限运算法则)
[两个重要极限&N次方差公式](#两个重要极限)


---
<span id='映射'></span>

## 映射
#### 映射的定义 
* $有集合X,Y,映射f$
* $X为f的定义域,记作D_f$
* $Y为f的值域,即X中所有元素的像的集合,记作R_f$
#### 映射的要素
* $D_f = X$,$R_f \subset Y 或 R_f = Y$
* $\forall x \in X, \exists y=f(x)唯一$
* $而\forall y \in R_f, y的原像不一定唯一$
#### 特殊映射
* $若R_f = Y,则称f为X到Y的满射$
* $若\forall x_1\ne x_2 \in X,f(x_1)\ne f(x_2),则称f为X到Y的单射$
* $若f为X到Y的满射和单射,则称f为X到Y的一一映射或双射$
#### 逆映射
$若f为X到Y的单射,即f:X\to R_f,则有g:R_f\to X$<br>$也就是说\forall y\in R_f,f(y) = x,称g为f的逆映射$
#### 复合映射
$若有\quad g:X\to Y_1\quad f:Y_2\to Z\quad Y_1\subset Y_2\quad$<br>$则有\quad f\circ g:X\to Z$<br>$(f\circ g)(x) = f(g(x)),x\in X$
$注意:$<br>$f与g的复合有顺序$<br>$f\circ g \ne g \circ f$<br>$f \circ g有意义 \ne g \circ f有意义$

<span id='函数'></span>

## 函数
#### 函数的特性
##### 有界性
$若f(x)\leq K_1,则f(x)有上界$
##### 单调性
$To Be Finished.$
##### 奇偶性
$To Be Finished.$
##### 周期性
$To Be Finished.$
#### 反函数
$有f^{-1}:f(D)\to D,则称f^{-1}(x)为f的反函数,称f(x)为直接函数$<br>$f(x)与f^{-1}(x)关于直线y=x对称$
#### 复合函数
$y=f(u)定义于D_f$<br>$u=g(x)定义于D_g,且其值域R_g \subset D_f,则由下式确定的函数$<br><p align='center'>$y = f(g(x)),\quad x \in D_g$</p><br>$称为由函数u=g(x)与函数y=f(u)构成的复合函数,它的定义域为D_g,变量u称为中间变量.$
#### 初等函数
$由常数和基本初等函数经过有限次的四则运算和有限次的函数复合步骤并可用一个式子表示的函数,称为初等函数.$

<span id='数列的极限'></span>

## 数列的极限
#### 数列极限的定义
$若\exists 常数\alpha,对于任意整数\epsilon,总有N\in N^*,使得当n>N时,有|X_n-\alpha |<\epsilon,$<br>$则称常数\alpha 是数列\{X_n\}的极限(或称数列\{X_n\}收敛与\alpha,$<br>$记作lim_{n\to\infty}=\alpha或x_n\to\alpha(n\to\infty).$<br>$若不存在N使大于N的所有n对应的(x_n-\alpha)都小于任意给定的\epsilon 即不存在满足条件的\alpha,$<br>$则称数列没有极限,或称数列发散,也称lim_{n\to\infty}x_n不存在.$
#### 收敛数列的性质
- $若数列收敛,则其极限唯一.$
- $若数列收敛,则其一定有界.$
- $若数列收敛与\alpha,则其任意子数列也收敛于\alpha.$
- $收敛数列的保号性$
  - $若lim_{n\to\infty}x_n=\alpha且\alpha>0,则存在N使得当n>N时,都有x_n>0.$
  - $反之亦然$

<span id='函数的极限及其性质'></span>

## 函数的极限及其性质
#### 自变量趋于有限值时函数的极限
$设函数f(x)在x_0的某一去心邻域内有定义.$<br>$若存在常数A,对于任意给定的正数\epsilon\quad(不论它多么小),$<br>$总存在整数\delta,使得当x满足不等式0<|x-x_0|<\delta时,对应的函数值f(x)都满足不等式|f(x)-A|<\epsilon,$<br>$则称常数A为函数f(x)当x\to x_0时的极限,记作lim_{x\to x_0}f(x)=A或f(x)\to A(当x\to x_0).$
#### 自变量趋于无穷大/无穷小时函数的极限
$To Be Finished.$
#### 函数极限的性质
- $唯一性:若有lim_{x\to x_0}f(x)=A,则A唯一.$
- $局部有界性:若lim_{x\to x_0}f(x)=A,则有常数M>0和\delta>0,使得当0<|x-x_0|<\delta时,有f(x)\leq M.$
- $若lim_{x\to x_0}f(x)=A,\begin{cases}A>0,\\A<0,\end{cases}则有常数\epsilon>0,使得当0<|x-x_0|<\epsilon时,有\begin{cases}f(x)>0.\\f(x)<0.\end{cases}$
- $若lim_{x\to x_0}f(x)=A(A\ne0),则有x_0的某一去心邻域\mathring{u}(x_0),当x\in\mathring{u}(x_0)时,则有|f(x)|>\cfrac{|A|}{2}.$
- $[推论]:若在x_0的某去心邻域内\begin{cases}f(x)\geq0,\\f(x)\leq0,\end{cases}且lim_{x\to x_0}f(x)=A,则\begin{cases}A\geq0.\\A\leq0.\end{cases}$
- $若有lim_{x\to x_0}f(x),有\{x_n\}为函数f(x)定义域内任一收敛于x_0的数列满足:x_n\ne x_0(n\in N_+),$<br>$则相应的函数值数列\{f(x_n)\}必收敛,且lim_{n\to\infty}f(x_n)=lim_{x\to x_0}f(x)$

<span id='无穷大与无穷小'></span>

## 无穷大与无穷小
#### 无穷小的定义
- $以0为极限的函数是当x\to x_0(或x\to\infty)时的无穷小.$
- $以0为极限的数列是当n\to\infty时的无穷小.$
<small>$无穷小\ne很小的数$</small><br><small>$0是可以作为无穷小的唯一的常数,因为如果f(x)=0,那么对于任意给定的\epsilon>0,总有|f(x)|<\epsilon.$</small>

#### 定理:函数具有极限的充要条件
$在自变量的同一变化过程x\to x_0(或x\to\infty)中,函数f(x)具有极限A的充分必要条件是f(x)=A+\alpha,其中\alpha是无穷小.$
#### 无穷大的定义
$设函数f(x)在x_0的某一去心邻域内有定义(或|x|大于某一正数时有定义),若对于若任意给定的正数M(无论它多么大)$<br>$总存在正数\delta(或正数X),只要x适合不等式0<|x-x_0|<\delta(或|x|>X)对应的函数值f(x)总满足不等式|f(x)|>M,$<br>$那么称函数f(x)是当x\to x_0(或x\to\infty)时的无穷大.$
> <small>$按函数极限的定义来说,当x\to x_0(或x\to\infty)时的无穷大的函数f(x)的极限是不存在的,但为了便于叙述函数的这一性态,我们也说函数的极限是无穷大,并记作$
> \[lim_{x\to x_0}f(x) = \infty\quad(或lim_{x\to\infty}f(x) = \infty)\]
> $如果在无穷大的定义中,把|f(x)>M|换成f(x)>M(或f(x)<-M),就记作:$
> \[lim_{x\to x_0(x\to\infty)}f(x)=+\infty\quad(或lim_{x\to x_0(x\to\infty)}f(x)=-\infty)\]
> $注意:无穷大( )不是数,不可与 很大的数混为一谈.$</small>
#### 定理:无穷大与无穷小相互转化
$在自变量的同一变化过程中,如果f(x)为无穷大,那么\cfrac{1}{f(x)}为无穷小;反之,如果f(x)为无穷小且f(x)\ne0,那么\cfrac{1}{f(x)}为无穷大.$

<span id='极限运算法则'></span>

## 极限运算法则
#### $定理1_{P_{38}}$
- $两个无穷小的和是无穷小,有限个无穷小的和也是无穷小$
#### $定理2_{P_{39}}$
- $有界函数与无穷小的乘积是无穷小.$
#### $\color{blue}{推论_{P_{39}}}$
- $常数与无穷小的乘积是无穷小.$
- $有限个无穷小的乘积是无穷小.$
#### $定理3_{P_{39}}$
$若limf(x) = A,limg(x) = B,则:$
- $lim(f(x)\pm g(x)) = limf(x)\pm limg(x) = A\pm B$
- $lim(f(x)\cdot g(x)) = limf(x)\cdot limg(x) = A\cdot B$
- $lim\cfrac{f(x)}{g(x)} = \cfrac{limf(x)}{limg(x)}=\cfrac{A}{B}$
#### $\color{blue}{推论_{P_{41}}}$
- $lim((C\cdot f(x))) = C\cdot limf(x)\quad(limf(x)存在,C是常数)$
- $lim(f(x)^n) = (limf(x))^n\quad (limf(x)存在,n\in N^*)$
#### $定理4_{P_{41}}$
$有数列\{x_n\}和\{y_n\},lim_{n\to\infty}x_n = A,lim_{n\to\infty}y_n = B$
- $lim_{x\to\infty}(x_n\pm y_n) = A\pm B$
- $lim_{n\to\infty}(x_n\cdot y_n) = A\cdot B$
- $lim_{n\to\infty}\cfrac{x_n}{y_n} = \cfrac{A}{B}$
#### $定理5_{P_{41}}$
$若lim\phi(x) = A,lim\psi(x) = B,则A\geq B.$

<span id='两个重要极限'></span>

## 两个重要极限
- <big>$lim_{x\to\infty}(1+\cfrac{1}{x})^x = e$</big>
- <big>$lim_{x\to\infty}\cfrac{sinx}{x} = 1$</big>

## N次方差公式
$a^n - b^n = (ToBeFinished...)$

## 无穷小的比



