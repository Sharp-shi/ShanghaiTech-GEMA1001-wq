# <center>hw_5<center>

## 必做题

### 1.  
#### (a) 证明：$ y = ax + b $（$ a \ne 0 $）是曲线 $ y = f(x) $ 的渐近线（渐近线的严格定义见讲义《第三讲》附录一）当且仅当  
$$
a = \lim_{x \to +\infty} \frac{f(x)}{x}, \quad b = \lim_{x \to +\infty} (f(x) - ax)
$$
或  
$$
a = \lim_{x \to -\infty} \frac{f(x)}{x}, \quad b = \lim_{x \to -\infty} (f(x) - ax).
$$

**解：**
先证充分性：  
若渐近线为 $ y = ax + b $，则  
$$
a = \lim_{x \to \pm\infty} \frac{f(x)}{x}, \quad b = \lim_{x \to \pm\infty} \left( f(x) - ax \right)
$$

由定义有  
$$
\lim_{x \to \pm\infty} |f(x) - ax - b| = 0
$$

$$
\lim_{x \to \pm\infty} |f(x) - ax| = b
$$

$$
\lim_{x \to \pm\infty} \left| \frac{f(x)}{x} - a - \frac{b}{x} \right| = 0
$$

$$
\Rightarrow \lim_{x \to \pm\infty} \frac{f(x)}{x} = a
$$

故成立. 

再证必要性：  
将 $ a, b $ 代入  
$$
\lim_{x \to \pm\infty} |f(x) - ax - b| = 0
$$

$$
\Rightarrow \lim_{x \to \pm\infty} |f(x) - ax - b| = 0
$$

故 $ y = ax + b $ 为渐近线. 






#### (b) 计算 $ y = \sqrt{3x^2 + 4x + 1} $ 所描绘曲线的渐近线. 

**解：**

(b)  
$\displaystyle \lim_{x \to \infty} f(x) = \infty$ 故不存在水平渐近线. 

对任意 $ x_0 \in (-2, -1] \cup \left[-\frac{1}{3}, +\infty\right) $，有  $\displaystyle \lim_{x \to x_0} f(x) = f(x_0)$ 故也不存在铅直渐近线. 

设渐近线为 $ y = ax + b $ 
$a = \displaystyle \lim_{x \to \infty} \frac{\sqrt{3x^2 + 4x + 1}}{x}
= \displaystyle \lim_{x \to \infty} \sqrt{3 + \frac{4}{x} + \frac{1}{x^2}} = \sqrt{3}$ 
$b = \displaystyle \lim_{x \to \infty} \left( \sqrt{3x^2 + 4x + 1} - \sqrt{3}\,x \right)$

令 $ t = \frac{1}{x} $，当 $ x \to \infty $ 时 $ t \to 0 $，代入得：  
$$
b = \lim_{t \to 0} \left( \sqrt{ \frac{3}{t^2} + \frac{4}{t} + 1 } - \frac{\sqrt{3}}{t} \right)
= \lim_{t \to 0} \left( \sqrt{ \frac{3 + 4t + t^2}{t^2} } - \frac{\sqrt{3}}{t} \right)
= \lim_{t \to 0} \frac{ \sqrt{3 + 4t + t^2} - \sqrt{3} }{t}
$$

$$
= \lim_{t \to 0} \frac{ \sqrt{3} \cdot \left( \sqrt{1 + \frac{4}{3}t + \frac{1}{3}t^2} - 1 \right) }{t}
$$

$$
= \lim_{t \to 0} \sqrt{3} \cdot \frac{ \frac{2}{3}t + o(t) }{t} = \sqrt{3} \cdot \frac{2}{3} = \frac{2\sqrt{3}}{3}
$$

$$
 = \frac{2\sqrt{3}}{3}
$$

因此，渐近线为：  
$$
y = \sqrt{3}\,x + \frac{2\sqrt{3}}{3}
$$




### 2. 当 $ x \to 0 $ 时，确定下列无穷小对于 $ x $ 的阶，并确定其主部：

#### (a) $ \sqrt[3]{x^2} - \sqrt{x} \quad (x \to 0^+) $

**解：**
设其阶为 $ k $
$$
\lim_{x \to 0^+} \frac{\sqrt[3]{x^2} - \sqrt{x}}{x^k}
$$


令 $ k = \frac{1}{2} $，则  
$$
\lim_{x \to 0^+} (x^\frac{1}{6} - 1) = -1
$$

所以，为 $ \frac{1}{2} $ 阶无穷小，主部为 $ -\sqrt{x} $



#### (b) $ \sqrt{a + x^3} - \sqrt{a} \quad (a > 0) $

**解：**

设其阶为 $ k $
$$
\lim_{x \to 0} \frac{\sqrt{a + x^3} - \sqrt{a}}{x^k}
= \lim_{x \to 0} \frac{1}{\sqrt{a + x^3} + \sqrt{a}} \cdot \frac{x^3}{x^k}
= \lim_{x \to 0} \frac{x^{3-k}}{\sqrt{a + x^3} + \sqrt{a}}
$$

当 $ k = 3 $ 时，  
$$
\lim_{x \to 0} \frac{1}{\sqrt{a + x^3} + \sqrt{a}} = \frac{1}{2\sqrt{a}}
$$

所以， 为 3 阶无穷小，主部为 $ \dfrac{x^3}{2\sqrt{a}} $



#### (c) $ \sqrt{1 + \tan x} - \sqrt{1 - \sin x} $

**解：**
设其阶为 $ k $
$$
\lim_{x \to 0} \frac{\sqrt{1 + \tan x} - \sqrt{1 - \sin x}}{x^k}
= \lim_{x \to 0} \frac{\tan x + \sin x}{x^k (\sqrt{1 + \tan x} + \sqrt{1 - \sin x})}
$$

$$
\tan x + \sin x \sim 2x
$$

$$
\sqrt{1 + \tan x} + \sqrt{1 - \sin x} \to 2
$$

所以，令 $ k = 1 $
$$
\lim_{x \to 0} \frac{2x}{x^k \cdot 2} = \lim_{x \to 0} \frac{1}{x^{k-1}} =1
$$

所以，为 1 阶无穷小，主部为 $ x $


#### (d) $ (\cos x)^x - 1 $

**解：**
设其阶为 $ k $
$$
\lim_{x \to 0} \frac{(\cos x)^x - 1}{x^k}
=\lim_{x \to 0}\frac{e^{x \ln(\cos x)} - 1}{x^k} =\lim_{x \to 0}\frac{{x \ln(\cos x)} }{x^k}=\lim_{x \to 0}\frac{{x \ln[1-\frac{x^2}{2}+o(x^2)]} }{x^k} =\lim_{x \to 0}\frac{-\frac{x^2}{2} + O(x^2)}{x^{k-1}}
$$



令 $ k = 3 $，极限为 $ -\frac{1}{2} $

所以，为 3 阶无穷小，主部为 $ -\frac{x^3}{2} $




### 3. 求下列各题中的常数 $ a $（或 $ a, b $）：

#### (a) $ \displaystyle \displaystyle \lim_{x \to \infty} \left( \frac{x + 2a}{x - a} \right)^x = 8 $

**解：** 
$$
\lim_{x \to \infty} \left( \frac{x + 2a}{x - a} \right)^x
= \lim_{x \to \infty} \left( 1 + \frac{3a}{x - a} \right)^{x - a} \cdot \left( 1 + \frac{3a}{x - a} \right)^a
= e^{3a}=8\\
a = \ln 2
$$



#### (b) 当 $ x \to 0 $ 时，$ \sqrt[4]{1 + a x^2} - 1 $ 与 $ \cos x - 1 $ 是等价无穷小

**解：**

$$
\lim_{x \to 0} \frac{\sqrt[4]{1 + a x^2} - 1}{\cos x - 1} 

\\= \lim_{x \to 0} \frac{\frac{1}{4} a x^2 + o(x^2)}{-\frac{1}{2} x^2 + o(x^2)} \\= -\frac{1}{2} a=1
$$

故 $$ a = -2 $$



#### (c) $ \displaystyle \displaystyle \lim_{x \to \infty} \left( \frac{x^2 + 1}{x + 1} - a x - b \right) = 0 $，并指出该计算的几何意义

**解：**
]
$$
\lim_{x \to \infty} \left( \frac{x^2 + 1}{x + 1} - a x - b \right) = 0
= \lim_{x \to \infty} \left( x - 1 + \frac{2}{x + 1} - a x - b \right)
= \lim_{x \to \infty} \left[ (1 - a)x - (b + 1) + \frac{2}{x + 1} \right]
$$

$ 1 - a = 0 \Rightarrow a = 1 $

$-(b + 1) = 0 \Rightarrow b = -1 $

因此：  
$$
a = 1, \quad b = -1
$$

故渐近线为：  
$$
y = x - 1
$$

即 $ y = x - 1 $ 是曲线 $ \dfrac{x^2 + 1}{x + 1} $ 的斜渐近线. 



#### (d) $ \displaystyle \displaystyle \lim_{x \to +\infty} \left( 3x - \sqrt{a x^2 - b x + 1} \right) = 2 $，并指出该计算的几何意义

**解：**
(d)  
$$
\lim_{x \to +\infty} \left( 3x - \sqrt{a x^2 - b x + 1} \right)
\\= \lim_{x \to +\infty} \frac{
(3x - \sqrt{a x^2 - b x + 1})(3x + \sqrt{a x^2 - b x + 1})
}{3x + \sqrt{a x^2 - b x + 1}}
\\= \lim_{x \to +\infty} \frac{
9x^2 - (a x^2 - b x + 1)
}{3x + \sqrt{a x^2 - b x + 1}}
\\= \lim_{x \to +\infty} \frac{
(9 - a)x^2 + b x - 1
}{3x + \sqrt{a x^2 - b x + 1}}
\\\\9 - a = 0 \\ a = 9
$$

代入后：  
$$
= \lim_{x \to +\infty} \frac{
b x - 1
}{3x + \sqrt{9x^2 - b x + 1}}
= \lim_{x \to +\infty} \frac{
b - \frac{1}{x}
}{3 + \sqrt{9 - \frac{b}{x} + \frac{1}{x^2}}}
b = 12
$$

因此：  
$$
a = 9, \quad b = 12
$$

故 $y = 3x - 2$是曲线 $ y = \sqrt{9x^2 - 12x + 1} $ 的斜渐近线. 




### 4. 计算下列极限（可用无穷小（大）替换）：

#### (a) $ \displaystyle \displaystyle \lim_{x \to 0} \frac{1 - \cos x}{x^2} $

**解：**
原式 = $\displaystyle\displaystyle \lim_{x \to 0} \frac{\frac{1}{2}x^2 + o(x^2)}{x^2}
= \displaystyle \lim_{x \to 0} \left( \frac{1}{2} + \frac{o(x^2)}{x^2} \right)
= \frac{1}{2}$




#### (b) $ \displaystyle \displaystyle \lim_{x \to 0} \frac{(e^x - 1) \ln(1 + x)}{\tan x \sqrt{1 - x^2} - 1} $

**解：**

原式=  $\displaystyle \displaystyle \lim_{x \to 0} \frac{[x + o(x)][x + o(x)]}{[x + o(x)] - 1}
= \displaystyle \lim_{x \to 0} \frac{x^2 + o(x^2)}{x - 1 + o(x)} = 0$



#### (c) $ \displaystyle \displaystyle \lim_{x \to 0} \frac{\ln \cos(ax)}{\ln \cos(bx)} \quad (a, b \ne 0) $

**解：**
$$
原式 = \lim_{x \to 0} \frac{\ln\left[1 - \frac{1}{2}a^2 x^2 + o(x^2)\right]}{\ln\left[1 - \frac{1}{2}b^2 x^2 + o(x^2)\right]}
\\= \lim_{x \to 0} \frac{-\frac{1}{2}a^2 x^2 + o(x^2)}{-\frac{1}{2}b^2 x^2 + o(x^2)}
\\= \lim_{x \to 0} \frac{-\frac{1}{2}a^2 + o(1)}{-\frac{1}{2}b^2 + o(1)}
\\= \frac{a^2}{b^2}
$$



#### (d) $ \displaystyle \displaystyle \lim_{x \to 0} \left( 2x + 3x^2 \right)^{1/x} $

**解：**
原式 = $\displaystyle \displaystyle \lim_{x \to 0} e^{\frac{1}{x} \ln(2x + 3x^2)}$
$= \displaystyle\displaystyle \lim_{x \to 0} e^{\frac{1}{x} [\ln x + \ln(3x + 2)]}$

$= \displaystyle\displaystyle \lim_{x \to 0} e^{\frac{1}{x} [\ln x + 3x + 1 + o(x)]}$

$= \displaystyle\displaystyle \lim_{x \to 0} e^{\frac{\ln(ex)}{x} +3}$

$= e^{-\infty} = 0$



### 5. 已知当 $ x \to 0 $ 时，$ f(x) $ 是比 $ x $ 高阶的无穷小，且  $\displaystyle \displaystyle \lim_{x \to 0} \frac{\ln\left(1 + \dfrac{f(x)}{\sin 2x}\right)}{3^x - 1} = 5,$求 $ \displaystyle \displaystyle \lim_{x \to 0} \frac{f(x)}{x^2} $

**解：**
$$
\lim_{x \to 0} \frac{\ln\left(1 + \dfrac{f(x)}{\sin 2x}\right)}{3^x - 1}
$$

$$
= \lim_{x \to 0} \frac{\dfrac{f(x)}{\sin 2x}}{( \ln 3 ) x}
= \lim_{x \to 0} \frac{f(x)}{\sin 2x \cdot (\ln 3) x}
$$

$$
= \lim_{x \to 0} \frac{f(x)}{2x \cdot (\ln 3) x}
= \lim_{x \to 0} \frac{f(x)}{2x^2 \ln 3}=5
$$

$$
\lim_{x \to 0} \frac{f(x)}{x^2} = 10 \ln 3
$$



### 6. 求下列函数的间断点，并确定其类型；若为可去间断点，补充或修改定义使之连续：

#### (a) $ y = \dfrac{\dfrac{1}{x} - \dfrac{1}{1+x}}{\dfrac{1}{x-1} - \dfrac{1}{x}} $

**解：**
$y = \frac{x - 1}{x + 1}$

$ x = -1 $ 分母为 0，分子为 $ -2 \ne 0 $，故为 **无穷间断点**

$ x = 0 $ 原函数无定义，但极限存在：
$$
\lim_{x \to 0} \frac{x - 1}{x + 1} = \frac{-1}{1} = -1
$$
故为 **可去间断点**

补充定义 $ y(0) = -1 $ 

$ x = 1 $ 原函数无定义，但极限存在：
$$
\lim_{x \to 1} \frac{x - 1}{x + 1} = 0
$$
故为 **可去间断点**

补充定义 $ y(1) = 0 $ 



#### (b) $ y = \ln |\cos x| $

**解：**
(b)  

当 $ \cos x = 0 $ 时，函数无定义  
$x = \frac{\pi}{2} + k\pi, \quad k \in \mathbb{Z}$$ |\cos x| \to 0^+ $

所以 $ \ln |\cos x| \to -\infty $，故为 **无穷间断点**



#### (c) $ y = \left[ \dfrac{1}{|x|} + 1 \right] $

**解：**

$ x = 0 $  因为$ \dfrac{1}{|x|} \to +\infty $，故 $ y \to +\infty $，为 **无穷间断点**

$ x = \pm \dfrac{1}{n - 1} $，$ n = 2,3,\dots $  为 **跳跃间断点**



#### (d) $ y = \dfrac{1}{1 + e^{\frac{1}{x-1}}} $

**解：**

$ x = 1 $ 

当 $ x \to 1^- $，$ y \to 0 $

当 $ x \to 1^+ $，$ y \to 1 $

$ x = 1 $为 **跳跃间断点**



### 7. 求下列各题中的常数 $ a, b $ 的值，使得函数连续：

#### (a) 
$$
f(x) = 
\begin{cases}
\dfrac{\sin(ax)}{x}, & x < 0 \\
1, & x = 0 \\
\frac{b(\sqrt{1 + x} - 1)}{x}, & x > 0
\end{cases}
$$

**解：**
$$
\lim_{x \to 0^-} \frac{\sin ax}{x} = a = 1
$$

$$
\lim_{x \to 0^+} \frac{b(\sqrt{1+x}-1)}{x} = \frac{b \cdot (\frac{1}{2}x)}{x} = \frac{1}{2} b = 1
$$

所以，$a = 1, b = 2$





#### (b)

$$
f(x) = \lim_{n \to \infty} \frac{x^{2n - 1} + a x^2 + b x}{x^{2n} + 1}
$$

**解：**

当 $|x| < 1$  
$$
f(x) = \lim_{n \to \infty} \frac{1 + a x^{2n} + b x^{2n-1}}{1 + x^{2n}} = 1
$$

当 $|x| > 1$  
$$
f(x) = \lim_{n \to \infty} \frac{x^{-2n} + a + b x^{-1}}{1 + x^{-2n}} = a + \frac{b}{x}
$$

当 $x = 1$  
$$
f(x) = \frac{1 + a + b}{2}
$$

当 $x = -1$  
$$
f(x) = \frac{1 + a - b}{2}
$$

$x \to 1^+$  
$$
a + \frac{b}{1} = \frac{1 + a + b}{2}
$$

$x \to -1^-$  
$$
a + \frac{b}{-1} = \frac{1 + a - b}{2}
$$

解得 $a = 0, b = 1$




### 8. 讨论函数  $f(x) = \begin{cases}x^a \sin \dfrac{1}{x}, & x > 0 \\e^x + b, & x \le 0\end{cases}$ 的连续性，其中 $ a, b $ 是任意常数. 

**解：**$ f(0) = 1+b $
$$
f(0-0) = \lim_{x \to 0^-} f(x) = \lim_{x \to 0^-} (e^x + b) = 1 + b = f(0)
$$

$a > 0$ 时   $ f(0+0) = \displaystyle\displaystyle \lim_{x \to 0^+} f(x) = 0 $

$a = 0$ 时  $\displaystyle\displaystyle \lim_{x \to 0} f(x)$不存在  

$a < 0$ 时  $f(x)$ 当 $x \to 0^+$ 时无穷振荡且振幅 $x^a$ 趋于 $+\infty$，故 $f(0+0)$不存在  

综上，$b = -1$ 时，当 $a > 0$，使 $f(0)$ 在 $0$ 处连续，否则振荡间断点  
	   $b \neq -1$ 时，当 $a > 0$，$0$ 为跳跃间断点  
				      $a \leq 0$，$0$ 为振荡间断点



### 9. 假设 $ f $ 在 $[0, 4]$ 上连续，且  $f(0) = f(2) = f(4) = 1, \quad f(1) = f(3) = -1.$试问：方程 $ f(x) = 0 $ 在 $[0, 4]$ 上解的个数？

**解：**由零点存在定理

在 $(0,1)  (1,2)  (2,3)  (3,4)$ 各有一个零点

故 $f(x) = 0$ 在 $[0,4]$ 上至少有 4 个不同的解



### 10. 证明方程 $ x = a \sin x + b $（$ a, b > 0 $）至少有一个正根. 

**解：**

$$
f(x) = a \sin x + b - x
$$

$$
f(0) = b > 0
$$

$$
f(a+b+1) = a \sin (a+b+1) + b - a - b - 1
$$

$$
= a [\sin (a+b+1)-1] - 1 < 0
$$

由零点存在定理，$f(x)$ 在 $(0, a+b+1)$ 上至少存在一个正根



### 11. 证明：对偶数次多项式方程  $f(x) = x^{2n} + a_1 x^{2n - 1} + \cdots + a_{2n - 1} x + a_{2n} = 0,$若 $ a_{2n} < 0 $，则它至少有两个实根. 

**解：**$f(0) = a_{2n} < 0$

因为其为偶数次

所以  
$x \to +\infty$ 时 $f(x) \to +\infty$

$x \to -\infty$ 时 $f(x) \to +\infty$

由零点存在定理，$f(x) = 0$ 至少有 2 个实根. 



### 12. 设函数 $ f(x), g(x) \in C[a, b] $，且 $ f(a) < g(a) $，$ f(b) > g(b) $. 

### 证明：存在 $ \xi \in (a, b) $，使得 $ f(\xi) = g(\xi) $. 

**解：**
$\begin{aligned}
& h(x) = f(x) - g(x) \\
&\quad h(a) < 0 \quad h(b) > 0
\end{aligned}$
由零点存在定理，$\exists \xi \in [a,b], h(\xi) = 0$

即 $f(\xi) = g(\xi)$



### 13. 设 $ f(x) \in C[0, 2] $，且 $ f(0) = f(2) $. 

### 证明：存在 $ x, y \in [0, 2] $，满足 $ y - x = 1 $，使得 $ f(x) = f(y) $. 

**解：**
$g(x) = f(x) - f(x+1)$，$\lambda \in [0, 1]$  
$$
g(0) = f(0) - f(1)
$$

$$
g(1) = f(1) - f(2) = f(1) - f(0) = -g(0)
$$

当 $g(0) = 0$，则取 $x = 0, y = 1$  

当 $g(0) \neq 0$  
$g(0) \cdot g(1) < 0$  

由零点存在定理  
$\exists \xi \in [0, 1], g(\xi) = 0$  

即  
$f(\xi) = f(\xi + 1)$  
$x = \xi, y = \xi + 1$



## 选做题

### 1. 设 $ f(x) \in C(\mathbb{R}) $，且 $ \displaystyle \displaystyle \lim_{x \to \infty} f(x) = A $（有限值）.   
###  证明：$ f(x) $ 在 $ \mathbb{R} $ 上有界. 

**解：**$\forall \epsilon > 0, \exists X_1 > 0, s.t. \forall |x| > X_1, |f(x) - A| < 1$

故 $\forall x > X_1, |f(x)| \leq |A| + 1$,

$f(x)$ 在 $[-X_1, X_1]$ 上有界

$\exists X_2 > 0, \forall |x| \leq X_1, |f(x)| \leq X_2$

则取 $X_3 = \max \{X_1, X_2\}$

$\forall x \in \mathbb{R}, |f(x)| \leq X_3$, $f(x)$ 在 $\mathbb{R}$ 有界

### 2. 证明：当 $ x \to 0 $ 时，无穷小量 $ x \sin \dfrac{1}{x} $ 没有阶. 

**解：**2、设其阶为 $k$，求 $\displaystyle\displaystyle \lim_{x \to 0} \frac{x \sin \frac{1}{x}}{x^k}$ 构建两组数列  
$$
a_n = \frac{1}{2\pi n}, \quad b_n = \frac{1}{2\pi n + \frac{\pi}{2}}\\ \quad \lim_{n \to \infty} a_n = \lim_{n \to \infty} b_n = 0
$$
$$
\sin \frac{1}{a_n} = 0, \quad \sin \frac{1}{b_n} = 1
$$
$$
\frac{a_n \sin \frac{1}{a_n}}{a_n^k} = 0
$$
$$
\lim_{n \to \infty} \frac{b_n \sin \frac{1}{b_n}}{b_n^k} = \lim_{n \to \infty} b_n^{1-k} \neq 0
$$

故 $\displaystyle\displaystyle \lim_{x \to 0} \frac{x \sin \frac{1}{x}}{x^k}$ 不存在  
故 $k$ 不存在，阶不存在



### 3. 设 $ \varphi(x) $ 在 $ x = 0 $ 处连续，且 $ \varphi(0) = 0 $，及 $ |f(x)| \le |\varphi(x)| $. 

### 证明：$ f(x) $ 在 $ x = 0 $ 处连续. 

**解：**

 $|f(0)| \leq |\varphi(0)| = 0$$\Rightarrow f(0) = 0$

$-|\varphi(x)| \leq f(x) \leq |\varphi(x)|$

由夹逼定理

$$\displaystyle \lim_{x \to 0} -|\varphi(x)| = \displaystyle \lim_{x \to 0} f(x) = \displaystyle \lim_{x \to 0} |\varphi(x)| = 0$$

故 $f(x)$ 在 $x=0$ 处连续



### 4. 设 $ f(x) \in C[0, 1] $，且 $ f(0) = f(1) $.   
###   证明：对任意 $ n \in \mathbb{N}^+ $，存在 $ \xi_n \in [0, 1] $，使得  $f(\xi_n) = f\left( \xi_n + \frac{1}{n} \right).$

**解：**

令 $g(x) = f(x) - f(x + \frac{1}{n})$
$$
S = \sum_{i=0}^{n-1} g(\frac{i}{n}) = f(0) - f(1) = 0
$$

若 $\forall i, g(\frac{i}{n}) > 0$，则 $S > 0$，矛盾  
若 $\forall i, g(\frac{i}{n}) < 0$，则 $S < 0$，矛盾  

故 $\exists i,$ $ s.t.$ $ g(\frac{i}{n}) = 0$  

或 $n$ 个数中有正有负  

$\exists i_1, i_2,$  $ s.t.$  $ g(i_1) > 0, g(i_2) < 0$

故 $\exists \xi_n \in (i_1, i_2), $ $s.t.$ $ g(\xi_n) = 0$

故 $\exists \xi_n \in [0, 1], $ $s.t.$ $ f(\xi_n) = f(\xi_n + \frac{1}{n})$



### 5. 设 $ f(x) \in C[0, 1] $，且 $ f(x) $ 只取有理值，若 $ f\left( \dfrac{1}{3} \right) = 2 $，

### 证明：对任意 $ x \in [0, 1] $，有 $ f(x) = 2 $. 

**解：** 若 $f(x)$ 不恒等于 $2$  
故 $\exists x_0 \in [0,1]$, s.t. $f(x_0) \neq 2$  
令 $f(x_0) = t$, $t \in \mathbb{Q}$ 且 $t \neq 2$  
考虑以 $\frac{1}{3}$ 与 $x_0$ 为端点的区间 $I$  
由于 $f(x) \in C[0,1]$, $f(x)$ 在 $I$ 上连续  
对于 $2$ 与 $t$ 之间的任意值 $k$, $\exists x_k \in I$, s.t. $f(x_k) = k$  
若 $k$ 为无理数，$f(x_k) = k$ 不成立  
故矛盾，故 $f(x) = 2$ 在 $[0,1]$ 上恒成立
