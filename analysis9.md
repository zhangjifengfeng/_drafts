---
title: 实分析
tags:
  - 陶哲轩实分析
  - 数学
mathjax: true
date: 2017-07-20 15:31:00
---



### 实分析第九章
---
#### 习题9.1
---

***
* ** 9.1.1 **
$$
设X是实直线的子集合，并设Y是集合，使得
X\subseteq Y \subseteq  \overline{X}
.
\\ 证明\overline{X} = \overline{Y}.
$$

---
> hello
> world

***
* **9.1.2**
证明引理9.1.11
$$
设X和Y是\mathbb{R}的子集合.
\\那么 X\subseteq \overline{X},\overline{X\cup Y} = \overline{X}\cup \overline{Y},\overline{X\cap Y}\subseteq \overline{X}\cap \overline{Y}.
\\ 如果X \subseteq Y,那么\overline{X} \subseteq \overline{Y}.
$$

---
>hello
>world

***
* **9.1.3**
证明引理9.1.13
$$
\mathbb{N}的闭包是\mathbb{N},\mathbb{Z}的闭包是\mathbb{Z},\mathbb{Q}的闭包是\mathbb{R},\mathbb{R}的闭包是\mathbb{R},空集\phi的闭包是\phi .
$$

---
>hello
>world

***
* **9.1.4**
$$
给出实直线的两个自己X,Y的例子，使\overline{X\cap Y}\neq\overline{X}\cap\overline{Y}.
$$

---
>hello
>world

***
* **9.1.5**
$$
设X是\mathbb{R}的子集合,并设x\in\mathbb{R},那么x是X的附着点
\\当且仅当存在一个全由X的元素组成的元素组成的序列(a_n)^{\infty}_{n=0},
\\它收敛到x.
$$

---
>hello
>world

***
* **9.1.6**
$$
设X是\mathbb{R}的子集合,证明\overline{X}是闭的(即\overline{\overline{X}} = \overline{X}).
\\进而证明,如果Y是包含X的闭集,那么Y也包含\overline{X}.
\\于是X的闭包\overline{X}是包含X的最小闭集.
$$

---
>hello
>world

***
* **9.1.7**
$$
设n\geq 1是正整数,并设X_1,...,X_n是\mathbb{R}的闭子集.
\\证明X_1\cup X_2\cup \ ... \ \cup X_n 也是闭的.
$$

---
>hello
>world

***
* **9.1.8**
$$
设I是集合(可以是无限的),并且对于每个\alpha \in I,设X_{\alpha} 是\mathbb{R}的闭集.
\\证明交集\cap _{\alpha \in I}也是闭的.
$$

---
>hello
>world

***
* **9.1.9**
$$
设X是集合实直线的子集合,证明X的每个附着点
\\要么是X的极限点，要么是X的孤立点，但不可得兼.
\\反之,证明X的每个极限点和每个孤立点都是X的附着点.
$$

---
>hello
>world

***
* **9.1.10**
$$
设X是\mathbb{R}的不空子集合,证明X是有界的当且仅当inf(X)和sup(X)都是有限的.
$$

---
>hello
>world

***
* **9.1.11**
证明
$$
如果X是\mathbb{R}的有界子集合,那么闭包\overline{X}也是有界的.
$$

---
>hello
>world

***
* **9.1.12**
证明
$$
\mathbb{R}的有界子集合的有限族的并集仍是有界集.
\\如果把有限族换为无限族,结论还成立吗?
$$
---
>hello
>world

***
* **9.1.13**
证明定理9.1.24
$$
设X是\mathbb{R}的子集,那么下面两个命题等价:
\\(a)\ \ X是闭的并且是有界的.
\\(b)\ \ 任给取值于X中的实数序列(a_n)^\infty_{n=0}(即对于一切n,a_n \in X),
\\存在它的一个子序列(a_{n_j}),它收敛到X中的某数L.
$$

---
>hello
>world

***
* **9.1.14**
$$
证明\mathbb{R}的任何有限子集都是闭的并且有界的.
$$

---
>hello
>world

***
* **9.1.15**
$$
设E是\mathbb{R}的有界子集合,并设S:=sup(E)是E的最小上界.
\\证明S是E的附着点,并且也是\mathbb{R}\setminus E的附着点.
$$

---
>hello
>world

***

---
#### 习题9.2
---

***
* **9.2.1**
$$
设f:\mathbb{R}\rightarrow \mathbb{R},g:\mathbb{R}\rightarrow \mathbb{R},下列恒等式中哪些是真的,哪些是假的?
\\对于前者给出证明,对于后者给出反例.
\\(f+g)\circ h=(f\circ h)+(g\circ h),
\\f\circ (g+h)=(f\circ g)+(f\circ h),
\\(f+g)h=(fh)+(gh),
\\f(g+h)=(fg)+(fh).
$$

---
>hello
>world

***

---
#### 习题9.3
---

***
* **9.3.1**
$$
设X是\mathbb{R}的子集合,f:X\rightarrow \mathbb{R}是函数,并设E是X的子集合,x_0是E的附着点,而L是实数,
\\那么下面两命题是逻辑上等价的:
\\(a)f在x_0处沿着E收敛到L.
\\(b)对于每个完全由E的元素组成,
\\并且收敛到x_0的序列(a_n)^\infty_{n=0}序列(f(a_n))^\infty_{n=0}都收敛到L.
$$

---
>hello
>world

***
* **9.3.2**
极限的算律
$$
设X是\mathbb{R}的自己,E是X的子集,x_0是E的附着点,
\\并设f:X\rightarrow \mathbb{R}以及g:X\rightarrow \mathbb{R}都是函数.
\\假设f在x_0处沿着E有极限L,而g在x_0处沿着E有极限M.那么
\\ \lim_{x\rightarrow x_0:x \in E}(f+g)(x)=L+M,
\\ \lim_{x\rightarrow x_0:x \in E}(f-g)(x)=L-m,
\\ \lim_{x\rightarrow x_0:x \in E}max(f,g)(x)=max(L,M),
\\ \lim_{x\rightarrow x_0:x \in E}min(f,g)(x)=min(L,M),
\\ \lim_{x\rightarrow x_0:x \in E}(fg)(x)=LM,
\\ \lim_{x\rightarrow x_0:x \in E}(cf)(x)=cL,(x\in \mathbb{R}).
\\最后，如果g在E上不取零值(即对于一切x\in E,g(x)\neq 0)并且M \neq 0,那么
\\ \lim_{x\rightarrow x_0:x \in E}(\frac{f}{g})(x) = \frac{L}{M}.
$$

---
>hello
>world

***
* **9.3.3**
极限是局部的
$$
设X是\mathbb{R}的子集合,E是X的子集合，而x_0是E的附着点.
\\并设f:X\rightarrow \mathbb{R}是函数,L是实数.
设\delta > 0,那么
\\ \lim_{x\rightarrow x_0:x \in E}f(x)=L,
\\当且仅当
\\ \lim_{x\rightarrow x_0:x \in E \cap (x_0-\delta,x_0+\delta)}f(x)=L
$$

---
>hello
>world

***

---
#### 习题9.4
---
***
* **9.4.1**
连续性的等价表述
$$
设X是\mathbb{R}的子集合,f:X\rightarrow \mathbb{R}是函数，并设x_0是X的元素.
\\那么下面三命题逻辑上等价:
\\(a)f在x_0处连续.
\\(b)对于由X的元素组成的任何收敛到x_0的序列(a_n)^\infty_{n=0}都有
\\ \lim_{n\rightarrow \infty}f(a_n)=f(x_0).
\\(c)对于每个\varepsilon >0都存在\delta >0,使得当x\in X且|x-x_0|<\delta时
\\ |f(x)-f(x_0)<\varepsilon.
$$

---
>hello
>world

***

* **9.4.2**
$$
设X是\mathbb{R}的子集合,
\\并设c \in \mathbb{R},证明由f(x):=c 定义的常值函数f:X \rightarrow  \mathbb{R}是连续的,
\\并证明由g(x):=x定义的恒等函数g:X\rightarrow \mathbb{R}也是连续的.
$$

---
>hello
>world

***
* **9.4.3**
$$
设a>0是正的实数,那么由f(x):=a^x定义的函数f:\mathbb{R}\rightarrow\mathbb{R}是连续的.
$$

---
>hello
>world

***
* **9.4.4**
$$
设p是实数,那么由f(x)=x^p定义的函数f:(0,\infty)\rightarrow \mathbb{R}是连续的.
$$

---
>hello
>world

***
* **9.4.5**
$$
设X和Y是\mathbb{R}的子集合,并设f:X \rightarrow Y,g: Y \rightarrow \mathbb{R}是函数.
\\设x_0是X的点,如果f在x_0处连续,g在f(x_0)处连续,
\\那么复合函数g\circ f:X \rightarrow \mathbb{R}在x_0处连续.
$$

---
>hello
>world

***
* **9.4.6**
$$
设X是\mathbb{R}的子集合,并设f:X\rightarrow \mathbb{R}是连续函数，设Y是X的子集合.
\\证明f在Y上的限制f|_Y :Y\rightarrow \mathbb{R}也是连续函数.
$$

---
>hello
>world

***
* **9.4.7**
$$
设n\geq 0是函数,并且对于每个0\leq i\leq n设c_i是实数.
\\设P:\mathbb{R}\rightarrow\mathbb{R}是函数P(x)=\sum_{i=0}^{n}c_i x^i,
\\这样的函数周知为单变量多项式.一个典型的例子是P(x)=6x^4 -3x^2+4.
\\证明P是连续的.
$$

---
>hello
>world
***

---
#### 习题9.4
---
***
* **9.5.1**
