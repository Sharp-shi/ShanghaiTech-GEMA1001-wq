# <center>hw_4<center> #

## 必做题： ##

### 1. 利用单调有界数列极限存在定理，证明下列数列极限的存在性.

(a) $a_n = \frac{3}{1^2 \cdot 2^2} + \frac{5}{2^2 \cdot 3^2} + \cdots + \frac{2n+1}{n^2(n+1)^2}$

**解：**$a_n - a_{n-1} = \frac{2n+1}{n^2(n+1)^2} > 0$

故 $\{a_n\}$ 单调增加

又因为 $a_n = \frac{1}{1^2} - \frac{1}{2^2} + \frac{1}{2^2} - \frac{1}{3^2} + \cdots + \frac{1}{n^2} - \frac{1}{(n+1)^2}$

$= 1 - \frac{1}{(n+1)^2} < 1$

故 $\{a_n\}$ 存在上界 $1$，s.t. $\forall n \in \mathbb{N}^*$，$a_n < 1$

故由单调有界数列极限存在定理，$a_n$ 极限存在





(b) $a_n = 1 + \frac{1}{2^2} + \frac{1}{3^3} + \cdots + \frac{1}{n^n}$

**解：**$a_n - a_{n-1} = \frac{1}{n^n} > 0$

故 $\{a_n\}$ 单调增加

又因为 $a_n \leq 1 + \frac{1}{2^2} + \frac{1}{3^2} + \cdots + \frac{1}{n^n} \leq 1 + \frac{1}{2^2} + \frac{1}{2^3} + \cdots + \frac{1}{2^n} = 1 + \frac{\frac{1}{4}(1 - (\frac{1}{2})^{n-1})}{1 - \frac{1}{2}} < \frac{3}{2}$

故 $\{a_n\}$ 存在上界 $\frac{3}{2}$，s.t. $\forall n \in \mathbb{N}^*$，$a_n < \frac{3}{2}$

故由单调有界数列极限存在定理，$a_n$ 极限存在



### 2. 证明下列递归数列收敛，并求其极限.

(a) $a_1 > 0$, $a_{n+1} = \frac{1}{2} \left( a_n + \frac{1}{a_n} \right)$ $(n=1,2,\cdots)$

**解：**(a) $a_{n+1} - a_n = \frac{1}{2}(a_n + \frac{1}{a_n}) - a_n$
$= \frac{1}{2}(\frac{1}{a_n} - a_n)$

① $a_n = 1$

② 若 $a_n > 1$
$a_{n+1} - a_n < 0$，$\{a_n\}$ 单调减少且 $\{a_n\}$ 有下界，故 $\{a_n\}$ 收敛

③ 若 $a_n < 1$
$a_{n+1} - a_n > 0$，$\{a_n\}$ 单调增加且 $\{a_n\}$ 有上界，故 $\{a_n\}$ 收敛

取极限
$x = \frac{1}{2}(x + \frac{1}{x})$，$x^2 = 1$，$x = 1$ ($x > 0$)
故极限为 $1$



(b) $a_1 = 1$, $a_{n+1} = 1 + \frac{a_n}{1+a_n}$, $n=1,2,\cdots$

**解：**由例2.5可知 $\{a_n\}$ 单调，且 $1 < a_n < 2$ 故 $a_n$ 收敛

取极限
$x = 1 + \frac{x}{1+x}$
$x = \frac{1+\sqrt{5}}{2} > 0$



(c) $a_1 = 2$, $a_{n+1} = 2 + \frac{1}{a_n}$, $n=1,2,\cdots$

**解：**
$a_{n+1} - a_n = -\frac{a_n - 2}{a_n}$

$a_{n+2} - a_n = -\frac{2(a_n - 1 - \sqrt{2})(a_n - 1 + \sqrt{2})}{2a_n + 1}$

当 $a_n < 1 + \sqrt{2}$，$a_{n+2} - a_n > 0$

$a_n > 1 + \sqrt{2}$，$a_{n+2} - a_n < 0$

故奇偶子列交替围绕 $1 + \sqrt{2}$ 逼近：$a_{2k+1}$ 单调增加且有上界 $1 + \sqrt{2}$，$a_{2k}$ 单调减少且有下界 $1 + \sqrt{2}$

故 $\{a_n\}$ 收敛，极限为 $1 + \sqrt{2}$



### 3. 请写出 $\lim_{x \to \infty} f(x)$ 不存在的严格定义.

**解：**$\forall A \in \mathbb{R}, \exists \epsilon > 0, \forall M > 0, \exists x > M ,|f(x) - A| \geq \epsilon$



### 4. 用定义严格证明 $f(x) = \frac{x(x+3)}{(x-1)(x+2)}$ 在 $x=1$ 处的左极限是 $-\infty$.

**解：**4. $\forall M > 0$，取 $\delta = \min\left\{\frac{1}{2}, \frac{1}{6M}\right\}$  
则当 $x \in (1 - \delta, 1)$ 时  

有  
$f(x) = \frac{x(x+3)}{(x-1)(x+2)} < -M$  
故  
$\lim_{x \to 1^-} f(x) = -\infty$



### 5. 用定义严格证明：$\lim_{x \to \infty} \frac{2x^2 - 1}{x^2 + 3} = 2$.

**解：**$\forall \epsilon > 0$，取 $M = \sqrt{\frac{7}{\epsilon}}$  
$|f(x) - 2| = \left|\frac{2x^2 - 1}{x^2 + 3} - 2\right| = \frac{7}{x^2 + 3} < \epsilon$  
故 
$\forall x > M$，$|f(x) - 2| < \epsilon$  
$\lim_{x \to \infty} \frac{2x^2 - 1}{x^2 + 3} = 2$



### 6. 证明函数 $f(x) = \frac{1}{x} \cos \frac{1}{x}$ 在点 $x=0$ 的邻域内无界，但当 $x \to 0$ 时，并非无穷大.

**解：**①无界：  
令 $x_n = \frac{1}{2n\pi}$，  
$\lim_{n \to \infty} x_n = 0$  
$f(x_n) = 2n\pi \cos(2n\pi) = 2n\pi \to \infty$  
故无界

②非无穷大  
令 $x_n = \frac{1}{2n\pi + \frac{\pi}{2}}$，  
$\lim_{n \to \infty} x_n = 0$  
$f(x_n) = (2n\pi + \frac{\pi}{2}) \cos(2n\pi + \frac{\pi}{2}) = 0$  
故  
$\lim_{n \to \infty} f(x_n) = 0$  
故非无穷大



### 7. 求下列函数在指定点的左、右极限，并判断函数在该点处是否存在极限.

(a) $f(x) = \frac{\sqrt{(x-1)^2}}{x-1}$ 在 $x_0 = 1$ 处.

**解：**
$\lim_{x \to 1^+} f(x) = 1$
$\lim_{x \to 1^-} f(x) = -1$
不存在极限



(b) $f(x) = \frac{2^{\frac{1}{x}} - 1}{2^{\frac{1}{x}} + 1}$ 在 $x_0 = 0$ 处.

**解：**令 $\frac{1}{x} = t$
$\lim_{t \to +\infty} \frac{2^t - 1}{2^t + 1} = 1$
$\lim_{t \to -\infty} \frac{2^t - 1}{2^t + 1} = -1$
不存在极限



### 8. 对函数 $f(x) = x \sin \frac{1}{x}$，证明 $\lim_{x \to 0} f(x) = 0$.并指出下面的计算错误在什么地方？

   $\lim_{x \to 0} x \sin \frac{1}{x} = \lim_{x \to 0} x \lim_{x \to 0} \sin \frac{1}{x} = 0$

**解：**$\lim_{x \to 0} \sin \frac{1}{x}$ 不存在，无法计算




### 9. 计算下面极限

a) $\lim_{x \to 4} \frac{x^2 - 6x + 8}{x^2 - 5x + 4}$

**解：**原式 $= \lim_{x \to 4} \frac{(x-2)(x-4)}{(x-1)(x-4)}$

$= \lim_{x \to 4} \frac{x-2}{x-1} = \frac{2}{3}$



b) $\lim_{x \to 0} \frac{\sqrt{1 + x + x^2} - 1}{\sin 2x}$

**解：**原式 $= \lim_{x \to 0} \frac{x+x^2}{\sin 2x (\sqrt{1+x+x^2}+1)}$

$= \lim_{x \to 0} \frac{1+x}{2\cos 2x (\sqrt{1+x+x^2}+1)}$

$= \frac{1}{4}$



c) $\lim_{x \to -8} \frac{\sqrt{1 - x} - 3}{2 + \sqrt[3]{x}}$

**解：**原式 $= \lim_{x \to -8} \frac{1-x-9}{(2+\sqrt[3]{x})(\sqrt{1-x}+3)}$

$= \lim_{x \to -8} \frac{-x-8}{(2+\sqrt[3]{x})(\sqrt{1-x}+3)}$

$= \lim_{x \to -8} \frac{-(\sqrt[3]{x}^2 - 2\sqrt[3]{x} + 4)}{\sqrt{1-x}+3} = -2$



d) $\lim_{x \to +\infty} \sqrt{x} (\sqrt{x + a} - \sqrt{x})$

**解：**原式 $= \lim_{x \to \infty} \frac{a\sqrt{x}}{\sqrt{x}+\sqrt{x+a}} = \frac{a}{1+\sqrt{1+\frac{a}{x}}} = \frac{a}{2}$



### 10. 计算下面极限

a) $\lim_{x \to a} \frac{\sin x - \sin a}{x - a}$

**解：** 原式 $= \lim_{x \to a} \frac{2 \cos \frac{x+a}{2} \sin \frac{x-a}{2}}{x-a}$  
$= \cos a$



b) $\lim_{x \to \frac{\pi}{2}} \frac{\cos x}{\frac{\pi}{2} - x}$

**解：**令 $t = \frac{\pi}{2} - x$  
原式 $= \lim_{t \to 0} \frac{\cos(\frac{\pi}{2}-t)}{t} = \lim_{t \to 0} \frac{\sin t}{t} = 1$



c) $\lim_{x \to 0} \frac{\sqrt{1 + x \sin x} - \cos x}{\sin^2 \frac{x}{2}}$

**解：**原式 $= \lim_{x \to 0} \frac{x \sin x + \sin^2 x}{\sin^2 \frac{x}{2} (\sqrt{1+x \sin x} + \cos x)}$  
$= \lim_{x \to 0} \frac{4(x \sin x + \sin^2 x)}{x^2 (\sqrt{1+x \sin x} + \cos x)}$  
$= \lim_{x \to 0} \frac{8}{\sqrt{1+x \sin x} + \cos x}$  
$= 4$



d) $\lim_{x \to 1} (1 - x) \tan \frac{\pi x}{2}$

**解：**令 $t = 1 - x$  
原式 $= \lim_{t \to 0} \frac{t \tan \frac{\pi(1-t)}{2}}{t}$  
$= \lim_{t \to 0} \frac{t \cot \frac{\pi t}{2}}{t}$  
$= \lim_{t \to 0} \frac{t}{\tan \frac{\pi t}{2}} = \frac{2}{\pi}$



### 11. 计算下列极限

a) $\lim_{x \to 0} \sqrt[3]{1 - 2x}$

**解：**原式 $= 1$



b) $\lim_{x \to \infty} \left( \frac{2}{x^2} + \cos \frac{1}{x} \right)^{x^2}$

**解：** 令 $t = \frac{1}{x}$  
原式 $= \lim_{t \to 0^+} (2t^2 + \cos t)^{\frac{1}{t^2}}$

$= \lim_{t \to 0^+} (1 + 2t^2 + \cos t - 1)^{\frac{1}{t^2}}$  
$\approx \lim_{t \to 0^+} (1 + \frac{3t^2}{2})^{\frac{1}{t^2}} = e^{\frac{3}{2}}$



c) $\lim_{x \to \infty} \left( \frac{x^2}{x^2 - 1} \right)^x$

**解：**原式 $= \lim_{x \to \infty} \left[ (1 + \frac{1}{x^2 - 1})^{x^2 - 1} \right]^{\frac{x}{x^2 - 1}}$

$= e^0 = 1$



d) $\lim_{x \to 0^+} \sqrt[3]{\cos \sqrt{x}}$

**解：**原式 $= 1$



## 选做题： ##

### 1. 求 ${a_n}$ 的极限，其中 $a_n = \frac{1! + 2! + \cdots + n!}{n!}$, $n = 1, 2, \cdots$.

**解：** $a_n = \frac{1! + 2! + \cdots + n!}{n!} = \frac{1}{n!} + \frac{2!}{n!} + \cdots + 1$

$\lim_{n \to \infty} a_n = 0 + 0 + \cdots + 1 = 1$





### 2. 给定两个正数 $a$ 和 $b$，且有 $0 < b < a$.令 $a_0 = a$, $b_0 = b$，并按递推公式 $a_n = \frac{a_{n-1} + b_{n-1}}{2}$, $b_n = \sqrt{a_{n-1} b_{n-1}}$, $n = 1, 2, \cdots$定义数列 ${a_n}, {b_n}$.证明这两个数列收敛于同一个极限（但不需求出极限值）.

**解：**$a_n = \frac{a_{n-1} + b_{n-1}}{2} > \sqrt{a_{n-1} b_{n-1}} = b_n$

$a_n - a_{n+1} = a_n - \frac{a_n + b_n}{2} > 0$，$\{a_n\}$ 单调减少

$\frac{b_{n+1}}{b_n} = \sqrt{\frac{a_n}{b_n}} > 1$，$\{b_n\}$ 单调增加

$\{a_n\}$ 有下界 $b_0$，$\{b_n\}$ 有上界 $a_0$，故 $\{a_n\}$、$\{b_n\}$ 均收敛

令 $\lim_{n \to \infty} a_n = A$，$\lim_{n \to \infty} b_n = B$

$A = \frac{A+B}{2}$，$A = B$，成立



### 3. 证明：$\lim_{x \to -\infty} a^x = 0$ $(a > 1)$.

**解：**令 $t = -x$

$\lim_{x \to -\infty} a^x = \lim_{t \to +\infty} a^{-t} = \lim_{t \to +\infty} \frac{1}{a^t} = 0$



### 4. 用定义证明 $\lim_{x \to x_0} \sin x = \sin x_0$.

**解：**$\forall \epsilon > 0$，取 $\delta = \epsilon$，当 $|x - x_0| < \delta$ 时

$|\sin x - \sin x_0| = \left| 2 \cos \frac{x + x_0}{2} \sin \frac{x - x_0}{2} \right| \leq 2 \left| \sin \frac{x - x_0}{2} \right| \leq |x - x_0| < \epsilon$

$\lim_{x \to x_0} \sin x = \sin x_0$



### 5. 考虑数列 $x_n = \cos \frac{x}{2} \cos \frac{x}{2^2} \cos \frac{x}{2^3} \cdots \cos \frac{x}{2^n}$.

(a) 证明：$\lim_{n \to \infty} x_n = \frac{\sin x}{x}$（提示：利用 $\sin 2\theta = 2 \sin \theta \cos \theta$）

**解：**$x_n = \frac{\sin x}{2 \sin \frac{x}{2}} \cdot \frac{\sin \frac{x}{2}}{2 \sin \frac{x}{4}} \cdots \frac{\sin \frac{x}{2^{n-1}}}{2 \sin \frac{x}{2^n}}$

$= \frac{\sin x}{2^n \sin \frac{x}{2^n}}$

$\lim_{n \to \infty} x_n = \frac{\sin x}{x} \lim_{n \to \infty} \frac{\frac{x}{2^n}}{\sin \frac{x}{2^n}} = \frac{\sin x}{x}$



(b) 证明 Vieta 公式：$\frac{2}{\pi} = \sqrt{\frac{1}{2}} \sqrt{\frac{1}{2} + \frac{1}{2} \sqrt{\frac{1}{2}}} \sqrt{\frac{1}{2} + \frac{1}{2} \sqrt{\frac{1}{2} + \frac{1}{2} \sqrt{\frac{1}{2}}}} \cdots$（提示：利用 $\cos \frac{\theta}{2} = \sqrt{\frac{1}{2} + \frac{1}{2} \cos \theta}$ 及 $\cos \frac{\pi}{4} = \sqrt{\frac{1}{2}}$）

**解：**$\frac{2}{\pi} = \frac{\sin \frac{\pi}{2}}{\frac{\pi}{2}} = \cos \frac{\pi}{4} \cos \frac{\pi}{8} \cos \frac{\pi}{16} \cdots$

$\cos \frac{\pi}{4} = \sqrt{\frac{1}{2}} \quad \cos \frac{\pi}{8} = \sqrt{\frac{1}{2} + \frac{1}{2}\sqrt{\frac{1}{2}}}$

故 $\frac{2}{\pi} = \sqrt{\frac{1}{2}} \sqrt{\frac{1}{2} + \frac{1}{2}\sqrt{\frac{1}{2}}} \sqrt{\frac{1}{2} + \frac{1}{2}\sqrt{\frac{1}{2} + \frac{1}{2}\sqrt{\frac{1}{2}}}} \cdots$
