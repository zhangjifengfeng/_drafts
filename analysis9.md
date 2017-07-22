---
title: 实分析第九章
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
设$X$是实直线的子集合，并设$Y$是集合，使得$X\subseteq Y \subseteq  \overline{X}$.证明$\overline{X} = \overline{Y}.$

---
>首先证明，若$X\subseteq Y,则\overline{X} \subseteq \overline{Y}.$
>设$x\in\overline{X}$,根据定义9.1.8可知，对于每个$\varepsilon>0$,都存在$y\in X$使它$\varepsilon-$接近于$x$,同时因为$X \subseteq Y$可知$y\in Y$,所以对于每个$\varepsilon>0$存在$y\in Y$使它$\varepsilon-$接近于$x$,即证$x \in \overline{Y}$.根据子集公理可知,$\overline{X}\subseteq\overline{Y}$成立.
>
>然后证明,设$X$是$\mathbb{R}$的子集,则$\overline{\overline{X}}= \overline{X}$.
>反证,若存在$x\in \overline{\overline{X}}$且$x \notin \overline{X}$,由于$x\in\overline{\overline{X}}$可知对于一切$\varepsilon>0$,存在$y\in\overline{X}$,使$|y-x|\leq \frac{\varepsilon}{2}$,同时由于$y\in\overline{X}$可知对于一切$\varepsilon>0$,存在$z\in X$使$|y-z|\leq \frac{\varepsilon}{2}$,综合两者,对于一切存在$z\in X$存在$y\in \overline{X}$,使$|x-z|=|(y-z)-(y-x)|\leq|y-z|+|y-x|\leq\varepsilon$,即证明$x\in\overline{X}$.这与$x\notin\overline{X}$矛盾.即假设不成立,原命题成立.
>
>最后证明,若$Y \subseteq \overline{X}$,则$\overline{Y}\subseteq\overline{X}$.
>由证明一可知,若$Y\subseteq \overline{X}$,则$\overline{Y}\subseteq\overline{\overline{X}}$.又因为$\overline{X}=\overline{\overline{X}}$,所以$\overline{Y}\subseteq \overline{X}$.即证上述蕴含成立.
>根据外延公理,由第一个证明和第三个证明可知,$\overline{X}=\overline{Y}$.


***
* **9.1.2**
证明引理9.1.11
设$X$和$Y$是$\mathbb{R}$的子集合.那么$ X\subseteq \overline{X},\overline{X\cup Y} = \overline{X}\cup \overline{Y},\overline{X\cap Y}\subseteq \overline{X}\cap \overline{Y}.$如果$X \subseteq Y,$
那么$\overline{X} \subseteq \overline{Y}$.

---
>一、证明$X \subseteq \overline{X}$
>设$x\in X$,根据定义9.1.8,对于$x$下述命题成立:对每个$\varepsilon >0$,都存在$x\in X$使$|x-x|=0 \leq \varepsilon$.所以$x$为X的附着点,即$x\in\overline{X}$.根据子集公理$X\subseteq \overline{X}$.
>
>二、证明$\overline{X \cup Y}=\overline{X} \cup \overline{Y}$
>首先证明$\overline{X\cup Y}\subseteq \overline{X}\cup\overline{Y}$.设$x\in \overline{X\cup Y}$,根据定义9.1.8,对每个$\varepsilon>0$,都存在$z\in X\cup Y$,使$|x-z| \leq \varepsilon$.若$z\in X$,有下述命题成立:对于每个$\varepsilon>0$,都存在$z\in X$,使$|x-z|\leq \varepsilon$.根据定义9.1.8,$x\in\overline{X}$,即$x\in\overline{X}\cup\overline{Y}$.若$x\in Y$,同理也有$x\in\overline{X}\cup\overline{Y}$.即证$\overline{X\cup Y}\subseteq \overline{X}\cup\overline{Y}$成立.
>
>然后证明$\overline{X\cup Y}\supseteq \overline{X}\cup\overline{Y}$.设$x\in\overline{X}\cup\overline{Y}$,若$x\in\overline{X}$,根据定义9.1.8,对每个$\varepsilon>0$,都存在$z\in X$,使$|x-z| \leq \varepsilon$.又因为$z\in X\cup Y$,所以有下述命题成立:对每个$\varepsilon>0$,都存在$z\in X\cup Y$,使$|x-z| \leq \varepsilon$,所以$x\in\overline{X\cup Y}$.若$x\in \overline{Y}$,同理可证$x\in\overline{X \cup Y}$.即证$\overline{X\cup Y}\supseteq \overline{X}\cup\overline{Y}$成立.
>
>根据外延公理,由上述两个证明结果可知$\overline{X \cup Y}=\overline{X} \cup \overline{Y}$成立.
>
>三、证明$\overline{X \cap Y}\subseteq\overline{X}\cap\overline{Y}$
>设$x\in \overline{X\cap Y}$,根据定义9.1.8,对于每个$\varepsilon>0$,存在$z\in X\cap Y$使$|x-z|\leq\varepsilon$.因为$z\in X$,所以有下述命题成立:对每个$\varepsilon>0$,都存在$z\in X$,使$|x-z| \leq \varepsilon$,所以$x\in\overline{X}$.同理又有$x\in\overline{Y}$,即$x\in\overline{X}\cap\overline{Y}$.根据子集公理,证得$\overline{X \cap Y}\subseteq\overline{X}\cap\overline{Y}$.
>
>四、证明如果$X\subseteq Y$,那么$\overline{X}\subseteq\overline{Y}$.
>习题9.1.1第一个证明已证.


***
* **9.1.3**
证明引理9.1.13
$\mathbb{N}$的闭包是$\mathbb{N},\mathbb{Z}$的闭包是$\mathbb{Z},\mathbb{Q}$的闭包是$\mathbb{R},\mathbb{R}$的闭包是$\mathbb{R},$空集$\phi$的闭包是$\phi .$

---
>证明一、$\mathbb{N}$的闭包是$\mathbb{N}$.
>首先证明$\mathbb{N}\subseteq\overline{\mathbb{N}}$,因为$\mathbb{N}\subseteq\mathbb{R}$,根据引理9.1.11,$\mathbb{N}\subseteq\overline{\mathbb{N}}$.
>
>然后证明$\mathbb{N}\subsetneq\overline{\mathbb{N}}$不成立.反证,假设$\mathbb{N}\subsetneq\overline{\mathbb{N}}$成立,则存在$x\in \overline{\mathbb{N}}$,且$x\notin \mathbb{N}$,根据定义9.1.8,对于每个$\varepsilon>0$,都存在$y\in \mathbb{N}$使$|x-y|\leq\varepsilon$,由引理4.1.11(序的性质)可知,若$x,y\in\mathbb{Z},x\neq y$,则$|x-y|\geq 1$.根据该命题的逆反命题可知$x=y$,又因为$y\in\mathbb{N}$所以$x\in\mathbb{N}$,这与假设的$x\notin \mathbb{N}$矛盾.所以假设不成立,即证明目标命题成立.
>
>由上述两个证明可知,$\mathbb{N}\subseteq\overline{\mathbb{N}}$且$\mathbb{N}\subsetneq\overline{\mathbb{N}}$不成立,所以$\mathbb{N}=\overline{\mathbb{N}}$成立.
>
>证明二、$\mathbb{Z}$的闭包是$\mathbb{Z}$.
>该证明和证明一同理.
>
>证明三、$\mathbb{Q}$的闭包是$\mathbb{R}$.
>首先证明$\overline{\mathbb{Q}}\subseteq\mathbb{R}$.设$x\in\overline{\mathbb{Q}}$,根据定义9.1.8,对于每个$\varepsilon >0$,都存在$y\in \mathbb{Q}$它$\varepsilon-$接近$x$.由$\mathbb{Q}\subseteq\mathbb{R}$可知$y\in\mathbb{R}$,根据定义9.1.8,$x\in\overline{\mathbb{R}}$,由证明四可知$\mathbb{R}=\overline{\mathbb{R}}$,所以$x\in\mathbb{R}$,根据子集公理,$\overline{\mathbb{Q}}\subseteq\mathbb{R}$.
>
>然后证明$\overline{\mathbb{Q}}\supseteq\mathbb{R}$.设$x\in\mathbb{R}$,根据实数序的性质可知对于每个$\varepsilon>0$都有$x+\varepsilon>x-\varepsilon$成立,根据命题5.4.14可知可以找到一个比例数$q$使$x- \varepsilon < q < x+\varepsilon$,化简可得$|x-q|<\varepsilon$,根据定义9.1.8,$x\in\overline{\mathbb{Q}}$,根据子集公理,$\overline{\mathbb{Q}}\supseteq\mathbb{R}$成立.
>
>由上述两个证明并根据外延公理可知,$\overline{\mathbb{Q}}=\mathbb{R}$成立.
>
>证明四、$\mathbb{R}$的闭包是$\mathbb{R}$.
>首先证明$\mathbb{R}\subseteq\overline{\mathbb{R}}$,因为$\mathbb{R}\subseteq\mathbb{R}$,根据引理9.1.11,$\mathbb{R}\subseteq\overline{\mathbb{R}}$.
>
>然后证明$\mathbb{R}\supseteq\overline{\mathbb{R}}$,设$x\in\overline{\mathbb{R}}$,根据定义9.1.8可知,$x\in\mathbb{R}$.
>

***
* **9.1.4**
给出实直线的两个自己$X,Y$的例子，使$\overline{X\cap Y}\neq\overline{X}\cap\overline{Y}.$

---
>hello
>world

***
* **9.1.5**
设$X$是$\mathbb{R}$的子集合,并设$x\in\mathbb{R}$,那么$x$是$X$的附着点当且仅当存在一个全由$X$的元素组成的元素组成的序列$(a_n)^{\infty}_{n=0}$,它收敛到$x$.

---
>hello
>world

***
* **9.1.6**
设$X$是$\mathbb{R}$的子集合,证明$\overline{X}$是闭的(即$\overline{\overline{X}} = \overline{X})$.进而证明,如果$Y$是包含$X$的闭集,那么$Y$也包含$\overline{X}$.于是$X$的闭包$\overline{X}$是包含$X$的最小闭集.

---
>hello
>world

***
* **9.1.7**
设$n\geq 1$是正整数,并设$X_1,...,X_n$是$\mathbb{R}$的闭子集.证明$X_1\cup X_2\cup \ ... \ \cup X_n $也是闭的.

---
>hello
>world

***
* **9.1.8**
设$I$是集合(可以是无限的),并且对于每个$\alpha \in I,设X_{\alpha}$是$\mathbb{R}$的闭集.证明交集$\cap _{\alpha \in I}$也是闭的.

---
>hello
>world

***
* **9.1.9**
设$X$是集合实直线的子集合,证明$X$的每个附着点要么是$X$的极限点，要么是$X$的孤立点，但不可得兼.反之,证明$X$的每个极限点和每个孤立点都是$X$的附着点.

---
>hello
>world

***
* **9.1.10**
设X是$\mathbb{R}$的不空子集合,证明$X$是有界的当且仅当$\inf(X)$和$\sup(X)$都是有限的.

---
>hello
>world

***
* **9.1.11**
证明,如果$X$是$\mathbb{R}$的有界子集合,那么闭包$\overline{X}$也是有界的.

---
>hello
>world

***
* **9.1.12**
证明
$\mathbb{R}$的有界子集合的有限族的并集仍是有界集.如果把有限族换为无限族,结论还成立吗?
---
>hello
>world

***
* **9.1.13**
(证明定理9.1.24)设X是$\mathbb{R}$的子集,那么下面两个命题等价:
(a) $X$是闭的并且是有界的.
(b) 任给取值于$X$中的实数序列$(a_n)^\infty_{n=0}$(即对于一切n,$a_n \in X$),存在它的一个子序列($a_{n_j}$),它收敛到$X$中的某数L.

---
>hello
>world

***
* **9.1.14**
证明$\mathbb{R}$的任何有限子集都是闭的并且有界的.

---
>hello
>world

***
* **9.1.15**
设$E$是$\mathbb{R}$的有界子集合,并设$S:=\sup(E)$是E的最小上界.证明$S$是$E$的附着点,并且也是$\mathbb{R}\setminus E$的附着点.

---
>hello
>world

***

---
#### 习题9.2
---

***
* **9.2.1**
设$f:\mathbb{R}\rightarrow \mathbb{R},g:\mathbb{R}\rightarrow \mathbb{R},$下列恒等式中哪些是真的,哪些是假的?对于前者给出证明,对于后者给出反例.
$$
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
设$X$是$\mathbb{R}$的子集合,$f:X\rightarrow \mathbb{R}$是函数,并设$E$是$X$的子集合,$x_0$是$E$的附着点,而$L$是实数,那么下面两命题是逻辑上等价的:
(a)$f$在$x_0$处沿着$E$收敛到$L$.
(b)对于每个完全由$E$的元素组成,并且收敛到$x_0$的序列$(a_n)^\infty_{n=0}$序列$(f(a_n))^\infty_{n=0}$都收敛到$L$.

---
>hello
>world

***
* **9.3.2**
极限的算律
设$X$是$\mathbb{R}$的自己,$E$是$X$的子集,$x_0$是E的附着点,并设$f:X\rightarrow \mathbb{R}$以及$g:X\rightarrow \mathbb{R}$都是函数.假设$f$在$x_0$处沿着$E$有极限$L$,而$g$在$x_0$处沿着$E$有极限$M$.那么
$$
\\ \lim_{x\rightarrow x_0:x \in E}(f+g)(x)=L+M,
\\ \lim_{x\rightarrow x_0:x \in E}(f-g)(x)=L-m,
\\ \lim_{x\rightarrow x_0:x \in E}max(f,g)(x)=max(L,M),
\\ \lim_{x\rightarrow x_0:x \in E}min(f,g)(x)=min(L,M),
\\ \lim_{x\rightarrow x_0:x \in E}(fg)(x)=LM,
\\ \lim_{x\rightarrow x_0:x \in E}(cf)(x)=cL,(x\in \mathbb{R}).
$$
最后，如果$g$在$E$上不取零值(即对于一切$x\in E,g(x)\neq 0$)并且M $\neq 0$,那么
$$ \lim_{x\rightarrow x_0:x \in E}(\frac{f}{g})(x) = \frac{L}{M}.$$

---
>hello
>world

***
* **9.3.3**
设$X$是$\mathbb{R}$的子集合,$E$是$X$的子集合，而$x_0$是$E$的附着点.并设$f:X\rightarrow \mathbb{R}$是函数,$L$是实数.设$\delta > 0$,那么
$$
\\ \lim_{x\rightarrow x_0:x \in E}f(x)=L,当且仅当 \lim_{x\rightarrow x_0:x \in E \cap (x_0-\delta,x_0+\delta)}f(x)=L
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
设$X$是$\mathbb{R}$的子集合,$f:X\rightarrow \mathbb{R}$是函数，并设$x_0$是$X$的元素.那么下面三命题逻辑上等价:
(a)f在$x_0$处连续.
(b)对于由$X$的元素组成的任何收敛到$x_0$的序列$(a_n)^\infty_{n=0}$都有$ \lim_{n\rightarrow \infty}f(a_n)=f(x_0).$
(c)对于每个$\varepsilon >0$都存在$\delta >0,$使得当$x\in X$且$|x-x_0|<\delta$时  $|f(x)-f(x_0)|<\varepsilon.$

---
>hello
>world

***

* **9.4.2**
设$X$是$\mathbb{R}$的子集合,并设$c \in \mathbb{R}$,证明由$f(x):=c $定义的常值函数$f:X \rightarrow  \mathbb{R}$是连续的,并证明由$g(x):=x$定义的恒等函数$g:X\rightarrow \mathbb{R}$也是连续的.

---
>hello
>world

***
* **9.4.3**
设$a>0$是正的实数,那么由$f(x):=a^x$定义的函数$f:\mathbb{R}\rightarrow\mathbb{R}$是连续的.

---
>hello
>world

***
* **9.4.4**
设$p$是实数,那么由$f(x)=x^p$定义的函数$f:(0,\infty)\rightarrow \mathbb{R}$是连续的.

---
>hello
>world

***
* **9.4.5**
设$X$和$Y$是$\mathbb{R}$的子集合,并设$f:X \rightarrow Y,g: Y \rightarrow \mathbb{R}$是函数.设$x_0$是$X$的点,如果$f$在$x_0$处连续,$g$在$f(x_0)$处连续,那么复合函数$g\circ f:X \rightarrow \mathbb{R}$在$x_0$处连续.

---
>hello
>world

***
* **9.4.6**
设$X$是$\mathbb{R}$的子集合,并设$f:X\rightarrow \mathbb{R}$是连续函数，设$Y$是$X$的子集合.
证明$f$在$Y$上的限制$f|_Y :Y\rightarrow \mathbb{R}$也是连续函数.

---
>hello
>world

***
* **9.4.7**
设$n\geq 0$是函数,并且对于每个$0\leq i\leq n$设$c_i$是实数.设$P:\mathbb{R}\rightarrow\mathbb{R}$是函数$$P(x)=\sum_{i=0}^{n}c_i x^i,$$
这样的函数周知为单变量多项式.一个典型的例子是$P(x)=6x^4 -3x^2+4.$证明P是连续的.

---
>hello
>world
***

---
#### 习题9.5
---

***
* **9.5.1**
设$E$是$\mathbb{R}$的子集合,$f:E\rightarrow\mathbb{R}$是函数,并设$x_0$是$E$的附着点.请为极限
$$\lim_{x\rightarrow x_0:x\in E f(x)=\infty(或-\infty)}$$
写一个定义.如果$f:\mathbb{R}\setminus \{0\} \rightarrow \mathbb{R}$是函数$f(x):=\frac{1}{x}$,用你的定义断定$f(0+)=\infty$且$f(0-)=-\infty$.另外对于命题9.3.9当$L=\infty$或$L=-\infty$时的某些类似之事予以叙述和证明.

---
>hello
>world
***

---
#### 习题9.6
---

***
* **9.6.1**
给出如下的例子:
解释一下为什么你构造的例子都不违背最大值原理.
(a)函数$f:(1,2)\rightarrow \mathbb{R}$,它连续并且有界,在某处达到它的最小值,但在任何点处也不达到它的最大值(即没有最大值).
(b)函数$f:[0,\infty)\rightarrow\mathbb{R}$,它连续并且有界,在某处达到它的最大值,但在任何点处也不达到它的最小值（即没有最小值).
(c)函数$f:[-1,1]\rightarrow\mathbb{R}$,它是有界的,但在任何点处也不达到它的最小值,且在任何点处也不达到它的最大值(即没有最大值).
(d)函数$f:[-1,1]\rightarrow\mathbb{R}$,它有上界但无下界.

---
>hello
>world

***

---
#### 习题9.7
---

***
* **9.7.1**
设$a<b$,并设$f:[a,b]\rightarrow\mathbb{R}$是$[a,b]$上的连续函数.设$M:=\sup_{x\in[a,b]}f(x)$是f的最大值,并设$m:=inf_{x\in[a,b]}f(x)$是最小值.如果$y$是介于$m$和$M$之间的实数$(即m\leq y\leq M)$,那么存在$c\in [a,b]$使得$f(c)=y$.进而有$f([a,b])=[m,M]$.

---
>hello
>world

***
* **9.7.2**
设$f:[0,1]\rightarrow[0,1]$是连续函数.证明存在实数$x\in [0,1]$,使$f(x)=x$.$($对于函数$f(x)\rightarrow x$使用中值定理$)$此点$x$叫作$f$的不动点.这个结果是不动点定理的一个基本例子,它在一定类型的分析学问题中起着重要的作用.

---
>hello
>world

***

---
#### 习题9.8
---

***
* **9.8.1**
解释为什么把$f$连续的假定换为$f$单调或严格单调时,最大值原理仍然成立.$($对于单调和严格单调两种情形可用统一解释.$)$

---
>hello
>world

***
* **9.8.2**
举例说明当连续的假定换为单调或严格单调时中值定理不成立.$($对于单调和严格单调两种情况可以使用同一反例.$)$

---
>hello
>world

***
* **9.8.3**
设$a<b$是实数,并设$f:[a,b]\rightarrow\mathbb{R}$是函数.如果$f$既是连续的又是1对1的,那么$f$是严格单调的.

---
>hello
>world

***
* **9.8.4**
设$a<b$是实数,并设$f:[a,b]\rightarrow\mathbb{R}$是函数.如果$f$既是连续的又是严格单调增的,那么$f$是从$[a,b]$到$[f(a),f(b)]$的双射,并且逆映射$f^{-1}:[f(a),f(b)]\rightarrow [a,b]$也是连续的并且严格单调增的.

---
>hello
>world

***
* **9.8.5**
举一个在每个比例数处间断而在每个非比例数处连续的函数的例子.由于比例数集合是可数的,我们把它写成
$$\mathbb{Q}=\{q(0),q(1),q(2),...\}$$
其中$q:\mathbb{N}\rightarrow \mathbb{Q}$是从$\mathbb{N}$到$\mathbb{Q}$的双射.现在定义函数$g:\mathbb{Q}\rightarrow \mathbb{R}$,令
$$g(q(n)):=2^{-n},n\in \mathbb{N}$$
，那么$g$映$q(0)$为$1$,$q(1)$为$2^{-1}$ ,等等.由于级数
$$\sum_{n=0}^{\infty}2^{-n}$$
是绝对收敛的,现在定义函数$f:\mathbb{R}\rightarrow\mathbb{R}$,令
$$f(x):=\sum_{r \in \mathbb{Q}: r< x}g(r)$$
由于
$$\sum_{r \in \mathbb{Q}}g(r)$$
是绝对收敛的,所以$f(x)$对于每个实数$x$都是定义成功的.
(a)证明$f$是严格单调增加的.
(b)证明对于每个比例数$r$,$f$在$r$处间断.
(c)证明对于每个费比例数$x$,$f$在$x$处连续.

---
>hello
>world

***
