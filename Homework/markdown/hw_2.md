# <center>hw_2<center>

## 必做题：

### 1. 数集 $E = \left\{ 1, \frac{1}{2}, \frac{1}{3}, \cdots, \frac{1}{n}, \cdots \right\}$ 的下确界是多少？证明你的结论.

**解: **$\inf E = 0$

证明: $\forall n, \frac{1}{n} > 0$，故 $0$ 为 $E$ 的一个下界

下证明，$\forall \epsilon > 0$，$\exists k$，s.t. $\frac{1}{k} < \epsilon + 0$

取 $k = \left[\frac{1}{\epsilon}\right] + 1$，则 $k > \frac{1}{\epsilon}$

所以 $\frac{1}{k} < \epsilon$，$\inf E = 0$



### 2. 对非空数集 $E$，证明若 $\inf E$ 存在，则其必唯一.

**解: **假如 $\inf E$ 不唯一，可设 $\alpha$ 与 $\alpha'$ 为 $E$ 的两不同下确界，

则根据下确界的定义，有 $\alpha \leq \alpha'$ 且 $\alpha' \leq \alpha$，故 $\alpha = \alpha'$，

则若 $\inf E$ 存在，则其必唯一



### 3. 用定义严格证明：$y = \frac{1}{x^2}$ 在 $(0, +\infty)$ 内无界.

**解: **③ $y = \frac{1}{x^2} > 0$ 故有下界  
下证明，$\forall M > 0$，$\exists x > 0$，s.t. $\frac{1}{x^2} > M$  
取 $x = \frac{1}{\sqrt{M}+1} < \frac{1}{\sqrt{M}}$  
即 $\frac{1}{x^2}  > M$  
故 $y = \frac{1}{x^2}$ 在 $(0,+\infty)$ 无上界即无界



### 4. 如果数列的一般项可写成 $a_n = f(n)$ 的形式，其中 $f$ 是 $\mathbb{R}$ 上的函数（或至少是 $[1, +\infty)$ 上的函数），证明：如 $f$ 单调增加，则 $\{a_n\}$ 亦单调增加.

**解: **④若 $f$ 单调增加  
则  $$\forall x_1, x_2 \in \mathbb{R} (x_1 < x_2), \quad f(x_1) \leq f(x_2)$$
所以  $$\forall n \in \mathbb{N}^*, \quad f(n) \leq f(n+1)$$
即 $a_n \leq a_{n+1}$，故 $\{a_n\}$ 单调增加。



### 5. 数列 $\left\{\frac{n+3}{n+1}\right\}$ 是否单调？是否有界？证明你的论断.

**解: **(1) 单调性：

设 $x_n = \frac{n+3}{n+1}$，比较前后两项  
$$x_{n+1} - x_n = \frac{n+4}{n+2} - \frac{n+3}{n+1} = \frac{n^2 + 5n + 4 - n^2 - 5n - 6}{(n+2)(n+1)} = -\frac{2}{(n+2)(n+1)} < 0$$

即 $x_{n+1} < x_n$，故该数列单调递减  

(2) 有界性： 
因为 $\{x_n\}$ 单调递减 
故 $x_n \leq x_1 = 2$ 
又因为 $x_n = \frac{n+3}{n+1} = 1 + \frac{2}{n+1} > 1$ 
故 $1 < x_n \leq 2$，该数列有界



### 6. 数列 $\{x_n\}$ 由 $x_{n+1} = x_n(1 - x_n)$ 给出，且初始值满足 $0 < x_1 < 1$，证明它是单调的且有下界. 并求其极限.

**解: **证明：单调性：
$$x_{n+1} - x_n = x_n(1 - x_n) - x_n = -x_n^2$$
若 $x_n = 0$，则 $x_{n+1} = x_n = 0$，矛盾，故 $x_n ≠ 0$ 
所以 $x_{n+1} - x_n < 0$

即 $x_{n+1} < x_n$，$\{x_n\}$ 是单调递减的

下界：$0 < x_1 < 1$  
注意到 $x_2 = x_1(1 - x_1) \in (0,1)$  
设 $x_k \in (0,1)$，则对 $n = k + 1$  
有 $x_{k+1} = x_k(1 - x_k) \in (0,1)$

故由数学归纳法知 $\{x_n\}$ 有下界

极限：因为 $\{x_n\}$ 单调递减且有下界，所以 $\{x_n\}$ 存在极限  
设 $$\lim_{n \to \infty} x_n = A$$
由$$x_{n+1} = x_n(1 - x_n)$$
得$$A = A(1 - A)$$
$A = 0$

故极限为 $0$



### 7. 用极限的定义严格证明 $$\lim_{n \to \infty} \frac{3n + 7}{2n + 13} = \frac{3}{2}$$.

**解: **证明：$\forall \epsilon > 0$

取 $N = \left[ \frac{25}{4\epsilon} - \frac{13}{2} \right] + 1$

当 $n > N$ 时，必有

$$|x_n - \frac{3}{2}| = \left| \frac{3n+7}{2n+13} - \frac{3}{2} \right| = \frac{25}{2(2n+13)} < \frac{25}{2(2\cdot \frac{25}{4\epsilon} - 13 + 13)} = \epsilon$$

所以
$$\lim_{n \to \infty} \frac{3n+7}{2n+13} = \frac{3}{2}$$



### 8. 用极限的定义严格证明 $$\lim_{n \to \infty} \frac{n!}{n^n} = 0$$.

**解: **因为  
$$\frac{n!}{n^n} = \frac{n \cdot (n-1) \cdots 1}{n \cdot n \cdots n} = \frac{n}{n} \cdot \frac{n-1}{n} \cdots \frac{1}{n} < \frac{1}{n}$$  

故 $\forall \epsilon > 0$，取 $N = \left[\frac{1}{\epsilon} \right] + 1$，则当 $n > N$ 时，有  
$$\left| \frac{n!}{n^n} \right| < \frac{1}{n} < \epsilon$$  

故  $$\lim_{n \to \infty} \frac{n!}{n^n} = 0$$



### 9. 用定义证明 $$a_n = \frac{1}{n} \sin \frac{n\pi}{2}$$ 是无穷小.

**解: **证明：

$$\forall \epsilon > 0, \, \text{取} N = \left[ \frac{1}{\epsilon} \right] + 1, \, \text{则当} n > N \, \text{时，有} \left| \frac{1}{n} \sin \frac{n\pi}{2} \right| < \frac{1}{n} < \epsilon$$

故 $a_n = \frac{1}{n} \sin \frac{n\pi}{2}$ 为无穷小。



### 10. 用定义证明 $$a_n = \frac{n^2 + 1}{2n - 1}$$ 是无穷大.

**解: **证明：

$$\forall G > 0, \, \text{取} N = \left[ {2}{G} \right] + 1, \, \text{则当} n > N \, \text{时，有} \left| \frac{n^2+1}{2n-1} \right| > \frac{n}{2} > G$$

故 $a_n = \frac{n^2+1}{2n-1}$ 为无穷大。



### 11. 设 $\{x_n\}$ 是无穷大量，$\{y_n\}$ 满足：$\exists \delta > 0$，$\exists N \in \mathbb{N}$，使得 $\forall n \geq N$，有 $|y_n| \geq \delta$，证明 $\{x_n y_n\}$ 是无穷大量.

**解: ** $\forall G > 0$，$\exists N_1 \in \mathbb{N}$，s.t. 当 $n > N_1$ 时，有 $|x_n| >G/\delta$  
$\exists \delta > 0$，$\exists N_2 \in \mathbb{N}$，s.t. 当 $n > N_2$ 时，有 $|y_n| \geq \delta$  

故 $\forall G > 0$，取 $N = \max\{N_1, N_2\}$  
则当 $n > N$ 时，$|x_n y_n| \geq |\delta x_n| >  G$  

故 $\{x_n y_n\}$ 为无穷大量




### 12. 举出满足下列要求的数列的例子.
### (1) 有界数列但无极限； (2) 无界数列但不是无穷大

**解: **(1) $a_n = (-1)^n$

(2) $a_n = \begin{cases} 
n & \text{当 } n \text{ 为奇数} \\
0 & \text{当 } n \text{ 为偶数}
\end{cases}$



## 选做题：

### 1. 设数集 $E$ 有上界，证明：数集 $-E := \{x \mid -x \in E\}$ 有下界，且 $\sup E = -\inf (-E)$.

**解: **(1) 设 $E$ 的上界为 $M$，即 $\forall x \in E$，有 $x \leq M$  
   对于数集 $-E$，$\forall y \in -E$，$\exists x \in E$，s.t. $y = -x$  
   因为 $x \leq M$，故 $y = -x \geq -M$，故 $-M$ 为 $-E$ 的一个下界  

(2)设 $E$ 的上确界为 $\beta$，即 $\forall \epsilon > 0$，$\exists x \in E$，s.t. $x > \beta - \epsilon$  
对于数集 $-E$，由上式知 $-\beta$ 为 $-E$ 的上界，且 $y = -x$，$\beta$ 为 $E$ 的最小上界，则 $-\beta$ 为 $-E$ 的最大下界  
故 $-\inf(-E) = \beta = \sup E$



### 2. 对非空数集 $A, B$，定义其和为 $A + B := \{a + b \mid a \in A, b \in B\}$。证明：若 $A, B$ 皆有上界，则 $A + B$ 亦有上界，且 $\sup (A + B) = \sup A + \sup B$.

**解: **

(1) 设 $A$ 的上界为 $M_1$，$B$ 的上界为 $M_2$，即  
$$\forall x_1 \in A, \, x_1 \leq M_1$$
$$\forall x_2 \in B, \, x_2 \leq M_2$$
则对于数集 $A+B$，  
$$\forall x \in (A+B), \, x = x_1 + x_2 \leq M_1 + M_2$$
故 $A+B$ 亦有上界。

(2) 设 $A$ 的上确界为 $\beta_1$，$B$ 的上确界为 $\beta_2$，即  
$$\forall \epsilon > 0, \, \exists x_1 \in A \, \text{s.t.} \, x_1 > \beta_1 - \frac{\epsilon}{2}$$
$$\forall \epsilon > 0, \, \exists x_2 \in B \, \text{s.t.} \, x_2 > \beta_2 - \frac{\epsilon}{2}$$
对于数集 $A+B$，  
$$\forall \epsilon > 0, \, \exists x \in (A+B) \, \text{s.t.} \, x = x_1 + x_2 > \beta_1 + \beta_2 - \epsilon$$
故 $$\sup(A+B) = \beta_1 + \beta_2 = \sup A + \sup B$$




### 3. 若数列 $a_n$ 满足 $a_n \leq qa_{n-1}$，其中 $a_n > 0, 0 < q < 1$，试用定义证明  $$\lim_{n \to \infty} a_n = 0$$.

**解: **(3) $\forall \epsilon > 0$，取 $N = \left\lfloor \frac{\ln \epsilon - \ln a_1}{\ln q} \right\rfloor + 1$

当 $n > N$ 时，有 $a_n \leq q^{n-1} \cdot a_1 < \epsilon$

故  $$\lim_{n \to \infty} a_n = 0$$



### 4. 设有数列 $\{a_n\}$ 和 $\{b_n\}$，如果  $$\lim_{n \to \infty} \frac{a_n}{b_n} = a(a \neq 0)$$ 且 $$\lim_{n \to \infty} a_n = 0$$ 证明 $$\lim_{n \to \infty} b_n = 0$$.

**解: **(4)  
$$\lim_{n \to \infty} \frac{a_n}{b_n} = a \quad (a \neq 0)$$

故 $$\exists N_1 \in \mathbb{N}, \, \text{s.t.} \, \left| \frac{a_n}{b_n} \right| > \frac{|a|}{2}$$

所以 $$|b_n| < |a_n| \cdot \frac{2}{|a|}$$

因为  $$\lim_{n \to \infty} a_n = 0, \, \forall \epsilon > 0, \, \exists N_2 \in \mathbb{N}, \, \text{s.t.} \, \text{当 } n > N_2, \, |a_n| < \epsilon \cdot \frac{|a|}{2}$$

取 $N = \max\{N_1, N_2\}$，则当 $n > N$ 时，

$$|b_n| < \epsilon \cdot \frac{|a|}{2} \cdot \frac{2}{|a|} = \epsilon$$

故  $$\lim_{n \to \infty} b_n = 0$$





