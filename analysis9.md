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

>证明五、$\phi$的闭包是$\phi$.

>首先证明$\phi\subseteq\overline{\phi}$,因为命题$x\in\phi$为假命题,所以命题:若$x\in\phi$,则$x\in\overline{\phi}$为真空蕴含,即此命题成立.

>

>然后证明$\overline{\phi}\subseteq\phi$,根据定义9.1.8,对于每个$\varepsilon>0$,存在$x\in\phi$使它$\varepsilon-$接近$x$,因为$x\in\phi$为假命题,所以不存在$x\in\phi$使它$\varepsilon-$接近$x$,所以$x\in\overline{\phi}$为假,所以命题;若$x\in\overline{\phi}$,则$x\in\phi$为真空蕴含,即此命题成立.




***

* **9.1.4**

给出实直线的两个自己$X,Y$的例子，使$\overline{X\cap Y}\neq\overline{X}\cap\overline{Y}.$




---

>如$X=[0,1) Y=(1,2]$,$\overline{X\cap Y} = \overline{\phi} = \phi$,而$\overline{X}\cap\overline{Y} = [0,1]\cap[1,2] = {1}$,此时$\overline{X\cap Y}\neq\overline{X}\cap\overline{Y}.$

>




***

* **9.1.5**

设$X$是$\mathbb{R}$的子集合,并设$x\in\mathbb{R}$,那么$x$是$X$的附着点当且仅当存在一个全由$X$的元素组成的元素组成的序列$(a_n)^{\infty}_{n=0}$,它收敛到$x$.




---

>首先证明若$x$是$X$的附着点,则存在一个全由$X$的元素组成的序列$(a_n)_{n=0}^{\infty}$,它收敛到$x$.首先构造集合$X_n=\{y|y\in X,|x-y|\leq \frac{1}{n}\}$,因为$x$是$X$的附着点,根据定义9.1.8可知,$X_n$不为空集,再根据选择公理可知,可以找到一个序列$(a_n)_{n=0}^{\infty}$,使得对一切$n\leq 1,a_n\in X_n$.同时因为对每一个$a_n$都有$|a_n-x|\leq\frac{1}{n}$即$x-\varepsilon\leq a_n \leq x+\varepsilon$,因为$\lim_{n\rightarrow\infty}(x-\varepsilon) =\lim_{n\rightarrow\infty}(x+\varepsilon) = x$,根据推论6.4.14(挤压判别法),序列$(a_n)_{n=0}^{\infty}$收敛至$x$.即证目标命题成立.

>

>然后证明若存在一个有$X$的元素组成的序列$(a_n)_{n=0}^{\infty}$它收敛到$x$,则$x$是$X$的附着点.已知序列$(a_n)_{n=0}^{\infty}$收敛到$x$,所以序列$(a_n - x)_{n=0}^{\infty}$收敛到$0$,即对每个$\varepsilon>0$存在$N>0$,当$n>N$时$|a_n-x-0|<\varepsilon$成立.因为$a_n\in X$,所以对于每个$\varepsilon>0$都有存在一个$a_n\in X$使$|a_n-x|<\varepsilon$成立.根据定义9.1.8,$x$是$X$的附着点.

>




***

* **9.1.6**

设$X$是$\mathbb{R}$的子集合,证明$\overline{X}$是闭的(即$\overline{\overline{X}} = \overline{X})$.进而证明,如果$Y$是包含$X$的闭集,那么$Y$也包含$\overline{X}$.于是$X$的闭包$\overline{X}$是包含$X$的最小闭集.




---

>证明一、$\overline{X}$是闭的.

>证明见习题9.1.1的第二个证明.

>

>证明二、如果$Y$是包含$X$的闭集,那么$Y$也包含$\overline{X}$.(注意:包含$X$的是用来修饰闭集的)

>已知$Y\subseteq X$,由引理9.1.11可知,$\overline{Y}\subseteq\overline{X}$,又因为$Y$是闭集可知$\overline{Y} = Y$,所以可得$Y\subseteq\overline{X}$.即证目标命题成立.

>




***

* **9.1.7**

设$n\geq 1$是正整数,并设$X_1,...,X_n$是$\mathbb{R}$的闭子集.证明$X_1\cup X_2\cup \ ... \ \cup X_n $也是闭的.




---

>使用归纳法即可证明,首先对于$n=1$时根据题设可知$X_1$是闭的.然后假设对于$n$时目标命题也成立(即$X_1\cup X_2\cup \ ... \ \cup X_n$也是闭的),最后对于$n+1$,设$Y=X_1\cup X_2\cup \ ... \ \cup X_n$,由引理9.1.11可知, $\overline{Y\cup X_{n+1}} = \overline{X_{n+1}} \cup \overline{Y}$,因为$Y$是闭的且$X_n$也是闭的可知$Y=\overline{Y},X_{n+1}=\overline{X_{n+1}}$,所以$\overline{Y\cup X_{n+1}} = Y\cup X_{n+1}$,即证$Y\cup X_{n+1}$也是闭的.综上归纳可知目标命题成立.

>




***

* **9.1.8**

设$I$是集合(可以是无限的),并且对于每个$\alpha \in I,设X_{\alpha}$是$\mathbb{R}$的闭集.证明交集$\cap _{\alpha \in I}$也是闭的.




---

>反证法,设$Y=\cap_{\alpha \in I} X_{\alpha}$,若$\cap_{\alpha \in I} X_{\alpha}$不是闭的,即存在$x\in\overline{Y}$且$x\notin Y$.因为$Y$是所有$x_{\alpha}$的交集可知对每一个$X_{\alpha}$都有$x\notin X_{\alpha}$且$x\in \overline{X_\alpha}$,所以$X_{\alpha}$不是闭的,这与题设$X_{\alpha}$是闭的矛盾.所以原命题成立.

>




***

* **9.1.9**

设$X$是集合实直线的子集合,证明$X$的每个附着点要么是$X$的极限点，要么是$X$的孤立点，但不可得兼.反之,证明$X$的每个极限点和每个孤立点都是$X$的附着点.




---

>反证法,若X的附着点中存在附着点$x_0$它既是$X$的极限点又是$X$的孤立点 或者  它既不是$X$的极限点又是$X$的孤立点.

>先看第一部分:它既是$X$的极限点又是$X$的孤立点.因为$x_0$是$X$的极限点所以$x$是$X|\{x\}$的附着点,的附着点,又因为$x_0$又是$X$的孤立点所以$x$不是$X|\{x\}$的附着点,两者存在矛盾.

>

>第二部分证明和第一部分同理.

>




***

* **9.1.10**

设X是$\mathbb{R}$的不空子集合,证明$X$是有界的当且仅当$\inf(X)$和$\sup(X)$都是有限的.




---

>首先证明若$X$是有界的,则$\inf(X)$和$\sup(X)$都是有限的.因为$X$是有界的根据定义9.1.22可知存在某个实数$M>0$,$X\subseteq [-M,M]$,根据定义5.5.5,可知$\inf(X)\leq \sup(X)\leq M$且$\sup(X)\geq\inf(X)\geq -M$,所以$\sup(X)\in R \inf(X)\in R$(反证法可证此蕴含),根据定义6.2.1,$\sup(X)$和$\inf(X)$都是有限的.

>

>然后证明若$\inf(X)$和$\sup(X)$都是有限的,则$X$是有界的.取$M=max(|\inf(X)|,|\sup(X)|)$,因为$\inf(X)$和$\sup(X)$都是有限的可知$\inf(X)\in R,\sup(X)\in R$,所以$M\in R$且对任意$x\in X$有$-M\leq \inf(X) \leq x \leq \sup(x) \leq M$,根据定义9.1.22可知$X$是有界的.

>







***

* **9.1.11**

证明,如果$X$是$\mathbb{R}$的有界子集合,那么闭包$\overline{X}$也是有界的.




---

>因为$X$是$\mathbb{R}$的有界集合,根据定义9.1.22可知存在实数$M>0,X\subseteq [-M,M]$,由引理9.1.11可知$\overline{X}\subseteq\overline{[-M,M]}=[-M,M]$,所以闭包$\overline{X}$也是有界的.

>




***

* **9.1.12**

证明

$\mathbb{R}$的有界子集合的有限族的并集仍是有界集.如果把有限族换为无限族,结论还成立吗?

---

>设存在有限族$(X_\alpha)_{\alpha\in I})$,因为有限族的每个集合都是$\mathbb{R}$的有界子集合,所以对于每个集合$X_\alpha$存在实数$M_\alpha >0$使$X_\alpha \subseteq [-M_\alpha,M_\alpha]$,取$M=\sup(\{M_\alpha|\alpha\in I\}$,即有$\cup_{\alpha\in I}X_\alpha\subseteq [-M,M]$,根据定义9.1.22可知其并集仍是有界集.

>

>如果把有限族换为无限族结论还成立吗?

>不成立,反例构造证明,若构造无限族中的集合为$X_\alpha = \{\alpha\}$,其并集为$\cup_{\alpha\in \mathbb{N}}X_\alpha = \mathbb{N}$,因为$\mathbb{N}$为无界集,所以命题在此前提下不成立.

>




***

* **9.1.13**

(证明定理9.1.24)设X是$\mathbb{R}$的子集,那么下面两个命题等价:

(a) $X$是闭的并且是有界的.

(b) 任给取值于$X$中的实数序列$(a_n)^\infty_{n=0}$(即对于一切n,$a_n \in X$),存在它的一个子序列($a_{n_j}$),它收敛到$X$中的某数L.




---

>证明一、$(a)\rightarrow (b)$

>设$(a_n)_{n=0}^\infty$为取值于X中的实数序列,因为$X$是有界的所以存在实数$M>0$使任意$x\in X$都有$-M\leq x\leq M$即对每个$a_n$有$-M\leq a_n \leq M$,所以$(a_n)_{n=0}^\infty$也是有界的,由定理6.8.8可知$(a_n)_{n=0}^\infty$至少有一个子序列$(a_i)_{n=0}^\infty$收敛,又因为$X$是闭的,由推论9.1.17可知,$\lim_{n->\infty} a_n \in X$,即存在某数$L\in X$,$(a_i)_{i=0}^\infty$收敛到X中的某数L.

>

>证明二、$(b)\rightarrow (a)$

>首先证明$X$是闭的,已知任给取值于$X$中的实数序列$(a_n)^\infty_{n=0}$,存在一个子序列$(a_i)_{i=0}^\infty$,它收敛到$X$中的某数$L$.由推论9.1.17可知,$X$是闭的.

>

>然后证明$X$是有界的,(主要考察$\sup(X)$不为$\infty$)构造$X_n=\{x\in X:\sup(X)-\frac{1}{n}\leq x \leq \sup(X)\}$由$X$为实数集根据定理5.5.9可知存在$\sup(X)$,所以集合$X_n$不为空集,使用选择公理可以找到一个序列$(a_n)_{n=0}^\infty$其中对于一切$n\geq 1$有$a_n\in X_n$,所以有对于一切$n>0$,$a_n\in X$并且$\sup(X)-\frac{1}{n} \leq a_n \leq \sup(X)$由推论6.4.14可知,$\lim_{n\rightarrow\infty} a_n = \sup(X)$,由命题$b$可知$\sup(X)\in X$,因为$X\subseteq \mathbb{R}$所以$\sup(X) \in \mathbb{R}$,同理可证$\inf(X)\in\mathbb{R}$.取$M=max(|inf(X)|,|sup(X)|)$,$X \in [-M,M]$,根据定义9.1.22可知,$X$是有界的.

>




***

* **9.1.14**

证明$\mathbb{R}$的任何有限子集都是闭的并且有界的.




---

>设$X$为$\mathbb{R}$的子集,由命题条件可知$X$是有限的,即存在双射函数$f:N\rightarrow X$且$N\in\mathbb{N}$,不妨构造双射函数$f$为$f(n) = \{a_n\}$其中$n\in N,a_n\in X$,一方面,根据定义9.1.10可知$a_n$是闭集,再由习题9.1.7可知$\cup_{n\in N}(\{a_n\})$为闭集.另一方面,由定义9.1.22可知$\{a_n\}$是有界的,根据双射函数$f$构造有限族$(\{a_n\})_{n\in N}$,根据习题9.1.12可知$\cup_{n\in N}(\{a_n\})$是有界集.即证目标命题成立.

>




***

* **9.1.15**

设$E$是$\mathbb{R}$的有界子集合,并设$S:=\sup(E)$是$E$的最小上界.证明$S$是$E$的附着点,并且也是$\mathbb{R}\setminus E$的附着点.




---

>证明一、$S$是$E$的附着点,可以构造$X_n=\{x\in E:\sup(E)-\frac{1}{n}\leq x \leq \sup(E)\}$由$E$为实数集根据定理5.5.9可知存在$\sup(E)$,所以集合$X_n$不为空集,使用选择公理可以找到一个序列$(a_n)_{n=0}^\infty$其中对于一切$n\geq 1$有$a_n\in X_n$,所以有对于一切$n>0$,$a_n\in E$并且$\sup(E)-\frac{1}{n} \leq a_n \leq \sup(E)$由推论6.4.14可知,$\lim_{n\rightarrow\infty} a_n = \sup(E)$,由引理9.1.14可知$\sup(E)$为$E$的附着点.

>

>证明二、$S$是$\mathbb{R}\setminus E$的附着点.可以构造$X_n=\{x\in E:\sup(E)+\frac{1}{n}\geq x \geq \sup(E)\}$,证明方法和证明一同理.

>




***




---

#### 习题9.2

---




***

* **9.2.1**

设$f:\mathbb{R}\rightarrow \mathbb{R},g:\mathbb{R}\rightarrow \mathbb{R},$下列恒等式中哪些是真的,哪些是假的?对于前者给出证明,对于后者给出反例.

$$
(f+g)\circ h=(f\circ h)+(g\circ h),
\\f\circ (g+h)=(f\circ g)+(f\circ h),
\\(f+g)h=(fh)+(gh),
\\f(g+h)=(fg)+(fh).
$$


---

>证明一、$(f+g)\circ h=(f\circ h)+(g\circ h)$为真.

>因为f与g有相同的定义域,由定义9.2.1可知,$(f+g)(x) = f(x)+g(x)$,因为f和g的定义域和h的值域是用一个集合,且根据定义3.3.10可知$(f+g)(h(x)) = (f+g)\circ h(x)$$= f(h(x)) + g(h(x)) = f\circ h(x) + g\circ h(x)$即证$(f+g) \circ  h = (f\circ h) + (g\circ h)$.

>

>证明二、$f\circ (g+h)=(f\circ g)+(f\circ h)$为假.

>反例构造,若$f=x^2 f:\mathbb{R}\rightarrow\mathbb{R}$且$g=x g:\mathbb{R}\rightarrow\mathbb{R}$且$h=\frac{x}{2} h:\mathbb{R}\rightarrow\mathbb{R}$,则$f\circ (g+h) = \frac{9}{4} x^2$,$f\circ h + f\circ g = \frac{5}{4}x^2$,此时$f\circ (g+h) \neq (f\circ g)+(f\circ h)$

>

>证明三、$(f+g)h=(fh)+(gh)$为真.

>设$x\in \mathbb{R}$,由定义9.2.1可知$(f+g)h(x) = (f(x)+g(x))h(x)$,因为$f(x),g(x),h(x)\in \mathbb{R}$所以根据命题5.3.11(实数的运算律)可知$(f(x)+g(x))h(x) = f(x)h(x)+g(x)h(x)$即有$(f+g)h(x) = f(x)h(x)+g(x)h(x)$.再根据定义9.2.1可知$(f+g)h(x) = fh(x)+gh(x)$.即证$(f+g)h=fh+gh$.(可由$(x,(f+g)h(x))\in (f+g)h$和$(x,fh(x)+gh(x)) \in (fh+gh)$结合外延公理可证最后一步,证明一的最后一步也如此).

>

>证明四、$f(g+h)=(fg)+(fh)$为真.

>设$x\in \mathbb{R}$,由定义9.2.1可知$f(g+h)(x) = f(x)(g(x)+h(x))$,因为$f(x),g(x),h(x)\in \mathbb{R}$所以根据命题5.3.11(实数的运算律)可知$f(x)(g(x)+h(x)) = f(x)g(x)+f(x)h(x)$即有$f(g+h)(x) = f(x)h(x)+f(x)g(x)$.再根据定义9.2.1可知$f(g+h)(x) = fg(x)+fh(x)$.即证$f(g+h) = fg+fh$.

>

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

>首先证明$(a)\rightarrow(b)$.

>设$(a_n)_{n=0}^\infty$为任意一个完全由$E$的元素组成且收敛到$x_0$的序列~~并且设$Y=\cup_{n\in\mathbb{N}}\{a_n\}$~~,因为$f$在$x_0$处沿着$E$收敛到$L$可知对于每个$\varepsilon>0$,存在$\delta>0$,使得当$f$限制在集合$\{x\in E:|x-x_0|<\delta\}$上是$\varepsilon-$接近于$L$的.又因为序列$(a_n)_{n=0}^\infty$收敛到$x_0$,所以对于每个$\delta>0$都存在$N>0$当$n>N$时有$|a_n-x_0|\leq \delta$,所以对于每个$\varepsilon>0$,存在$N>0$当使得当$f$限制在集合$\{a_n|n>N\}$上是$\varepsilon-$接近于$L$的.即对于于每个$\varepsilon>0$,存在$N>0$当$n>N$时$f(a_n)$是$\varepsilon-$接近于$L$的.所以命题(b)成立.

>

>然后证明$(b)\rightarrow(a)$.

>反证:若$f$在$x_0$处沿着$E$不能收敛到$L$.则存在$\varepsilon_0>0$,此时不存在$\delta>0$,使得当$f$限制在集合$\{x\in E:|x-x_0|<\delta\}$上是$\varepsilon_0-$接近于$L$的.由命题(b)可知对于$\varepsilon_0>0$,存在$N>0$当$n>N$时$f(a_n)$是$\varepsilon_0-$接近于$L$的.即存在$\delta>0$使$a_n\in \{x\in E:|x-x_0|<\delta\}$.两者矛盾.所以原命题成立.

>




***

* **9.3.2**

极限的算律

设$X$是$\mathbb{R}$的自己,$E$是$X$的子集,$x_0$是E的附着点,并设$f:X\rightarrow \mathbb{R}$以及$g:X\rightarrow \mathbb{R}$都是函数.假设$f$在$x_0$处沿着$E$有极限$L$,而$g$在$x_0$处沿着$E$有极限$M$.那么

$$
   \lim_{x\rightarrow x_0:x \in E}(f+g)(x)=L+M,
\\ \lim_{x\rightarrow x_0:x \in E}(f-g)(x)=L-m,
\\ \lim_{x\rightarrow x_0:x \in E}max(f,g)(x)=max(L,M),
\\ \lim_{x\rightarrow x_0:x \in E}min(f,g)(x)=min(L,M),
\\ \lim_{x\rightarrow x_0:x \in E}(fg)(x)=LM,
\\ \lim_{x\rightarrow x_0:x \in E}(cf)(x)=cL,(x\in \mathbb{R}).
$$

最后，如果$g$在$E$上不取零值(即对于一切$x\in E,g(x)\neq 0$)并且M $\neq 0$,那么

$$ \lim_{x\rightarrow x_0:x \in E}(\frac{f}{g})(x) = \frac{L}{M}.$$




---

>证明一、$ \lim_{x\rightarrow x_0:x \in E}(f+g)(x)=L+M $.

>由于$x_0$是$E$的附着点,根据引理9.1.14,我们知道有一个有E的元素组成的序列$(a_n)_{n=0}^\infty$收敛到$x_0$,由于$f$在$x_0$处沿着$E$收敛到$L$,所以根据命题9.3.9可知$(f(a_n))_{n=0}^\infty$收敛到$L$.类似地可证$(g(a_n))_{n=0}^\infty$收敛到$M$,根据序列的极限算律定理6.1.19可知$((f-g)(a_n))_{n=0}^\infty$收敛到$L-M$再根据命题9.3.9所以$f-g$在$x_0$处沿着$E$有极限$L-M$.

>

>剩下几个命题证明与证明一类似.




***

* **9.3.3**

设$X$是$\mathbb{R}$的子集合,$E$是$X$的子集合，而$x_0$是$E$的附着点.并设$f:X\rightarrow \mathbb{R}$是函数,$L$是实数.设$\delta > 0$,那么

$$
\\ \lim_{x\rightarrow x_0:x \in E}f(x)=L,当且仅当 \lim_{x\rightarrow x_0:x \in E \cap (x_0-\delta,x_0+\delta)}f(x)=L
$$

---

>首先证明$若\lim_{x\rightarrow x_0:x \in E}f(x)=L则 \lim_{x\rightarrow x_0:x \in E \cap (x_0-\delta,x_0+\delta)}f(x)=L$

>反证:若$ \lim_{x\rightarrow x_0:x \in E \cap (x_0-\delta,x_0+\delta)}f(x)= M$且$M \neq L$,由第二部分的证明可知$\lim_{x\rightarrow x_0:x \in E}f(x)=M$,因为$L\neq M$这与$\lim_{x\rightarrow x_0:x \in E}f(x)=L$矛盾.即证原命题成立.

>

>然后证明$若\lim_{x\rightarrow x_0:x \in E \cap (x_0-\delta,x_0+\delta)}f(x)=L$则$\lim_{x\rightarrow x_0:x \in E}f(x)=L$

>已知$\lim_{x\rightarrow x_0:x \in E \cap (x_0-\delta,x_0+\delta)}f(x)=L$,所以对于每个$\varepsilon>0$存在$\delta_0>0$使得当$f$限制在集合$\{x\in  E \cap (x_0-\delta,x_0+\delta):|x-x_0|<\delta_0\}$上是$\varepsilon-$接近于$L$的.因为$E \supsetneq  E \cap (x_0-\delta,x_0+\delta)$,所以有对于每个$\varepsilon>0$存在$\delta_0>0$使得当$f$限制在集合$\{x\in E:|x-x_0|<\delta_0\}$上是$\varepsilon-$接近于$L$的,即证$\lim_{x\rightarrow x_0:x \in E}f(x)=L$,

>




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

>首先证明$(a)\rightarrow(b)$.

>由(a)可知$f$在$x_0$处连续,根据定义(9.4.1)可知,当$x$在$X$中收敛到$x_0$时$f(x)$的极限存在并且等于$f(x_0)$.由命题9.3.9可知,对于$X$的元素组成的任何收敛到$x_0$的序列$(a_n)^\infty_{n=0}$ 都有 $\lim_{n\rightarrow \infty}f(a_n)= f(x_0)$.

>

>然后证明$(b)\rightarrow(c)$

>由命题9.3.9可知,$f$在$x_0$处沿着$X$收敛到$f(x_0)$,再由定义9.3.6可知,对每个$\varepsilon>0$,$f|_X$都是在$x_0$附近$\varepsilon-$接近于$f(x_0)$即对于每个$\varepsilon>0$存在$\delta>0$使得当$f$限制在集合$\{x\in X:|x-x_0|<\delta\}$上$|f(x)-f(x_0)|<\varepsilon$.

>

>最后证明$(c)\rightarrow(a)$

>由定义9.3.6可知,$f$在$x_0$处沿着$X$收敛到$f(x_0)$由定义9.4.1可知$f$在$x_0$处连续.

>




***




* **9.4.2**

设$X$是$\mathbb{R}$的子集合,并设$c \in \mathbb{R}$,证明由$f(x):=c $定义的常值函数$f:X \rightarrow  \mathbb{R}$是连续的,并证明由$g(x):=x$定义的恒等函数$g:X\rightarrow \mathbb{R}$也是连续的.




---

>

>首先证明$f(x):=c$定义的常值函数$f:X \rightarrow  \mathbb{R}$是连续的.

>对任意$x_0\in X$,因为对$x\in X$都有$|f(x)-f(x_0)|=0$,所以有对每个$\varepsilon>0$取任意$x\in X$都有$|f(x)-f(x_0)|<\varepsilon$,即对任意$x_0\in X$根据定义9.3.6,$f$在$x_0$处沿着$X$收敛到$f(x_0)$,再根据定义9.4.1可知,常值函数$f:X \rightarrow  \mathbb{R}$是连续的.

>

>然后证明$f(x):=x$定义的恒等函数$f:X \rightarrow  \mathbb{R}$是连续的.

>对任意$x_0\in X$对于每个$\varepsilon>0$为使$|f(x)-f(x_0)|=|x-x_0|<\varepsilon$成立,只需$\delta=\varepsilon$使$x\in X$且$|x-x_0|<\delta$.即存在$\delta>0$,使得当$x\in X$且$|x-x_0|<\delta$根据命题9.4.7,$f$在$x_0$处连续.此时有对于任意$x_0\in X$有$f$在$x_0$处连续.根据定义9.4.1可知,$f(x):=x$定义的恒等函数$f:X \rightarrow  \mathbb{R}$是连续的.

>




***

* **9.4.3**

设$a>0$是正的实数,那么由$f(x):=a^x$定义的函数$f:\mathbb{R}\rightarrow\mathbb{R}$是连续的.




---

>首先证明$a^x$在零点处连续,由命题9.3.18可知极限是局部的,为考察零点处的连续性不妨设$0<x< \frac{1}{n}$,$n$为正整数,所以有$a^0< a^x< a^{\frac{1}{n}}$因为$a^0=1$且由命题6.5.3可知$\lim_{n\rightarrow\infty}a^{\frac{1}{n}} = 1$根据命题6.4.14可知,$\lim_{x\rightarrow 0^{+} }a^x = 1$同理可证$\lim_{x\rightarrow 0^{-}} a^x = 1$,所以$a^x$在零点处连续.

>

>然后证明$a^x$在$\mathbb{R}$上连续,对于任意$x_0\in\mathbb{R}$根据命题6.7.3极限算律可知因为$\lim{x\rightarrow x_0}(a^x -a^{x_0})$$=a^x_0 \lim{x\rightarrow x_0}(a^(x-x_0) -1)$令$t=x-x_0$则有$\lim{t\rightarrow 0}(a^t -1)$又因为$\lim_{t\rightarrow 0}a^t = 1$所以$\lim{t\rightarrow 0}(a^t -1) = 0$所以有$\lim{x\rightarrow x_0}a^x = a^{x_0}$所以$a^x$在$x_0$处连续.根据定义9.4.1可知,$a^x$在$\mathbb{R}$上连续.

>




***

* **9.4.4**

设$p$是实数,那么由$f(x)=x^p$定义的函数$f:(0,\infty)\rightarrow \mathbb{R}$是连续的.




---

>首先归纳证明$\lim_{x\rightarrow 1}x^n = 1$,对于$n=1$由习题9.4.2可知$\lim_{x\rightarrow 1}x=1$,然后假设对于$n$,有$\lim_{x\rightarrow 1}x^n = 1$,对于$n+1$由命题6.7.3可知$\lim_{x\rightarrow 1}x^{n+1} = \lim_{x\rightarrow 1}x^n . \lim_{x\rightarrow 1}x = 1$所以归纳可知$\lim_{x\rightarrow 1}x^n = 1$

>

>然后证明$x^p$在$x=1$处连续.对于实数$p$,由命题习题5.4.3可知存在整数$m$使$m \leq p < m+1$,并且当$0 < x<1$时有$x^m\leq x^p\leq x^{m+1}$当$x\geq 1$时有$x^{m+1}\leq x^p\leq x^m$因为$\lim_{x\rightarrow 1}x^m = 1$且$\lim_{x\rightarrow 1}x^{m+1} = 1$根据命题6.1.14可知,$\lim{x\rightarrow 1}x^p = 1$.

>

>最后证明$x^p$在$\mathbb{R}$上连续,设$x_0\in\mathbb{R}$根据命题6.7.3可知,$\lim_{x\rightarrow x_0}(x^p-x_0^p) $$= x_0^p \lim_{x\rightarrow x_0}(\frac{x^p}{x^p_0} - 1)$令$t=\frac{x}{x_0}$所以有$x_0^p \lim_{t\rightarrow 1}(t^p -1)$由第二个证明可知$\lim{t\rightarrow 1}t^p = 1$所以$x_0^p \lim_{t\rightarrow 1}(t^p -1) = x_0^p.0 = 0$,$\lim_{x\rightarrow x_0}x^p = x^p_0$,根据定义9.4.1可知,$x^p$在$\mathbb{R}$上连续.

>




***

* **9.4.5**

设$X$和$Y$是$\mathbb{R}$的子集合,并设$f:X \rightarrow Y,g: Y \rightarrow \mathbb{R}$是函数.设$x_0$是$X$的点,如果$f$在$x_0$处连续,$g$在$f(x_0)$处连续,那么复合函数$g\circ f:X \rightarrow \mathbb{R}$在$x_0$处连续.




---

>因为$g$在$f(x_0)$处连续根据定义9.4.1可知,对于每个$\varepsilon>0$存在$\delta>0$使当$f(x)\in Y$且$|f(x)-f(x_0)|<\delta$有$|g(f(x))-g(f(x_0))|<\varepsilon$.又因为$f$在$x_0$处连续所以对于任意$\delta>0$有存在$\delta_1>0$使当$x \in X$且$|x-x_0|<\delta_1$有$|f(x)-f(x_0)|<\delta$.所以有对于每个$\varepsilon>0$存在$\delta_1>0$使当$x \in X$且$|x-x_0|<\delta_1$有$|g(f(x))-g(f(x_0))|<\varepsilon$.根据定义9.4.1可知,复合函数$g\circ f:X \rightarrow \mathbb{R}$在$x_0$处连续.

>




***

* **9.4.6**

设$X$是$\mathbb{R}$的子集合,并设$f:X\rightarrow \mathbb{R}$是连续函数，设$Y$是$X$的子集合.

证明$f$在$Y$上的限制$f|_Y :Y\rightarrow \mathbb{R}$也是连续函数.




---

>设$y_0\in Y$,因为$y_0\in X$且$f:x\rightarrow \mathbb{R}$是连续函数,根据定义9.4.1可知,有对于每个$\varepsilon>0$存在$\delta>0$使当$x\in X$且$|x-y_0|<\delta$有$|f(x)-f(y_0)|\leq \varepsilon$.因为$y_0\in \{x\in X:|x-y_0|<\delta\}$且$y_0\in \{y \in Y:|y-y_0|<\delta\}$,所以$\{y \in Y:|y-y_0|<\delta\} \neq \phi$(存在),又因为$\{x\in X:|x-y_0|<\delta\} \supsetneq \{y \in Y:|y-y_0|<\delta\}$(合理)所以对于对于每个$\varepsilon>0$存在$\delta>0$使当$x\in X$且$|y-y_0|<\delta$有$|f(y)-f(y_0)|\leq \varepsilon$.根据定义9.4.1,$f$在$Y$上的限制$f|_Y :Y\rightarrow \mathbb{R}$也是连续函数.

>




***

* **9.4.7**

设$n\geq 0$是函数,并且对于每个$0\leq i\leq n$设$c_i$是实数.设$P:\mathbb{R}\rightarrow\mathbb{R}$是函数$$P(x)=\sum_{i=0}^{n}c_i x^i,$$

这样的函数周知为单变量多项式.一个典型的例子是$P(x)=6x^4 -3x^2+4.$证明P是连续的.




---

>使用归纳法证明,对于$n=1$时$p(x)=C_0+C_1 x$由命题9.4.9可知此时$p(x)$是连续的.假设对于$n$,$p(x) = \sum_{i=0}^{n}C_i x^i$是连续的,对于$n+1$,$p(x) = \sum_{i=0}^{n+1}$$=\sum_{i=0}^{n} + C_{n+1}x^{n+1}$,由命题9.4.11可知,$C_{n+1}x^{n+1}$是连续的,再由命题9.4.9可知$p(x) = \sum_{i=0}^{n+1}$是连续的.归纳证得p是连续的.

>

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

>定义:设$E$是$\mathbb{R}$的子集合,$f:E\rightarrow \mathbb{R}$是函数并设$x_0$为实数,且$x_0$为$E$的附着点.我们说$f$在$x_0$处沿着$E$收敛到$\infty$写作$\lim_{x\rightarrow x_0:x\in E}f(x) = \infty$当且仅当$f$在$x_0$处沿着$E$不收敛到任何实数$L$.

>

>命题9.3.9当$L=\infty$时,

>叙述:设$X$是$\mathbb{R}$的子集合,$f:X\rightarrow\mathbb{R}$是函数,并设E是X的子集合,$x_0$是$E$的附着点,而$L$是实数.那么下述两命题是逻辑上等价的:

>(a)$f$在$x_0$处沿着$E$收敛到$\infty$.

>(b)对于每个完全由$E$的元素组成,并且收敛到$x_0$的序列$(a_n)_{n=0}^\infty$序列$(f(a_n))_{n=0}^\infty$都收敛到$\infty$.

>

>证明:

>首先证明$(a)\rightarrow(b)$.

>设$(a_n)_{n=0}^\infty$为任意一个完全由$E$的元素组成且收敛到$x_0$的序列并设$L$为任意实数,因为$f$在$x_0$处沿着$E$收敛到$\infty$可知对于每个$\varepsilon>0$,不存在$\delta>0$,使得当$f$限制在集合$\{x\in E:|x-x_0|<\delta\}$上是$\varepsilon-$接近于$L$的.又因为序列$(a_n)_{n=0}^\infty$收敛到$x_0$,所以对于每个$\delta>0$都存在$N>0$当$n>N$时有$|a_n-x_0|\leq \delta$,所以对于每个$\varepsilon>0$,不存在$N>0$当使得当$f$限制在集合$\{a_n|n>N\}$上是$\varepsilon-$接近于$L$的.即对于于每个$\varepsilon>0$,不存在$N>0$当$n>N$时$f(a_n)$是$\varepsilon-$接近于$L$的.所以命题(b)成立.

>

>然后证明$(b)\rightarrow(a)$.

>反证:若$f$在$x_0$处沿着$E$能收敛到$L$.则存在$\varepsilon_0>0$,此时存在$\delta>0$,使得当$f$限制在集合$\{x\in E:|x-x_0|<\delta\}$上是$\varepsilon_0-$接近于$L$的.由命题(b)可知对于$\varepsilon_0>0$,不存在$N>0$当$n>N$时$f(a_n)$是$\varepsilon_0-$接近于$L$的.即不存在$\delta>0$使$a_n\in \{x\in E:|x-x_0|<\delta\}$.两者矛盾.所以原命题成立.

>

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

>构造一、

>$$f(x)=x^2,f:(1,2)\rightarrow\mathbb{R}$$

>构造二、

>$$f(x)=\frac{1}{x+2},f:[0,+\infty)\rightarrow\mathbb{R}$$

>构造三、

>$$f(x) =
\begin{cases}
x,  & \text{if $x \neq -1$ and $x \neq 1$} \\
0.5, & \text{if $n=1$}\\
-0.5, & \text{if $n=0$}
\end{cases}f:[-1,1]\rightarrow\mathbb{R}$$

>构造四、

>$$f(x)=\frac{1}{x-1},f:[-1,1] \rightarrow\mathbb{R}$$

>




***




---

#### 习题9.7

---




***

* **9.7.1**

设$a<b$,并设$f:[a,b]\rightarrow\mathbb{R}$是$[a,b]$上的连续函数.设$M:=\sup_{x\in[a,b]}f(x)$是f的最大值,并设$m:=inf_{x\in[a,b]}f(x)$是最小值.如果$y$是介于$m$和$M$之间的实数$(即m\leq y\leq M)$,那么存在$c\in [a,b]$使得$f(c)=y$.进而有$f([a,b])=[m,M]$.




---

>由题目可知$M$为$f$在$[a,b]$上的最大值,$m$为$f$在$[a,b]$上的最小值.所以存在$d\in[a,b]$使$f(d)=m$且存在$e\in[a,b]$使$f(e)=M$且有$[d,e]\subseteq[a,b]$.由习题可知$f:[a,b]\rightarrow\mathbb{R}$在$[a,b]$上的连续函数,由定理9.7.1中值定理可知,若$y$是介于$m$和$M$之间的实数,那么存在$c\in [d,e]$使得$f(c)=y$,又因为$[a,b]\supseteq [d,e]$所以存在$c\in [a,b]$使得$f(c) = y$.

>




***

* **9.7.2**

设$f:[0,1]\rightarrow[0,1]$是连续函数.证明存在实数$x\in [0,1]$,使$f(x)=x$.$($对于函数$f(x)\rightarrow x$使用中值定理$)$此点$x$叫作$f$的不动点.这个结果是不动点定理的一个基本例子,它在一定类型的分析学问题中起着重要的作用.




---

>设$g(x)=f(x)-x,g:[0,1]\rightarrow \mathbb{R}$,因为$f:[0,1]\rightarrow [0,1]$上为连续函数且$x:[0,1]\rightarrow [0,1]$上为连续函数,根据命题9.4.9可知函数$g$在[0,1]上为连续函数,设$M=\sup_{x\in [0,1]} f(x)$是函数$f$的最大值,$m=\inf_{x\in [0,1]} f(x)$是函数$f$的最小值.由题可知$M=1,m=0$所以存在$e\in [0,1]$使$f(e)=M$且存在$d\in [0,1]$使$f(d)=m$,当$x=d$时$g(d)=f(d)-d=-d$因为$d\geq 0$所以$g(d)\leq 0$.另一方面,当$x=e$时,$g(e)=f(e)-e=1-e$因为$0\leq e\leq 1$所以$1-e \geq 0$即$g(e) \geq 0$.$[d,e] \subseteq [0,1]$由习题9.4.6可知,函数$g$在$[d,e]$上连续,由中值定理可知,因为$0\in [g(d),g(e)]$所以存在$c\in [d,e]$使$g(c) = 0$即存在$c\in [0,1]$使$f(x)=x$.

>

>函数的表达（定义域、值域、函数名以表示笛卡尔积、函数映射方式以清晰表示定义域变量和值域变量:常用形式函数名(定义域变量名)）

>

***




---

#### 习题9.8

---




***

* **9.8.1**

解释为什么把$f$连续的假定换为$f$单调或严格单调时,最大值原理仍然成立.$($对于单调和严格单调两种情形可用统一解释.$)$




---

>若$f$是单调函数,可知$f$在$b$和$a$处达到最值,此时$a\in [a,b],b \in [a,b]$仍都满足最大值原理.

>若$f$是严格单调函数,解释同理.

>




***

* **9.8.2**

举例说明当连续的假定换为单调或严格单调时中值定理不成立.$($对于单调和严格单调两种情况可以使用同一反例.$)$




---

>反例:

>$$f(x)=\begin{cases}
1,  & \text{if $x \geq 0$} \\
-1, & \text{if $x \leq 0$}
\end{cases},f:\mathbb{R}\rightarrow\{1,-1\}$$
>




***

* **9.8.3**

设$a<b$是实数,并设$f:[a,b]\rightarrow\mathbb{R}$是函数.如果$f$既是连续的又是1对1的,那么$f$是严格单调的.




---

>第一种情况:当$f(a)<f(b)$时,反证,若$f$不是严格单调增的,则存在$x_1,x_2\in [a,b],x_1<x_2$且$f(x_1)\geq f(x_2)$,因为$f$在$[a,b]$上为连续的函数,由习题9.4.6可知,在其子集$[a,x_1],[x_1,x_2],[x_2,b]$上也为连续的函数,再考察$f(a)$与$f(x_1)$的大小关系,情况一、若$f(a)\geq f(x_1)$,则有$f(a)\geq f(x_2)$且$f(x_2) \leq f(b)$,即存在$y\in [f(x_2),f(a)]\cap [f(x_2),f(b)]$由定理9.7.1中值定理可知存在$c_1\in [a,x_2]$且$c_2\in [x_2,b]$使$f(c_1)=f(c_2)=y$这与$f$为一对一的函数矛盾.情况二、若$f(a) \leq f(x_1)$,则有$f(a) \leq f(x_1)$且$f(x_1)\geq f(x_2)$,即存在$y_1\in [f(a),f(x_1)]\cap [f(x_2),f(x_1)]$由定理9.7.1中值定理可知存在$c_3\in [a,x_1]$且$c_4 \in [x_1,x_2]$使$f(c_3) = f(c_4) = y_1$这与$f$为一对一的函数矛盾.综合情况一、二可知此时反证的假设不成立,所以证得$f$是严格单调的.

>第二种情况:当$f(a)=f(b)$时,这直接与函数$f$为一对一的矛盾.

>第三种情况:当$f(a)>f(b)$时,同样可以使用反证法,证明与第一种情况同理.

>综合三种情况可证,如果$f$既是连续的又是1对1的,那么$f$是严格单调的.

>




***

* **9.8.4**

设$a<b$是实数,并设$f:[a,b]\rightarrow\mathbb{R}$是函数.如果$f$既是连续的又是严格单调增的,那么$f$是从$[a,b]$到$[f(a),f(b)]$的双射,并且逆映射$f^{-1}:[f(a),f(b)]\rightarrow [a,b]$也是连续的并且严格单调增的.




---

>证明一:$f$是从$[a,b]$到$[f(a),f(b)]$的双射.

>首先证明$f$是单射.设$x_1,x_2\in [a,b],x_1 \neq x_2$不妨设$x_1<x_2$,因为$f$是严格单调增的,所以$f(x_1)<f(x_2)$即$f(x_1)\neq f(x_2)$即证$f:[a,b]\rightarrow\mathbb{R}$是单射函数.

>然后证明$f$是满射的.因为$f$为严格单调递增的函数且定义域为闭区间所以可知最大值为$M=sup_{x\in [a,b]} f(x) = f(b)$且最小值为$m=inf_{x\in [a,b]} f(x) = f(a)$,由推论9.7.4可知$f([a,b])=[m,M]$.

>最后有前两个证明可知$f$是从$[a,b]$到$[f(a),f(b)]$的双射.

>

>证明二:逆映射$f^{-1}:[f(a),f(b)]\rightarrow [a,b]$也是连续的并且严格单调增的.

>设$y_0\in [f(a),f(b)] f^{-1}(y_0)=x_0\in [a,b]$,对于任意给定的$\varepsilon>0$要找出$\delta>0$使当$|y-y_0|<\delta$有$|f^{-1}(y)-f^{-1}(y_0)|=|f^{-1}(y)-x_0|<\varepsilon$成立,$|f^{-1}(y)-x_0|<\varepsilon$即有$x_0-\varepsilon < f^{-1}(y) < x_0+\varepsilon$设$y_1=f(x_0-\varepsilon),y_2=f(x_0+\varepsilon)$,取$\delta = min(|y_0-y_1|,|y_0-y_2|)$时可使$|f^{-1}(y)-f^{-1}(y_0)|<\varepsilon$成立.即证逆映射$f^{-1}:[f(a),f(b)]\rightarrow [a,b]$也是连续的并且严格单调增的.




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

(c)证明对于每个非比例数$x$,$f$在$x$处连续.




---

>证明:(a)证明$f$是严格单调增加的.

>设$x_1\in\mathbb{R},x_2\in\mathbb{R}$,不妨设$x_1<x_2$.由命题5.4.14可知可以找到一个比例数$q$,使$x_1<q<x_2$,$f(x_2)=f(x_1)+\sum_{r\in \mathbb{Q}:x_1\leq r\leq x_2}g(r)$,因为$g(q)>0$所以$\sum_{r\in \mathbb{Q}:x_1\leq r\leq x_2}g(r) > 0$所以$f(x_2)>f(x_1)$,即证$f$是严格单调增加的函数.

>

>证明:(b)证明对于每个比例数$r$,$f$在$r$处间断.

>$f(r)=\sum_{s\in\mathbb{Q}:s<r}g(s)$,对于任意$X>r$$f(x)=\sum_{s\in\mathbb{Q}:s<r}g(s)+\sum_{s\in\mathbb{Q}:r \leq s<x}g(s)$ $\geq f(r)+g(r)$因为$g(r) = 2^{-n}$ 所以有 $f(x) \geq f(r) + 2^{-n}$这样$f(r)$不右连续,也就是间断.

>

>证明:(c)证明对于每个非比例数$x$,$f$在$x$处连续.

>首先证明函数$f_{n}$在x_0处连续,设$x_0\in\mathbb{r}$且$x_0$为非比例数,首先构造函数$f_{n}(x) = \sum_{r\in \mathbb{R}:r<x,g(r)\geq 2^{-n}}g(r)$.$|f_{n}(x)-f_{n}(x_0)|=\sum_{r\in \mathbb{R}:x_0<r<x,g(r)\geq 2^{-n}}g(r) (0\leq j \leq k \leq n ,j=\inf(\{h:x_0<q(h)<x,g(q(h))\geq 2^{-n} \}),k=\sup(\{h:x_0<q(h)<x,g(q(h))\geq 2^{-n}) )$因为存在$\delta$使$\{r:x_0-\delta<r<x_0+\delta,g(r)\geq 2^{-n}\} = \phi$(反证法可证,若不存在会导致$\{r:x_0-\delta<r<x_0+\delta,g(r)\geq 2^{-n}\}$为无限集合,这与其基数$n$有限矛盾.),此时当$x\in [x_0-\delta,x_0+\delta]$时,$|f_{n}(x)-f_{n}(x_0)|=0$小于任何$\varepsilon>0$,即证,$f_{n}$在$x_0$处连续.

>然后证明$|f(x)-f_n (x)|\leq 2^{-n}$.

>$|f(x)-f_{n} (x) = \sum_{r\in\mathbb{Q},r<x,g(r)\leq 2^{-n-1}}$ $\leq 2-(2-2(\frac{1}{2})^{n+1}) = (2)^{-n}$ 

>




***




---

#### 习题9.9

---




***

* **9.9.1**

引理9.9.7

设$(a_n)_{n=1}^\infty$和$(b_n)_{n=1}^\infty$是实数序列(不必是有界的或收敛的).那么$(a_n)_{n=1}^\infty$和$(b_n)_{n=1}^\infty$是等价的,当且仅当$\lim_{n\rightarrow \infty} (a_n-b_n) = 0$.




---

>首先证明:若$(a_n)_{n=1}^\infty$和$(b_n)_{n=1}^\infty$是等价的,则$\lim_{n\rightarrow \infty} (a_n-b_n) = 0.$

>因为$(a_n)_{n=1}^\infty$和$(b_n)_{n=1}^\infty$是等价的,根据定义9.9.5可知有对于任意$\varepsilon \leq 1$存在$N\leq 0$使得当$n>N$时有$|a_n-b_n|<\varepsilon$即有$|(a_n-b_n)-0|<\varepsilon$.根据定义6.1.5可知序列$(a_n-b_n)_{n=1}^\infty$收敛到$0$.

>然后证明:若$\lim_{n\rightarrow \infty} (a_n-b_n) = 0$则$(a_n)_{n=1}^\infty$和$(b_n)_{n=1}^\infty$是等价的.

>因为$\lim_{n\rightarrow \infty} (a_n-b_n) = 0$根据定义6.1.5可知对于任意$\varepsilon>0$存在$N\leq 1$使得当$n>N$时有$|a_n-b_n-0|<\varepsilon$即有$|a_n-b_n|<\varepsilon$根据定义9.9.5可知$(a_n)_{n=1}^\infty$和$(b_n)_{n=1}^\infty$是等价的.

>




***

* **9.9.2**

设$X$是$\mathbb{R}$的子集合,并设$f:X\rightarrow \mathbb{R}$是函数.那么下述两命题逻辑上等价:

(a)$f$在$X$上一致连续.

(b)只要序列$(x_n)_{n=0}^\infty$和序列$(y_n)_{n=0}^\infty$是由$X$的元素组成的等价序列,那么序列$(f(x_n))_{n=0}^\infty$和$(f(y_n))_{n=0}^\infty$也是等价的.




---

>首先证明:$(a)\rightarrow (b)$.

>因为$f$在$X$上一致连续,所以根据定义9.9.2,有对于每个$\varepsilon>0$,都存在$\delta>0$,使得只要$x,x_0\in X$并且$x$与$x_0$是$\delta-$接近的,$f(x)$与$f(x_0)$就是$\varepsilon-$接近的,因为序列$(x_n)_{n=0}^\infty$和序列$(y_n)_{n=0}^\infty$是由$X$的元素组成的等价序列,所以根据定义9.9.5可知对任意$\delta>0$存在$N\leq 0$使当$n>N$时有$|x_n-y_n|<\delta$并且所有$x_n,y_n\in X$.所以有对于任意$\varepsilon>0$存在$N\leq 0$使当$n>N$时有$|f(x_n)-f(y_n)|<\varepsilon$,根据定义9.9.5可知序列$(f(x_n))_{n=0}^\infty$和$(f(y_n))_{n=0}^\infty$也是等价的.

>

>然后证明:$(b)\rightarrow (a)$.

>由$(b)$可知$(x_n)_{n=0}^\infty$和$(y_n)_{n=0}^\infty$是由$X$的元素组成的等价序列,那么序列$(f(x_n))_{n=0}^\infty$和$(f(y_n))_{n=0}^\infty$也是等价的可知,对于任意$\varepsilon>0$,都有对每个$\delta>0$存在$N>0$使当$n>N$时有$|x_n-y_n|<\delta$则有$|f(x_n)-f(y_n)|<\varepsilon$,又因为$x_n,y_n$为任意在$X$上且受$|x_n-y_n|<\delta$约束的元素,所以有对于任意$\varepsilon>0$,都有对每个$\delta>0$对任意$x,x_0\in X$满足$|x_n-y_n|<\delta$则有$|f(x)-f(x_0)|<\varepsilon$,根据定义9.9.2可知$f$在$X$上一致连续.

>

>

>静态映射改变法则

>




***

* **9.9.3**

设$X$是$\mathbb{R}$的子集合,并设$f:X\rightarrow \mathbb{R}$是一致连续函数.如果$(x_n)_{n=0}^\infty$是由$X$中的元素组成的Cauchy序列,那么$(f(a_n))_{n=0}^\infty$也是Cauchy序列.




---

>因为$f$为一致连续函数,所以对于任何$\varepsilon>0$都有存在$\delta>0$使当$x,x_0\in X$且$|a_n-a_m|<\delta$,有$|f(x)-f(x_0)<\varepsilon$,因为$(x_n)_{n=0}^\infty$是由$X$中的元素组成的Cauchy序列,即对于任意$\delta>0$都存在$N\leq 0$是当$n,m>N$时有$|a_n-a_m|<\delta$,所以有对任何$\varepsilon>0$都有$\delta>0$存在$N\leq 0$是当$n,m>N$时有$|a_n-a_m|<\delta$则有$|f(a_n)-f(a_m)<\varepsilon$,根据定义5.1.8可知$(f(a_n))_{n=0}^\infty$也是Cauchy序列.

>




***

* **9.9.4**

设$X$是$\mathbb{R}$的子集合,$f:X\rightarrow \mathbb{R}$是一致连续函数,并设$x_0$是$X$的附着点.那么极限

$$\lim_{x\rightarrow x_0:x\in X} f(x)$$

存在(当然它是实数).




---

>因为$x_0$是$X$的附着点,根据引理9.1.14可知,存在一个全由$X$的元素组成的序列$(a_n)_{n=0}^\infty$,它收敛到$x_0$,由命题6.1.12可知,$(a_n)_{n=0}^\infty$是cauchy序列,再根据命题9.9.12可知,序列$(f(a_n))_{n=0}^\infty$也为cauchy序列.由定理6.4.18可知

$$\lim_{x\rightarrow x_0:x\in X} f(x)$$

存在.

>




***

* **9.9.5**

设$X$是$\mathbb{R}$的子集合,$f:X\rightarrow \mathbb{R}$是一致连续函数.如果$E$是$X$的有界子集合,那么$f(E)$也是有界的.




---

>假设$f(E)$不是有界的,那么对于每个实数$M$,都存在一个元素$x\in [a,b]$使得$|f(x)|\geq M$.所以对于每个自然数$n$,集合$\{x\in X:|f(x)|\geq n\}$不是空集.于是可以从$X$中选取一个序列$(x_n)_{n=1}^\infty$使对于一切$n$,$|f(x_n)|\geq n$.这个序列位于$X$中,因为$E$为有界子集,所以序列$(x_n)_{n=1}^\infty$为有界序列,再根据定理6.6.8可知其存在一个子序列$(x_{n_j})_{j=0}^\infty$收敛到某极限$L\in X$,其中$n_0<n_1<n_2<...$是自然数的增序列.即有$n_j\geq j$对一切$j\in \mathbb{N}$成立.由于$f$在$X$上一致连续,根据推论9.9.14可知$\lim_{j\rightarrow \infty} f(x_{n_j}) = f(L)$,于是序列$(f(x_{n_j}))_{j=0}^\infty$是收敛的,从而使有界的.另一方面,我由此序列的构造知$|f(x_{n_j})|\geq n_j \geq j$对于一切$j$成立,从而$(f(x_{n_j}))_{j=0}^\infty$不是有界的,这是一个矛盾.

>




***

* **9.9.6**

设$X,Y,Z$是$\mathbb{R}$的子集合,设$f:X\rightarrow Y$是$X$上的一致连续函数,并设$g:Y\rightarrow Z$是$Y$上的一致连续函数.证明$g\circ f:X\rightarrow Z$是$X$上的一致连续函数.




---

>首先因为$g:Y\rightarrow Z$是$Y$上的一致连续函数,根据定义9.9.2可知,对任意$\varepsilon>0$都存在$\delta>0$使当只要$y,y_0\in Y$且$|y-y_0|<\delta$则$|g(y)-g(y_0)|<\varepsilon$又因为$f:X\rightarrow Y$是$X$上的一致连续函数.所以有对任意$\delta>0$都存在$\delta_0>0$使当只要$x,x_0 \in X$且$|x-x_0|<\delta_0$则$|f(x)-f(x_0)|<\delta$令$y=f(x),y_0=f(x_0)$可知对任意$\varepsilon>0$都存在$\delta_0>0$使当$x,x_0\in X$且$|x-x_0|<\delta$有$|g(f(x))-g(f(x_0))|<\varepsilon$根据定义9.9.2,即证$g\circ f:X\rightarrow Z$是$X$上的一致连续函数.

>




***




---

#### 习题9.10

---




***

* **9.10.1**

设$(a_n)_{n=0}^\infty$是实数序列,那么$a_n$也可以看作是从$\mathbb{N}$到$\mathbb{R}$的函数,它把每个自然数$n$映射到一个实数$a_n$.证明

$$\lim_{n\rightarrow \infty:n\in \mathbb{N}} a_n = \lim_{n\rightarrow \infty} a_n$$

其中左边的极限是用定义9.10.3确定的,而右边的极限是用定义6.1.8确定的.更准确地说,证明:如果上述两极限中有一个存在,那么另一个也存在并且它们有相同的值.于是这里的两个极限是一致的.




---

>首先证明:若$\lim_{n\rightarrow \infty} a_n$存在且等于$L$则$\lim_{n\rightarrow \infty:n\in \mathbb{N}} a_n$存在且等于$L$.

>因为$\lim_{n\rightarrow \infty} a_n$存在,根据定义6.1.8可知存在实数$L$,对于每个实数$\varepsilon>0$,存在$N\geq m$,使得$(a_n)_{n=N}^\infty$是$\varepsilon-$接近于$L$的,因为$\{n:n\in \mathbb{N},n\geq N\} = \mathbb{N}\cap (N,+\infty)$,所以对每个$\varepsilon>0$,都存在$N$使得$f$在$\mathbb{N}\cap(N,+\infty)$上是$\varepsilon-$接近于的$L$.

>然后证明:若$\lim_{n\rightarrow \infty:n\in \mathbb{N}} a_n$存在且等于$L$则$\lim_{n\rightarrow \infty} a_n$存在且等于$L$.

>证明与上同理.




***

