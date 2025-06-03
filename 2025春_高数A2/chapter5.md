---
 title: 高等数学讲义(下)
author: 胡煜成
description: 首都师范大学2025秋季学期高等数学A
"og:description": 浏览器版和手机版
"og:image": https://vlook-doc.pages.dev/pic/vlook-og.png
keywords:
- 高等数学,微积分,讲义
vlook-chp-autonum: h1{{第 ### 节 }},h3{{### }}
vlook-query: vdl=on
vlook-query: ws=off
---

[回到主页面](index.html)


# 无穷级数
> [!tip]
> 
> 本章的内容主要包括**常数项级数的收敛性**和**函数的级数展开**. 对**常数项级数**的研究可以追溯到古人对极限过程的早期理解. 而**函数项级数**则是分析学中一项极其重要的工具, 函数项级数蕴含了深层次的数学思想, 即用简单的无穷多项的和来表示一个复杂的对象.

## 常数项级数的概念和性质

> [!note]
> 
> ==常数项级数的直观例子==
> 
> ---
> > ==例1：一尺之杠, 日取其半==
> > $$
> > \begin{aligned}
> > & S_1=\frac{1}{2} \\
> > & S_2=\frac{1}{2}+\frac{1}{4}=\frac{3}{4} \\
> > & S_3=\frac{1}{2}+\frac{1}{4}+\frac{1}{8}=\frac{7}{8} \\
> > & \cdots \\
> > & S_n=\frac{1}{2}+\frac{1}{4}+\cdots+\frac{1}{2^n}=\frac{\frac{1}{2}\left(1-\left(\frac{1}{2}\right)^n\right)}{1-\frac{1}{2}}=1-\frac{1}{2^2} \\
> > & \lim _{n \rightarrow \infty} S_n=1
> > \end{aligned}
> > $$
>
> > ==例2：割圆法与圆面积==
> 


> [!important]
> 
> ==级数的定义==
>
> 无穷多个数的和称为**无穷级数**, 简称**级数**.
> 
> 给定数列 $a_n, n = 1, 2, \cdots, \infty$, $S_n= \displaystyle \sum_{i}^{\ n} a_n$ 称为数列 $a_n$ 的**部分和**, 如果 $\displaystyle \lim _{n \rightarrow \infty} S_n=S$ 有极限，称级数**收敛**, 否则称级数**发散**.

>[!tip]
>
>P253 例1. 等比数列
>$$
>S_n=\sum_{i=1}^{\ n} a q^{i-1}, a \neq 0
>$$
>
>$q \neq 1 \quad S_n=\frac{a}{1-q}-\frac{a q^n}{1-q}$
>
>$|q|<1$ ,收敛.
>$q=1  $,发散 .
>$|q|>1$ , 发散.
$q=-1 $ 发散.

>p253．例2：$\displaystyle S_n=\sum_{i=1}^{\ n} i$, 发散

>P253．例3：
>$$
>\quad S_n=\frac{1}{1 \cdot 2}+\frac{1}{2 \cdot 3}+\cdots+\frac{1}{n(n+1)}
>$$
>$$
\begin{aligned}
& =\frac{1}{1}-\frac{1}{2}+\frac{1}{2}-\frac{1}{3}+\cdots+\frac{1}{n}-\frac{1}{n+1} \\
& =1-\frac{1}{n+1} \rightarrow 1 \quad \text { 收敛. }
\end{aligned}
>$$

> [!important] 
> 
>
>**性质1**：$\quad \sum u_n=s . \quad \sum k u_n=k s.$
>
>**性质2**：$已知\sum u_n=s, \sum U_n=δ,有
\sum\left(u_n+v_n\right)=s+δ.
$
>
>**性质3**：改变级数有限项不影响收敛性.
>
>**性质5** :
>$$
>级数收敛 \displaystyle \Longrightarrow \lim _{n \rightarrow \infty} a_n \Rightarrow 0.
>$$
>
> $$
> 例\quad \frac{1}{2}-\frac{2}{3}+\frac{3}{4}-\cdots+(-1)^{n-1} \frac{n}{n+1}
> $$
>
>$$
>\lim _{n \rightarrow \infty} a_n=0 \nRightarrow \text { 级数收敛. }
>$$
>
>$$
>例\ \ 1+\frac{1}{2}+\frac{1}{3}+\cdots+\frac{1}{n}
>$$

## 常数项级数的审敛法

>[!tip]
>
> 直接计算部分和很多时候并不可行, 如果我们只关心级数收敛与否, 可以使用一些判别法来判断级数的收敛性, 这些判别法也称为**审敛法**.

### 正项级数

> [!important]
> 
> ==定理1==
> 
> 正项级数 $\displaystyle \sum_{n=1}^{\infty} u_n$ 收敛的充要条件是 $S_n$ 有界。
>
> 注: 本质上这个定理就是我们上册学过的**单调有界有极限**.

> [!important]
> 
> ==定理2==
> 
> $\sum u_n$ 和 $\sum v_n$ 都是正项级数，$u_n \leqslant v_n$, 则 
>
>$$\sum  v_n收敛 \Rightarrow \sum  u_n收敛$$
>$$\sum u_n \text { 发散 } \Rightarrow \sum v_n \text { 发散. }$$
>
> 注: 上述结论与数列的前 $N$ 项无关.

> [!note]
> 
> $P 260$ 例2：$\sum \frac{1}{\sqrt{n(n+1)}}$
> $\frac{1}{n+1}<\frac{1}{\sqrt{n(n+1)}}<\frac{1}{\sqrt{n n}}$

> [!important]
> 
> ==定理3== $
> \lim _{n \rightarrow \infty} \frac{u_n}{v_n}=l$ ，$l>0$ ，则二者同收敛.
>

> [!note]
>P261例3．$\sum_{n=1}^{\infty} \sin \frac{1}{n}$
>
>解：
>$$
\lim \frac{\sin \frac{1}{n}}{\frac{1}{n}}=1 . \quad \sum \sin \frac{1}{n} 发散
>$$

>[!important]
>
> ==定理4 (非常重要)==
> 已知$\quad \lim _{n \rightarrow 0} \frac{u_{n+1}}{u_n}=ρ$
>$$
>\begin{array}
>ρ<1 . & \text { 收敛. } \\
>ρ>1 . & \text { 发散. } \\
>ρ=1 . & \text { 不确定.}
>\end{array}
>$$

>[!tip]
例4．$P263 . \quad 1+\frac{1}{1}+\frac{1}{1· 2}+\frac{1}{1·2·3}+\cdots+\frac{1}{(n-1)!}+\dots$
>$$
\lim _{n \rightarrow \infty} \frac{u_{n+1}}{u_n}=\lim _{n \rightarrow \infty} \frac{(n-1)!}{n!}=\lim _{n \rightarrow \infty} \frac{1}{n}=0 \quad \text {, 收敛. }
>$$
>
>例5．$\quad \frac{1}{10}+\frac{1·2}{10^2}+\frac{1·2·3}{10^3}+\cdots+\frac{n!}{10^n}$
>$$
\lim _{n \rightarrow \infty} \frac{u_{n+1}}{u_n}=\lim _{n \rightarrow \infty} \frac{(n+1)}{10}=\infty \text {, 发散. }
>$$


### 交错级数

>[!important]
> 
> ==交错级数的定义==
> [补充]

>[!important]
>
> ==定理7（莱布尼茨定理）==
>对$\sum_{n=1}^{\infty}(-1)^{n-1} u_n$,
>若 $ u_n \geqslant u_{n+1} . \quad \lim _{n \rightarrow \infty} u_n=0$,则级数收敛.

> [!note]
>$$
\begin{aligned}
& 1-\frac{1}{2}+\frac{1}{3}-\frac{1}{4}+\cdots+(-1)^{n-1} \frac{1}{n}+\cdots \\
& u_n=\frac{1}{n}, \quad u_n>u_{n+1} \quad \lim _{n+1} u_n=0
\end{aligned}
>$$


### 绝收数与条件收敛

> [!important]
> ==绝对收敛== 
> 
> $\displaystyle \sum_{n=1}^{\infty}\left|u_n\right|$ 收敛
>
> ==条件收敛==
> 
> $\displaystyle \sum_{n=1}^{\infty}\left|u_n\right|$ 发散但 $\displaystyle \sum_{n=1}^{\infty} u_n$ 收敛
>
> 注: 绝对收敛 $\Rightarrow$ 条件收敛.

>[!note]
>
>p268．例9.$\quad \sum \frac{\sin n \alpha}{n^2}$
>解：
>$$
> 因\sum\left|\frac{\sin \alpha}{n^2}\right| \leqslant \sum \frac{1}{n^2}, 故收敛
>$$


## 幂级数

> [!tip]
> 由常数数列构成的级数称为**常数项级数**, 由无穷多个函数的和构成的无穷级数称为**函数项级数**. **幂级数**是函数项级数中最简单也最直观的例子.

>### 幂级数
>
>$$
>\displaystyle \sum_{n=1}^{\infty} a_n x^n = a_0 + a_1x + a_2x^2 + \cdots + a_nx^n + \cdots
>$$
>其中常数a_0,a_1,a_2,…,a_n,…叫做幂级数的系数.

>**例1：**
>
>$$
1 + x + x^2 + \cdots + x^n + \cdots = \frac{1 - x^n}{1 - x}
>$$
>
>* $|x| < 1$：收敛
>* $|x| > 1$：发散
>* $x = 1$：发散
>* $x = -1$：发散

>**例2：**
>
>$$
1 + \frac{x}{1!} + \frac{x^2}{2!} + \frac{x^3}{3!} + \cdots + \frac{x^n}{n!} + \cdots = e^x
>$$
>
>* $-\infty < x < \infty$：收敛

---

>**定理1**（阿贝尔(Abel)定理）
>如果级数$\displaystyle \sum_{n=1}^{\infty} a_n x^n$ 当$x=R(R\neq 0)$时收敛，那么
>* 适合不等式
 $|x| < R $ 的一切 x 使得幂级数绝对收敛。
 >
>反之，如果级数$\displaystyle \sum_{n=1}^{\infty} a_n x^n$ 当 $x=R(R\neq 0)$时发散，那么 
>* 适合不等式 $|x| > R$的一切 x 使得幂级数发散。
>
>注意：$x = R, -R$：待定
>

>收敛半径：正数$R$
>
>收敛区域：开区间$(-R, R)$，$[-R, R]$, $(-R, R]$, $(-R, R)$ 

>**定理2**：
>
>如果
>$$
\lim_{n \to \infty} \left| \frac{a_{n+1}}{a_n} \right| = \ell,
>$$
>其中a_n,a_{n+1}为幂级数相邻两项的系数，$\ell$为常数，则幂级数的收敛半径为
>$$
R = 
\begin{cases}
\frac{1}{\ell}, & \ell \ne 0 \\
\infty, & \ell = 0 \\
0, & \ell = +\infty.
\end{cases}
>$$
>
>计算：
>$$
\left| \frac{a_{n+1}x^{n+1}}{a_nx^n} \right| = |x|\ell < 1
\Rightarrow |x| < \frac{1}{\ell}
>$$

---
>[!tip]
>
>例1（P276）：
>
>$$
x - \frac{x^2}{2} + \frac{x^3}{3} - \cdots + (-1)^n \frac{x^n}{n} + \cdots
>$$
>
>$$
\ell = \lim_{n \to \infty} \left| \frac{a_{n+1}}{a_n} \right| = \lim_{n \to \infty} \frac{\frac{1}{n+1}}{\frac{1}{n}} = 1
\Rightarrow R = 1
>$$
>
>* $x = -1 \Rightarrow -1 + \frac{1}{2} - \cdots$：发散
>* $x = 1 \Rightarrow 1 - \frac{1}{2} + \frac{1}{3} - \cdots$：收敛
>
>收敛区间：$(-1, 1]$


>**例2**
>
>$$
1 + x + \frac{x}{2!}  + \cdots + \frac{1}{n!}x^n + \cdots
>$$
>
>$$
\ell = \lim_{n \to \infty} \frac{1}{n+1} = 0
\Rightarrow R = \infty \Rightarrow (-\infty, \infty)
>$$

>**例3**
>求幂级数 $\displaystyle\sum_{n=1}^\infty {n!}{x^n}$ 的收敛半径（规定 $0! = 1$）
>
>**解**：
>$$
\rho = \lim_{n\to\infty} \left| \frac{a_{n+1}}{a_n} \right| = \lim_{n\to\infty} \frac{(n+1)!}{n!} = \lim_{n\to\infty} \frac{n+1}{1} =+\infty 
>$$
>故收敛半径 $R = 0$，级数在 $x=0$ 收敛。

>**例5**
>求幂级数 $\displaystyle\sum_{n=1}^\infty \frac{(x-1)^n}{2^n \cdot n}$ 的收敛域.
>
>**解**：
> 令 $t = x - 1$，级数变为 $\displaystyle\sum_{n=1}^\infty \frac{t^n}{2^n n}$
>
> 因为
   >$$
   \rho = \lim_{n\to\infty} \left| \frac{a_{n+1}}{a_n} \right| = \frac{2^n n }{2^{n+1}(n+1)} = \frac{1}{2}
   >$$
   >故收敛半径 $R = 2$.
> 收敛区间为$ | t | <2$，即$ -1 < x < 3 $.
   >- 当  $x = -1$,级数变为 $\displaystyle\sum_{n=1}^\infty \frac{(-1)^n}{n}$（收敛）
   >- 当  $x = 3$）,级数变为 $\displaystyle\sum_{n=1}^\infty\frac{1}{n}$（发散）
>因此原级数的收敛域是$[-1, 3)$


## 幂级数展开
>常用展开式：
>1. 指数函数：
   >$$ e^x = 1 + x + \frac{x^2}{2!} + \cdots+\frac{x^n}{n!}+\cdots \quad (-\infty < x < \infty) $$
>2. 正弦函数：
   >$$ \sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \cdots+(-1)^n \frac{x^{2n+1}}{(2n+1)!}+\cdots \quad (-\infty < x < \infty) $$
>3. 几何级数：
   >$$ \frac{1}{1+x} = \sum_{n=0}^\infty (-1)^n x^n \quad (-1 < x < 1) $$
>4. 对数函数：
   >$$ \ln(1+x) = \sum_{n=1}^\infty \frac{(-1)^{n-1}}{n} x^n \quad (-1 < x \leq 1) $$
>5. 余弦函数：
>   >$$ \cos x = \sum_{n=1}^\infty \frac{(-1)^{n}}{2n!} x^(2n) \quad (-\infty < x < \infty) $$

>## 幂级数展开例题

>**例3**
将函数 $f(x) = (1 - x) \ln(1 + x)$ 展开成 $x$ 的幂级数。
>
>**解**：
>已知 $\ln(1+x)$ 的幂级数展开：
>$$
\ln(1+x) = \sum_{n=1}^\infty \frac{(-1)^{n-1}}{n} x^n \quad (-1 < x \leq 1)
>$$
>
>因此：
>$$
\begin{aligned}
f(x) &= (1-x) \sum_{n=1}^\infty \frac{(-1)^{n-1}}{n} x^n \\
&= \sum_{n=1}^\infty \frac{(-1)^{n-1}}{n} x^n - \sum_{n=1}^\infty \frac{(-1)^{n-1}}{n} x^{n+1} \\
&= \sum_{n=1}^\infty \frac{(-1)^{n-1}}{n} x^n - \sum_{n=2}^\infty \frac{(-1)^{n}}{n-1} x^n \\
&= x + \sum_{n=2}^\infty  \frac{(-1)^{n-1}(2n-1)}{n(n-1)}   x^n
\end{aligned} \quad 
>$$
>**例4**  将函数 $\sin x$ 展开成 $(x - \frac{\pi}{4})$ 的幂级数。
>
>**解**：
>$$
\sin x = \sin\left( \frac{\pi}{4} + \left(x - \frac{\pi}{4}\right) \right) 
= \sin\frac{\pi}{4} \cos\left(x - \frac{\pi}{4}\right) + \cos\frac{\pi}{4} \sin\left(x - \frac{\pi}{4}\right)
>$$

>**例5**
>将函数 $f(x) = \frac{1}{x^2 + 4x + 3}$ 展开成 $(x-1)$ 的幂级数。
>
>**解**：
>$$
f(x) = \frac{1}{(x+1)(x+3)} = \frac{1}{2(1+x)} - \frac{1}{2(3+x)}
>$$
>
>变形为 $(x-1)$ 形式：
>$$
\frac{1}{2(1+x)} = \frac{1}{4\left(1 + \frac{x-1}{2}\right)}, \quad \frac{1}{2(3+x)} = \frac{1}{8\left(1 + \frac{x-1}{4}\right)}
>$$
>
> 利用几何级数展开：
>$$
\begin{aligned}
\frac{1}{4\left(1 + \frac{x-1}{2}\right)} &= \frac{1}{4} \sum_{n=0}^\infty \frac{(-1)^n}{2^n} (x-1)^n \quad (-1 < x < 3) \\
\frac{1}{8\left(1 + \frac{x-1}{4}\right)} &= \frac{1}{8} \sum_{n=0}^\infty \frac{(-1)^n}{4^n} (x-1)^n \quad (-3 < x < 5)
\end{aligned}
>$$
>
>所以
>$$
f(x) = \sum_{n=0}^\infty (-1)^n \left( \frac{1}{2^{n+2}} - \frac{1}{2^{2n+3}} \right) (x-1)^n \quad (-1 < x < 3)
>$$

## 傅里叶级数（Fourier Series）

不考

[回到主页面](index.html)