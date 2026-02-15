#  <center> Cal_hw_1 </center> 

## **必做题：**

### 1.写出命题 $p \Leftrightarrow q$ 的真值表，其中 $p, q$ 为任意命题.

**解:** 

| $p$ | $q$ | $p \Rightarrow q$ | $p \Leftarrow q$ | $p \Leftrightarrow q$ |
|:---:|:---:|:-----------------:|:----------------:|:---------------------:|
|  0  |  0  |         1         |         1        |           1           |
|  1  |  0  |         0         |         1        |           0           |
|  0  |  1  |         1         |         0        |           0           |
|  1  |  1  |         1         |         1        |           1           |

### 2.利用真值表，证明德摩根律

$\neg(p \vee q) \Leftrightarrow \neg p \wedge \neg q$
$\neg(p \wedge q) \Leftrightarrow \neg p \vee \neg q$

**解:** 

| $p$ | $q$ | $\neg(p \vee q)$ | $\neg p \wedge \neg q$ |
|:---:|:---:|:----------------:|:----------------------:|
|  0  |  0  |        1         |           1            |
|  1  |  0  |        0         |           0            |
|  0  |  1  |        0         |           0            |
|  1  |  1  |        0         |           0            |

| $p$ | $q$ | $\neg(p \wedge q)$ | $\neg p \vee \neg q$ |
|:---:|:---:|:------------------:|:--------------------:|
|  0  |  0  |         1          |          1           |
|  1  |  0  |         1          |          1           |
|  0  |  1  |         1          |          1           |
|  1  |  1  |         0          |          0           |

### 3. 用逻辑符号（$\forall$, $\exists$等）严格写出下面命题，并写出其否定形式.

**解:**  (a) $p : \forall a \in \mathbf{X}, a \geq m$

$\neg p : \exists a \in \mathbf{X}, a < m$

(b) $p : \forall x_1,x_2 \in (a,b) (x_1 < x_2), f(x_1) < f(x_2)$

$\neg p : \exists x_1,x_2 \in (a,b) (x_1 < x_2), f(x_1) \geq f(x_2)$

(c) $p : [\forall x_1,x_2 \in (a,b) (x_1 < x_2), f(x_1) < f(x_2)] \vee [\forall x_1,x_2 \in (a,b) (x_1 < x_2), f(x_1) > f(x_2)]$

$\neg p : [\exists x_1,x_2 \in (a,b) (x_1 < x_2), f(x_1) \geq f(x_2)] \wedge [\exists x_1,x_2 \in (a,b) (x_1 < x_2), f(x_1) \leq f(x_2)]$

(d) 
① $p : \forall X \in \mathbb{R}^+, \exists n \in \mathbb{N}^*, \text{s.t } a_n > X$

$\neg p : \exists X \in \mathbb{R}^+, \forall n \in \mathbb{N}^*, \text{s.t } a_n \leq X$

② $p : \forall X \in \mathbb{R}^-, \exists n \in \mathbb{N}^*, \text{s.t } a_n < X$

$\neg p : \exists X \in \mathbb{R}^-, \forall n \in \mathbb{N}^*, \text{s.t } a_n \geq X$



### 4. 利用数学归纳法证明 $(1+x)^n > 1+nx$，其中 $x > -1$, $x \neq 0$, $n \geq 2$, $n \in \mathbb{N}$.

**解:**  当 $n = 2$ 时，有  $$(1 + x)^2 = x^2 + 2x + 1 > 2x + 1$$  
设命题对 $n = k$ ($k \geq 2$) 成立，  
则当 $n = k + 1$ 时，根据归纳假设，有  

$$ (1 + x)^k > 1 + kx \\ $$ 

$$ (1 + x)^{k+1} > (1 + kx)(1 + x) = kx^2 + 1 + (k + 1)x > 1 + (k + 1)x$$

即命题对 $n = k + 1$ 亦成立，从而由数学归纳法原理知命题对所有 $n \geq 2$ 成立。



### 5.利用欧拉公式证明三角函数的加法公式.

**解:**  $e^{ix} = \cos x + i \sin x$

$e^{iy} = \cos y + i \sin y$

$e^{i(x+y)} = \cos x \cos y + i \cos x \sin y + i \sin x \cos y - \sin x \sin y$

$$= (\cos x \cos y - \sin x \sin y) + i \left( \cos x \sin y + \sin x \cos y \right)$$

所以  $$ e^{i(x+y)} = \cos (x+y) + i \sin (x+y)$$

$$\therefore \cos (x+y) = \cos x \cos y - \sin x \sin y$$

$$\sin (x+y) = \sin x \cos y + \cos x \sin y$$



### 6.验证 $\cosh^2 x - \sinh^2 x = 1$ 和 $\cosh (x \pm y) = \cosh x \cosh y \pm \sinh x \sinh y$.

**解:**  (1) $\sinh x = \frac{e^x - e^{-x}}{2}$  

$\cosh x = \frac{e^x + e^{-x}}{2}$  
$\cosh^2 x - \sinh^2 x = \frac{e^{2x} + e^{-2x}}{4} - \frac{e^{2x} - 2 + e^{-2x}}{4} = 1$



(2) 右边 $= \cosh x \cosh y \pm \sinh x \sinh y$  
$= \frac{e^x + e^{-x}}{2} \times \frac{e^y + e^{-y}}{2} \pm \frac{e^x - e^{-x}}{2} \times \frac{e^y - e^{-y}}{2}$  
$= \frac{e^{x+y} + e^{x-y} + e^{-x+y} + e^{-x-y}}{4} \pm \frac{e^{x+y} - e^{x-y} - e^{-x+y} + e^{-x-y}}{4}$  
$= \frac{e^{x+y} + e^{-x \pm y}}{2} = \cosh(x \pm y) =$ 左边



### 7.写出尖点曲线 $y^2 = x^3$ 的一个参数方程描述.

**解:**  $\begin{cases}
x = t^2 \\
y = t^3
\end{cases}$



### 8.将下列隐函数方程曲线转化为参数方程曲线，并指出参数的变化范围.

**解:**  a) 

$4(x^2 - x + \frac{1}{4}) + (y + 1)^2 = 2$  
$$2(x - \frac{1}{2})^2 + \frac{1}{2}(y + 1)^2 = 1$$  

所以 参数方程  
$$\begin{cases} 
x = \frac{\sqrt{2}}{2} \cos \theta + \frac{1}{2} \\ 
y = \sqrt{2} \sin \theta - 1 
\end{cases}$$  
$$\theta \in [0, 2\pi]$$

b)  
$$\begin{cases} 
x = \frac{1 - e^t - t^3}{2} \\ 
y = t 
\end{cases}$$
$$t \in \mathbb{R}$$



### 9.将下列曲线方程转化为极坐标方程，并指出 θ 的变化范围.

a) $$r^2 = \frac{1}{\cos 2\theta}$$

$$\theta \in (-\frac{\pi}{4}, \frac{\pi}{4}) \cup (\frac{3}{4} \pi, \frac{5}{4} \pi)$$

b) $$r = \cos 2\theta$$

$$\theta \in [-\frac{\pi}{4}, \frac{\pi}{4}] \cup [\frac{3}{4} \pi, \frac{5}{4} \pi]$$

### 10.绘制下列极坐标方程表示的曲线的图形.

**解:**  a) $r = a\theta$ $(a > 0)$

<img src="C:\Users\ss\Downloads\desmos-graph.png" alt="desmos-graph" style="zoom:80%;" />

b) $r = \tan \theta \sec \theta$

<img src="C:\Users\ss\Downloads\desmos-graph (1).png" alt="desmos-graph (1)" style="zoom:40%;" />

c) $r = a \cos 4\theta$

<img src="C:\Users\ss\Downloads\desmos-graph (2).png" alt="desmos-graph (2)" style="zoom:40%;" />





## 选做题

### 1.迪利克雷（Dirichlet）函数定义为：$$D(x) := \begin{cases}1 & x \in \mathbb{Q} \\0 & x \notin \mathbb{Q}\end{cases}$$迪利克雷函数是否为周期函数？如果是，其最小正周期是否存在？

**解:** ①$D$ 是周期函数，任意有理数 $T$ 都是其周期

若 $X \in \mathbb{Q}$ ,  $X+T \in \mathbb{Q}$ ,  $$D(X) = D(X+T) = 1$$

若 $X \notin \mathbb{Q}$，$X+T \notin \mathbb{Q}$ , $$D(X) = D(X+T) = 0$$

②不存在最小正周期

$T$ 可以无限接近0，只要$T \in Q$ 且 $T > 0$



### 2.不通过求导，计算三次曲线 $y = x^3 + 2x + 3$ 在 $x = 1$ 处（即过点 $(1, 6)$）的切线方程。

**解:** 设切线$y - 6 = k(x - 1)$

令 $$y = k(x - 1) + 6 = x^3 + 2x + 3$$

$$k(x - 1)  = x^3 + 2x - 3$$

$$(x - 1)(x^2 + x + 3 - k) = 0$$

因为直线在 $(1, 6)$ 处与曲线相切

所以 $x = 1$为方程的二重根，

所以 当 $x = 1$ 时，$x^2 + x + 3 - k = 0$

所以 $ k = 5$

所以  切线方程：$y = 5x + 1$



### 3.用归纳法证明：第 $n$ 个素数 $p_n < 2^{2^n}$。

**解:** 先证：令 $Q_k = \prod_{i=1}^{k} p_i + 1$

若 $Q_k$ 为素数，$Q_k > P_k$，则 $Q_k \geq P_{k+1}$

若 $Q_k$ 为合数，设 $Q_k$ 的一个素因子为 $P$，则 $P \geq P_{k+1}$，$Q_k > P_{k+1}$

若 $P$ 为 $P_i$... $P_k$ 中的一个

所以  $Q_k \mid P $ , $\prod_{i=1}^k P_i \mid P$

所以  $Q_k - \prod_{i=1}^k P_i = 1$  , $1 \mid P $ , 不成立

所以 $P \geq P_{k+1}$ ,  $Q_k > P_{k+1}$

综上，$Q_k \geq P_{k+1}$



下证原命题：当 $n = 1$ 时

有 $p_1 = 2 < 2^2 = 4$

设命题对 $n = k$ ($k \geq 1$) 成立

$$p_k < 2^{2^k}$$

$$\prod_{i=1}^{k} p_i < \prod_{i=1}^{k} 2^{2^i} = 2^{\sum_{i=1}^{k} 2^i} = 2^{2^{k+1}-2} $$

$$P_{k+1} \leq Q_k = \prod_{i=1}^{k} p_i + 1 < 2^{2^k-2} + 1 < 2^{2^{k+1}}$$

$$P_{k+1} < 2^{2^{k+1}}$$

即命题对 $n = k + 1$ 亦成立，从而由数学归纳法原理知命题对所有 $n \geq 1$ 成立



### 4. 对映射 $T$ 及其逆映射 $T^{-1}$，证明有 $T \circ T^{-1} = I|_{R(T)}$; $T^{-1} \circ T = I|_{D(T)}$，其中 $I$ 代表恒等映射，即满足 $I(x) = x, \forall x$ 的映射。
**解:** 设 $T : D(T) \rightarrow R(T)$  
$T^{-1} : R(T) \rightarrow D(T)$

① $T \circ T^{-1}$
$$(T \circ T^{-1})(y) = T[T^{-1}(y)]$$
$$= T(x) = y = I|_{R(T)}(y)$$

所以 $T \circ T^{-1} = I|_{R(T)}$

② $T^{-1} \circ T$
$$(T^{-1} \circ T)(x) = T^{-1}[T(x)]$$
$$= T^{-1}(y) = x = I|_{D(T)}(x)$$

所以 $T^{-1} \circ T = I|_{D(T)}$

### 5. 写出命题"线性映射 $T : \mathbb{R} \rightarrow \mathbb{R}$ 是单射当且仅当：若 $T(x) = 0$，则 $x = 0$" 的逆否命题，并证明该命题。

**解:** ①逆否命题：线性映射 $T : \mathbb{R} \rightarrow \mathbb{R}$ 不是单射当且仅当 $\exists$ $x \neq 0$ 使得 $T(x) = 0$。

②证明：另证：$T$为线性映射  
$$T(0) = T(2 \times 0) = 2T(0), \quad T(0) = 0$$  
$$T(-x) = T(-1 \times x) = -T(x)$$  

先证充分性  
当线性映射 $T: \mathbb{R} \rightarrow \mathbb{R}$ 是单射时  
$$T(x) = 0 = T(0)$$  
因为 $T(x)$ 为单射  
所以 $x = 0$，充分性成立  

再证必要性：  
若 $T(x) = 0$ 则 $x = 0$  
假设 $T(x)$ 不是单射  
$
\exists x_1, x_2 (x_1 \neq x_2)$ s.t. $ T(x_1) = T(x_2) $
所以 $T(x_1) - T(x_2)$  
$$= T(x_1 - x_2) = 0$$  
所以  $x_1 - x_2 = 0$ 即 $x_1 = x_2$（矛盾）  
所以 $T(x)$ 为单射，必要性成立  

综上，原命题成立



### 6. 若 $T : \mathbb{R} \rightarrow \mathbb{R}$ 是线性映射，证明 $T$ 是单射当且仅当 $T$ 是满射。

**解:** 解：设 $a = T(1)$

$$T(x) = T(x \cdot 1) = xT(1) = ax$$

先证充分性：

当 $T$ 为单射，则 $a \neq 0$

$\forall y \in \mathbb{R}$，取 $x_0 = \frac{y}{a}$，则 $$T(x_0) = a \cdot \frac{y}{a} = y$$

所以 $T$ 为满射。

再证必要性：

当 $T$ 为满射，则 $a \neq 0$

若存在 $x_1, x_2 \in \mathbb{R}$，使得 $T(x_1) = T(x_2)$，即$$ax_1 = ax_2$$

因为 $a \neq 0$，所以 $x_1 = x_2$，故 $T$ 为单射。

综上，命题成立。





