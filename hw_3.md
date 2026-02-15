#   <center>hw_3<center>

## 必做题：

### 2. $\forall \alpha > 0$, $\lim_{n \to \infty} \frac{1}{n^\alpha} = ?$ 证明你的论断。

**解：**$$\lim_{n \to \infty} \frac{1}{n^\alpha} = 0$$

证明：$\forall \epsilon > 0$，取 $N = \left\lfloor \left( \frac{1}{\epsilon} \right)^{\frac{1}{\alpha}} \right\rfloor + 1$

当 $n > N$ 时，必有
$$\left| \frac{1}{n^\alpha} - 0 \right| = \frac{1}{n^\alpha} < \epsilon$$

故 $\lim_{n \to \infty} \frac{1}{n^\alpha} = 0$



### 3. 利用夹逼定理计算 $\lim_{n \to \infty} \frac{(2n-1)!!}{(2n)!!}$（其中 $(2n-1)!! = (2n-1)(2n-3) \cdots 5 \cdot 3 \cdot 1$; $(2n)!! = (2n)(2(n-1)) \cdots 4 \cdot 2$）

**解：**
$0 < \frac{(2n-1)!!}{(2n)!!} < \sqrt{\frac{2}{3} \cdot \frac{4}{5} \cdot \frac{6}{7} \cdots \frac{2n}{2n+1} \cdot \frac{1}{2} \cdot \frac{2}{3} \cdot \frac{3}{4} \cdots \frac{2n-1}{2n}} = \frac{1}{\sqrt{2n+1}}$

由于 $\lim_{n \to \infty} \frac{1}{\sqrt{2n+1}} = 0$

故由夹逼定理可知 $\lim_{n \to \infty} \frac{(2n-1)!!}{(2n)!!} = 0$



### 4. 设 $A = \max\{a_1, a_2, \cdots, a_m\}(a_i > 0, i = 1, 2, \cdots, m)$, 证明$\lim_{n \to \infty} \sqrt[n]{a_1^n + a_2^n + \cdots + a_m^n} = A$

**解：**因为 $A = \max\{a_1, a_2, \cdots, a_m\}$

所以  
$$A = (A^n)^{\frac{1}{n}} < (a_1^n + a_2^n + \cdots + a_m^n)^{\frac{1}{n}} < (mA^n)^{\frac{1}{n}} = \sqrt[n]{m} \cdot A$$

由于  $$\lim_{n \to \infty} \sqrt[n]{m}A = A$$  , 由夹逼定理知，  $$\lim_{n \to \infty} \sqrt[n]{a_1^n + a_2^n + \cdots + a_m^n} = A$$



### 5. 计算 $\lim_{n \to \infty} \left( \frac{1}{3n^3 + 2n^2 + 1} + \frac{2^2}{3n^3 + 2n^2 + 1} + \cdots + \frac{n^2}{3n^3 + 2n^2 + 1} \right)$

**解：**$$\lim_{n \to \infty} \left( \frac{1}{3n^3 + 2n^2 + 1} + \frac{2^2}{3n^3 + 2n^2 + 1} + \cdots + \frac{n^2}{3n^3 + 2n^2 + 1} \right)$$

$$= \lim_{n \to \infty} \left[ \frac{1^2 + 2^2 + \cdots + n^2}{3n^3 + 2n^2 + 1} \right]$$

$$= \lim_{n \to \infty} \left[ \frac{n(n+1)(2n+1)}{6(3n^3 + 2n^2 + 1)} \right]$$

$$= \lim_{n \to \infty} \left[ \frac{(1+\frac{1}{n})(2+\frac{1}{n})}{6(3+\frac{2}{n}+\frac{1}{n^3})} \right]$$

$$= \frac{1 \cdot 2}{6 \cdot 3} = \frac{1}{9}$$



### 6. 计算 $\lim_{n \to \infty} \sqrt{n}(\sqrt{n+1}-\sqrt{n})$

**解：** 
$$
\lim_{n \to \infty} \sqrt{n}(\sqrt{n+1} - \sqrt{n})
= \lim_{n \to \infty} \frac{\sqrt{n}}{\sqrt{n+1} + \sqrt{n}}
= \lim_{n \to \infty} \frac{1}{\sqrt{1+\frac{1}{n}} + 1}
= \frac{1}{1 + 1} = \frac{1}{2}
$$



### 7. 利用结论 $\lim_{n \to \infty} \left( 1 + \frac{1}{n} \right)^n = e$

### (a) 计算下列个极限（提示：本质上是凑出 $\left( 1 + \frac{1}{n} \right)^n$ 这种结构，一般地，只要凑出 $\left( 1 + \frac{1}{□} \right)^□$ 就可以了，其中 □ 是任意（正负）无穷大量）

### $\lim_{n \to \infty} \left( 1 + \frac{1}{n^3} \right)^{2n^3} ; \quad \lim_{n \to \infty} \left( 1 + \frac{1}{n} \right)^{(-1)^n \sin n}$

**解：**7. (a)  
$$
\lim_{n \to \infty} \left(1 + \frac{1}{n^3}\right)^{2n^3}
= \lim_{n \to \infty} \left[\left(1 + \frac{1}{n^3}\right)^{n^3}\right]^2
= e^2
$$
$$
\lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^{(-1)^n \sin n}
= \lim_{n \to \infty} \left[\left(1 + \frac{1}{n}\right)^n\right]^{\frac{(-1)^n \sin n}{n}}
= \lim_{n \to \infty} e^{\frac{(-1)^n \sin n}{n}} = e^0 = 1
$$



### (b) 以 $ \lim_{n \to \infty} \left(1 - \frac{1}{n}\right)^{-n} = e $ 为例说明上面提示中说明的合理性。

**解：**(b)  

$$\lim_{n \to \infty} \left(1 - \frac{1}{n}\right)^{-n}$$
$$= \lim_{n \to \infty} \left(\frac{n-1}{n}\right)^{-n}$$
$$= \lim_{n \to \infty} \left(\frac{n}{n-1}\right)^n$$
$$= \lim_{n \to \infty} \left(1 + \frac{1}{n-1}\right)^{n-1} \cdot \left(1 + \frac{1}{n-1}\right)$$
$$= e \cdot 1 = e$$

由提示可知  
$$
\lim_{n \to \infty} \left(1 - \frac{1}{n}\right)^{-n} = \lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n = e
$$
故上面提示中说明合理。



### 8. 计算 $ \lim_{n \to \infty} (n^2 - n + 2)^{\frac{1}{n}} $ 

 **解：**8. 当 $n \to \infty$ 时，有  
$$
n^2 - n + 2 \sim n^2
$$
故  
$$
\lim_{n \to \infty} (n^2 - n + 2)^{\frac{1}{n}}
= \lim_{n \to \infty} (n^2)^{\frac{1}{n}}
$$
$$
= \lim_{n \to \infty} \left(n^{\frac{1}{n}}\right)^2
= \left(\lim_{n \to \infty} n^{\frac{1}{n}}\right)^2
= 1^2 = 1
$$






### 9. 计算 $ \lim_{n \to \infty} \left(\frac{1}{n^2} + \frac{3}{n^2} + \cdots + \frac{2n-1}{n^2}\right) $

**解：**9\. $\lim_{n \to \infty} \left( \frac{1}{n^2} + \frac{3}{n^2} + \cdots + \frac{2n-1}{n^2} \right)$

$= \lim_{n \to \infty} \frac{1 + 3 + 5 + \cdots + (2n-1)}{n^2}$

$= \lim_{n \to \infty} \frac{n^2}{n^2}$

$= 1$



### 10. 计算 $ \lim_{n \to \infty} \left[\frac{1}{1 \cdot 3} + \frac{1}{2 \cdot 4} + \frac{1}{3 \cdot 5} + \cdots + \frac{1}{n(n+2)}\right] $

**解：**$\lim_{n \to \infty} \left[ \frac{1}{1 \cdot 3} + \frac{1}{2 \cdot 4} + \frac{1}{3 \cdot 5} + \cdots + \frac{1}{n(n+2)} \right]$

$= \lim_{n \to \infty} \frac{1}{2} \left( 1 - \frac{1}{3} + \frac{1}{2} - \frac{1}{4} + \frac{1}{3} - \frac{1}{5} + \cdots + \frac{1}{n-1} - \frac{1}{n+1} + \frac{1}{n} - \frac{1}{n+2} \right)$

$= \lim_{n \to \infty} \frac{1}{2} \left( 1 + \frac{1}{2} - \frac{1}{n+1} - \frac{1}{n+2} \right)$

$= \frac{3}{4}$



### 11. 计算 $ \lim_{n \to \infty} \left(1 + \frac{1}{2}\right)\left(1 + \frac{1}{2^2}\right)\left(1 + \frac{1}{2^4}\right)\cdots\left(1 + \frac{1}{2^{2^n}}\right) $

**解：**$\lim_{n \to \infty} (1 + \frac{1}{2}) (1 + \frac{1}{2^2}) (1 + \frac{1}{2^4}) \cdots (1 + \frac{1}{2^{2^n}})$

$= \lim_{n \to \infty} (1 + \frac{1}{2} + \frac{1}{2^2} + \frac{1}{2^3} + \cdots + \frac{1}{2^{2^{n+1}-1}})$

$= \lim_{n \to \infty} (1 - \frac{1}{2^{2^{n+1}}}) \div (1 - \frac{1}{2})$

$= \lim_{n \to \infty} (2 - \frac{1}{2^{2^{n+1}-1}})$

$= 2$



### 12. 计算 $ \lim_{n \to \infty} \left(1 - \frac{1}{1 + 2}\right)\left(1 - \frac{1}{1 + 2 + 3}\right)\cdots\left(1 - \frac{1}{1 + 2 + 3 + \cdots + n}\right) $

**解：**$\lim_{n \to \infty} (1 - \frac{1}{n}) \left( 1 - \frac{1}{1 + 2 + 3} \right) \cdots \left( 1 - \frac{1}{1 + 2 + 3 + \cdots + n} \right)$

$= \lim_{n \to \infty} \frac{1}{2} \cdot \frac{4}{3} \cdot \frac{2}{3} \cdot \frac{5}{4} \cdots \frac{n-1}{n} \cdot \frac{n+2}{n+1}$

$= \lim_{n \to \infty} \frac{1}{n} \cdot \frac{n+2}{3}$

$= \frac{1}{3}$




## 选做题：

### 1. 给定数列 $\{a_n\}$，$\forall m \in \mathbb{N}$，记 $ S_m := \sum_{k=1}^m a_k $，即 $ S_1 = a_1, \quad S_2 = a_1 + a_2, \quad S_3 = a_1 + a_2 + a_3 \cdots $

### 证明：如果 $\{S_m\}$ 收敛，则 $\{a_n\}$ 是无穷小量。并举例说明，$\{a_n\}$ 是无穷小并不能保证 $\{S_n\}$ 的收敛。

**解：**证明：若 $\{ S_n \}$ 收敛，设$\lim_{n \to \infty} S_n = \alpha$

则$a_n = S_{n+1} - S_n$

两边取极限
$\lim_{n \to \infty} a_n = \lim_{n \to \infty} S_{n+1} - \lim_{n \to \infty} S_n = \alpha - \alpha = 0$

故 $\{ a_n \}$ 为无穷小量

举例：
$a_n = \frac{1}{n}$

$S_n = \sum_{i=1}^{n} \frac{1}{i}$ ，为调和级数，是发散的，不收敛



### 2. 证明：若 $ \lim_{n \to \infty} x_n = A $，则 $ \lim_{n \to \infty} \frac{x_1 + \cdots + x_n}{n} = A $。

**解：**2\. $\lim_{n \to \infty} x_n = A$

即 $\forall \epsilon > 0$，$\exists N_1 \in \mathbb{N}$，s.t. $\forall n > N_1$，$|x_n - A| < \frac{\epsilon}{2}$

$\left| \frac{x_1 + \cdots + x_n}{n} - A \right|$

$= \left| \frac{(x_1 - A) + \cdots + (x_n - A)}{n} \right| \leq \frac{|x_1 - A| + \cdots + |x_n - A|}{n}$

将和式分为两部分：
$\frac{|x_1 - A| + \cdots + |x_{N_1} - A|}{n} + \frac{|x_{N_1+1} - A| + \cdots + |x_n - A|}{n}$

对于第二部分：
$\frac{|x_{N_1+1} - A| + \cdots + |x_n - A|}{n} < \frac{n - N_1}{n} \cdot \frac{\epsilon}{2} < \frac{\epsilon}{2}$

对于第一部分：

取 $N_2 = \max \left\{ N_1, \frac{2(|x_1 - A| + \cdots + |x_{N_1} - A|)}{\epsilon} \right\}$

s.t.$\frac{|x_1 - A| + \cdots + |x_{N_1} - A|}{n} < \frac{\epsilon}{2}$

故当 $n > N_2$ 时

$\left| \frac{x_1 + \cdots + x_n}{n} - A \right| < \frac{\epsilon}{2} + \frac{\epsilon}{2} = \epsilon$

故 $\lim_{n \to \infty} \frac{x_1 + \cdots + x_n}{n} = A$