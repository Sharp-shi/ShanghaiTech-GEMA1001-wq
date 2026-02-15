# <center>hw_8<center>
## 必做题：
### 1. 设 $f(x) = (a + b \cos x) \sin x - x$ 当 $x \to 0$ 时是 $x$ 的五阶无穷小，求 $a, b$. 

**解：**
$$
\sin x = x - \frac{x^3}{6} + \frac{x^5}{120} + o(x^5)
$$

$$
\cos x = 1 - \frac{x^2}{2} + \frac{x^4}{24} + o(x^4)
$$

$$
f(x) = [a + b(1 - \frac{x^2}{2} + \frac{x^4}{24})] (x - \frac{x^3}{6} + \frac{x^5}{120}) - x + o(x^5)
$$

$x$ 系数：$(a+b) - 1$

$x^3$ 系数：$-\frac{a+b}{6} - \frac{b}{2} = -\frac{a+b}{6}$

$x^5$ 系数：$\frac{a+b}{120} + \frac{b}{12} + \frac{b}{24} = \frac{a+b}{120}$

故

$$
\begin{cases}
a+b-1 = 0 \\
\frac{a+b}{6} = 0 \\
\frac{a+b}{120} != 0
\end{cases}
$$

$a = \frac{4}{3}$

$b = -\frac{1}{3}$




### 2. 利用极值判别法 $I$ 求下列函数的极值：

#### $a) \, y = \frac{\ln^2 x}{x}, $

**解：**
$$
y' = \frac{2\ln x - \ln^2 x}{x^2} = 0
$$
$$
x = 1 \text{ 或 } e^2
$$

$x \in (0,1)$  
$y' < 0$  单调减少  

$x \in (1,e^2)$  
$y' > 0$  单调增加 
$x \in (e^2,+\infty)$  
$y' < 0$  单调减少 

极小值  当 $x = 1$, $y = 0$  
极大值  当 $x = e^2$, $y = \frac{4}{e^2}$



#### $b) \, y = x^2 (a - x)^2 \, (a > 0)$

**解：**

 $y' = 2x (a - x)^2 + 2x^2 (x - a)$
$$
= 2x (x - a)(2x - a)
$$

$x \in (-\infty, 0)$  $y' < 0$  单调减少

$x \in (0, \frac{a}{2})$  $y' > 0$  单调增加

$x \in (\frac{a}{2}, a)$  $y' < 0$  单调减少

$x \in (a, +\infty)$  $y' > 0$  单调增加

极小值  
$$
\begin{cases} 
x = 0 & y = 0 \\ 
x = a & y = 0 
\end{cases}
$$

极大值  
$$
x = \frac{a}{2} \quad y = \frac{a^4}{16}
$$



### 3. 利用极值判别法 $II$ 求下列函数的极值：
#### $a) \, y = xe^{-x}, $

**解：**

3. $a$  
$$
y = e^{-x} - xe^{-x} = (1-x)e^{-x}
$$

$$
y'' = e^{-x}(x-2)
$$

当 $x = 1$  
$y' = 0$  
$y'' = -e^{-1} < 0$

故极大值  
$x = 1$  
$y = \frac{1}{e}$



#### $b)\, y = \arctan x - \frac{1}{2} \ln (1 + x^2)$

**解：**
$$
y' = \frac{1}{1+x^2} - \frac{x}{1+x^2} = \frac{1-x}{1+x^2}
$$

$$
y'' = \frac{x^2 - 2x - 1}{(1+x^2)^2}
$$

当 $x = 1$  
$y' = 0$  
$y'' = -\frac{1}{2} < 0$

故极大值  
$x = 1$  
$y = \frac{\pi}{4} - \frac{1}{2}\ln 2$



### 4. 设函数 $y = y(x)$ 由方程 $x^2 y^2 + y = 1 \, (y > 0)$ 给出，求其极值. 

**解：**
$$
2x y^2 + x^2 \cdot 2y y' + y' = 0
$$

$$
y' = \frac{-2xy^2}{2x^2 y + 1} = 0
$$

$$
x = 0
$$

故 $y = 1$

又  
$$
y'' (2x^2 y + 1) + y' (2x^2 y + 1)' = -(2y^2 + 4xy y')
$$

$x = 0, y = 1, y' = 0$ 代入  

$$
y'' = -2 < 0
$$

故极大值  
$x = 0 \quad y = 1$

无极小值



### 5. 设 $f(x) \in C[0, +\infty]$，$f(0) = 0$，且 $f'(x)$ 单调增加，证明：$\varphi(x) = \frac{f(x)}{x}$ 在 $(0, +\infty)$ 上也是单调增加的. 

**解：**

设 $\varphi(x) = \frac{x f'(x) - f(x)}{x^2}$

在 $[0, x]$ 上，$\exists \xi \in (0, x)$

$$
f(x) - f(0) = f'(\xi)(x-0)
$$

$$
f(x) = x f'(\xi)
$$

$$
\varphi(x) = \frac{f'(\xi) - f'(x)}{x}
$$

又 $f'(x)$ 单调增加，$x > 0$。

故 $\varphi'(x) > 0$ 

成立



### 6. 求下列函数在指定区间上的最大值和最小值：
#### $  y = |4x^3 - 18x + 27| \, 在 \, [0, 2] \, 上；$

**解：**


令 $f(x) = 4x^3 - 18x + 27$  
$$
f'(x) = 12x^2 - 18 = 0
$$

$$
x = \frac{\sqrt{6}}{2}
$$

当 $x = 0$  
$f(0) = 27$  

$$
x = \frac{\sqrt{6}}{2} \quad f\left(\frac{\sqrt{6}}{2}\right) = 27 - 6\sqrt{6}
$$

$$
x = 2 \quad f(2) = 23
$$

又 $f(x)$ 在 $[0, 2]$ 上恒大于 $0$

故 $y_{\max} = 27$  

$$
y_{\min} = 27 - 6\sqrt{6}
$$



### 7. 写出 $y = \arcsin x$ 和 $y = \tan x$ 的带拉格朗日余项的三阶马克劳林公式（须有计算过程）.

**解：**

(1) $f(x) = \arcsin x$

$f(0) = 0$

$f'(x) = \frac{1}{\sqrt{1-x^2}} \quad f'(0) = 1$

$f''(x) = \frac{x}{(1-x^2)^{\frac{3}{2}}} \quad f''(0) = 0$

$f'''(x) = \frac{1}{(1-x^2)^{\frac{3}{2}}} + \frac{3x^2}{(1-x^2)^{\frac{5}{2}}} \quad f'''(0) = 1$

故 $\arcsin x = x + \frac{1}{6} x^3 + o(x^3)$

(2) $f(x) = \tan x \quad f(0) = 0$

$f'(x) = \sec^2 x \quad f'(0) = 1$

$f''(x) = 2\sec^2 x \tan x \quad f''(0) = 0$

$f'''(x) = 4\sec^2 x \tan^2 x + 2\sec^4 x \quad f'''(0) = 2$

$\tan x = x + \frac{1}{3} x^3 + o(x^3)$



### 8. 由代数基本定理知：$n$ 次多项式至多有 $n$ 个实根. 利用此结论及罗尔定理，不求函数 $f(x) = (x - 1)(x - 2)(x - 3)(x - 4)$ 的导数，说明方程 $f'(x) = 0$ 有几个实根，并指出根所在的区间. 

**解：**

$f(x) = 0$
$$
x = 1,2,3,4
$$

$f(x)$ 在 $[1,2]$, $[2,3]$, $[3,4]$ 上连续可导，且在端点处值为 $0$

故 $\exists \xi_1 \in (1,2), \xi_2 \in (2,3), \xi_3 \in (3,4)$

s.t. 
$$
f'(\xi_1) = f'(\xi_2) = f'(\xi_3) = 0
$$

$f(x)$ 为 $4$次多项式，$f'(x)$ 为 $3$ 次多项式

故 $f'(x) = 0$ 有 $3$ 个实根，分别位于 $(1,2)$, $(2,3)$, $(3,4)$



### 9. 设 $a_0, a_2, \cdots, a_{n-1}, a_n$ 都是实数，证明：若下条件满足$\frac{a_0}{n+1} + \frac{a_1}{n} + \cdots + \frac{a_{n-1}}{2} + a_n = 0$ 则 $a_0 x^n + a_1 x^{n-1} + \cdots + a_{n-1} x + a_n = 0$ 在 $(0, 1)$ 内至少有一个实根. 

**解：**

$$f(x) = \frac{a_0}{n+1} x^{n+1} + \cdots + \frac{a_{n-1}}{2} x^2 + a_n x$$ 在 $[0,1]$ 上连续可导
$$
f(0) = 0 \quad f(1) = \frac{a_0}{n+1} + \cdots + a_n = 0
$$

故 $\exists \xi \in (0,1)$  
s.t.  
$$
f'(\xi) = 0
$$

又  
$$
f'(x) = a_0 x^n + \cdots + a_n
$$

故方程在 $(0,1)$ 内至少有 $1$ 个实根 $\xi$



### 10. 设 $f(x) \in C[a,b] \cap D(a,b)$，且 $f(a)f(b) > 0$，$f(a)f\left(\frac{a+b}{2}\right) < 0$. 证明：至少存在一点 $\xi \in (a,b)$，使得 $f'(\xi) = f(\xi)$. 

**解：**

令 $F(x) = e^{-x}f(x)$

$$
F'(x) = e^{-x}\left[ f'(x) - f(x) \right]
$$

若 $f(a)f\left(\frac{a+b}{2}\right)<0$，则 $\exists x_1\in (a,\frac{a+b}{2})$ s.t. $f(x_1)=0$

若 $f(b)f\left(\frac{a+b}{2}\right)<0$，则 $\exists x_2\in (\frac{a+b}{2},b)$ s.t. $f(x_2)=0$

此时 $F(x_1) = F(x_2) = 0$

由罗尔定理，$\exists \xi \in (x_1, x_2) \subset (a,b)$ s.t. $F'(\xi) = 0$ 即 $f'(\xi) = f(\xi)$



### 11. 利用拉格朗日中值定理，证明下面的不等式：
#### a) $0 < a < b, n > 1$ 时：$na^{n-1}(b-a) < b^n - a^n < nb^{n-1}(b-a)$

**解：** 
$$
f(x) = x^n
$$

$\exists \xi \in (a, b)$ s.t. $f(b) - f(a) = f'(\xi) (b-a)$

$$
b^n - a^n = n \xi^{n-1} (b-a)
$$

所以 a^{n-1} < \xi^{n-1} < b^{n-1}$

所以  $a^{n-1} (b-a) < n \xi^{n-1} (b-a) < n b^{n-1} (b-a)$

$$
n a^{n-1} (b-a) < b^n - a^n < n b^{n-1} (b-a)
$$



#### b) $|\sin x - \sin y| \leq |x-y|$

**解：**

$f(t) = \sin t$

令 $x < y$ 且 $\xi \in (x, y)$  

$$
\sin y - \sin x = \cos \xi \cdot (y - x)
$$

$$
| \sin y - \sin x | = | \cos \xi | \cdot |y - x|
$$

又 $| \cos \xi | \leq 1$

故 $| \sin y - \sin x | \leq | y - x |$



### 12. 设 $f(x) \in C[a,b] \cap D(a,b)$ ($0 < a < b$)，证明：$\exists \xi \in (a,b)$，使得$f(b) - f(a) = \xi f'(\xi) \ln \frac{b}{a}$

**解：**  
$g(x) = \ln x$  

故 $\exists \xi \in (a, b)$  

$$
\frac{f(b) - f(a)}{g(b) - g(a)} = \frac{f'(\xi)}{g'(\xi)}
$$

即  
$$
\frac{f(b) - f(a)}{\ln b - \ln a} = \frac{f'(\xi)}{\frac{1}{\xi}}
$$

$$
f(b) - f(a) = \xi f'(\xi) \ln \frac{b}{a}
$$



### 13. 设 $f(x)$ 在 $[a,b]$ 上二阶可导，且 $f'(a) = f'(b) = 0$，证明：$\exists \xi \in (a,b)$，使得$|f''(\xi)| \geq \frac{4}{(b-a)^2} |f(b) - f(a)|$

**解：**


泰勒展开：  
$$
f(b) = f(c) + f'(c)(b-c) + \frac{1}{2} f''(\xi_1)(b-c)^2
$$
$$
= f(c) + f'(c) \cdot \frac{b-a}{2} + \frac{1}{2} f''(\xi_1) \cdot \left( \frac{b-a}{2} \right)^2
$$

$\xi_1 \in (c, b)$

$$
f(a) = f(c) + f'(c)(a-c) + \frac{1}{2} f''(\xi_2)(a-c)^2
$$
$$
= f(c) - f'(c) \cdot \frac{b-a}{2} + \frac{1}{2} f''(\xi_2) \cdot \left( \frac{b-a}{2} \right)^2
$$

$\xi_2 \in (a, c)$

两式相减：  
$$
f(b) - f(a) = f'(c)(b-a) + \frac{(b-a)^2}{8} [f''(\xi_1) - f''(\xi_2)]
$$

又由拉格朗日中值定理：  
$$
f'(b) = f'(c) + f''(\eta_1)(b-c) \quad \eta_1 \in (c, b)
$$
$$
f'(a) = f'(c) + f''(\eta_2)(a-c) \quad \eta_2 \in (a, c)
$$

结合 $f'(a) = f'(b) = 0$：  
$$
f''(\eta_2) = -f''(\eta_1)
$$

设 $M = \max_{\xi \in (a,b)} |f''(\xi)|$

由前面的推导：  
$$
|f''(\eta_1)| = |f''(\eta_2)| \leq M
$$

$$
f(b) - f(a) = f'(c)(b-a) + \frac{(b-a)^2}{8} [f''(\xi_1) - f''(\xi_2)]
$$

由于 $f'(a) = f'(b) = 0$，由罗尔定理：  
$\exists \eta_3 \in (a,b)$ s.t. $f''(\eta_3) = 0$

考虑：  
$$
\frac{(b-a)^2}{2} |f''(\eta_3)| = \left| [f(b) - f(a)] - \frac{(b-a)^2}{8} [f''(\xi_1) - f''(\xi_2)] \right|
$$

$$
\frac{(b-a)^2}{2} |f''(\eta_3)| \leq |f(b) - f(a)| + \frac{(b-a)^2}{8} |f''(\xi_1) - f''(\xi_2)|
$$

假设 $|f''(\xi)| < \frac{4}{(b-a)^2} |f(b) - f(a)|$ 不成立  

则存在 $\xi \in (a,b)$ 使得 $|f''(\xi)| \geq \frac{4}{(b-a)^2} |f(b) - f(a)|$

结合前面的不等式：  
$$
\frac{(b-a)^2}{2} \cdot \frac{4}{(b-a)^2} |f(b) - f(a)| \leq |f(b) - f(a)| + \frac{(b-a)^2}{8} \cdot 2M
$$

简化得：  
$$
2|f(b) - f(a)| \leq |f(b) - f(a)| + \frac{(b-a)^2}{4} M
$$

$$
|f(b) - f(a)| \leq \frac{(b-a)^2}{4} M
$$

矛盾，故假设不成立
即存在 $\xi \in (a,b)$，使得  
$$
|f''(\xi)| \geq \frac{4}{(b-a)^2} |f(b) - f(a)|
$$


### 14. 设 $f(x)$ 在 $[0,1]$ 上二次可微，且 $f(0) = f(1) = 0$，证明：$\exists \xi \in (0,1)$，使得$ 2f'(\xi) + \xi f''(\xi) = 0$

**解：**

令 $g(x) = x f(x)$

$f(0) = f(1) = 0$，故由罗尔定理，$\exists c \in (0,1)$ s.t. $f'(c) = 0$

$g(0) = 0 \cdot f(0) = 0$，$g(c) = c \cdot f(c)$，但 $f(c)$ 不一定为 $0$

重新考虑：令 $g(x) = x^2 f'(x)$

$g(0) = 0^2 \cdot f'(0) = 0$  
由 $f'(c) = 0$，得 $g(c) = c^2 \cdot f'(c) = 0$

故 $g(0) = g(c) = 0$，由罗尔定理，$\exists \xi \in (0,c) \subset (0,1)$ s.t. $g'(\xi) = 0$

$$
g'(\xi) = 2\xi f'(\xi) + \xi^2 f''(\xi) = 0
$$

又 $\xi \neq 0$，故  
$$
2f'(\xi) + \xi f''(\xi) = 0
$$


### 15. 设 $f(x) \in C[a,b] \cap D(a,b)$，且 $f(a) = f(b) = 1$，求证：$\exists \xi, \eta \in (a,b)$，使得$e^{\eta - \xi} [f(\eta) + f'(\eta)] = 1$

**解：**

![Capture_20251210_232952](D:\Huawei Share\Huawei Share\Capture_20251210_232952.jpg)

### 16. 求下列函数图形的凹（下凸）凸区间及拐点：

#### a) $y = x^4 - 12x^3 + 48x^2 - 50;$

**解：**
$$
y' = 4x^3 - 36x^2 + 96x
$$

$$
y' = 4x(x-2)(x-4)
$$

$$
y'' = 12x^2 - 72x + 96 = 12(x-2)(x-4)
$$

$x \in (-\infty, 2)$  $y'' > 0$  凹

$x \in (2, 4)$  $y'' < 0$  凸

$x \in (4, +\infty)$  $y'' > 0$  凹

拐点：  
$x = 2$  $y = 62$  
$x = 4$  $y = 206$ 

拐点 $(2, 62)$，$(4, 206)$



#### b) $y = a^2 - \sqrt[3]{x-b}$

**解：**
$$
y' = -\frac{2}{3}(x-b)^{-1/3}
$$

$$
y'' = \frac{2}{9}(x-b)^{-4/3}
$$

$x \in (-\infty, b)$  $y'' < 0$  凸

$x \in (b, +\infty)$  $y'' > 0$  凸

拐点 $(b, a^2)$



### 17. 证明：曲线 $y = \frac{x+1}{x^2+1}$ 有三个拐点且位于同一条直线上. 

**解：**
$$
y'' = \frac{1 - 2x - x^2}{(x^2 + 1)^2}
$$
$$
y''' = \frac{4x^3 + 8x^2 - 6x - 2}{(x^2 + 1)^3}
$$
令 $y''' = 0$ 得：
$$
2x^3 + 4x^2 - 3x - 1 = 0
$$

设拐点处的切线方程为 $y = kx + m$

在拐点处有：
$$
\frac{x + 1}{x^2 + 1} = kx + m
$$

整理得：
$$
kx^3 + mx^2 + (k-1)x + (m-1) = 0
$$

又拐点满足：
$$
2x^3 + 4x^2 - 3x - 1 = 0
$$

由于两个方程同解，对应系数成比例：
$$
\frac{k}{2} = \frac{m}{4} = \frac{k-1}{-3} = \frac{m-1}{-1}
$$

解得：
$$
k = \frac{2}{5}, \quad m = \frac{4}{5}
$$

故三个拐点均在直线 $y = \frac{2}{5}x + \frac{4}{5}$ 上



### 18. 证明下列不等式：

#### (a) 设常数 $p > 1$，则当 $x \in [0,1]$ 时，有 $x^p + (1-x)^p \geq \frac{1}{2^{p-1}}$. 

**解：**

18.  
$(a)$ $f(x) = x^p + (1-x)^p$  
$$
f'(x) = p x^{p-1} - p(1-x)^{p-1} = 0
$$

$$
x^{p-1} = (1-x)^{p-1} \quad \Rightarrow \quad x = \frac{1}{2}
$$

$$
f''(x) = p(p-1)x^{p-2} + p(p-1)(1-x)^{p-2}
$$

在 $(0,1)$ 内，$p>1$ 时  
$$
f''(x) > 0
$$
故  
$$
f\left(\frac{1}{2}\right) = \frac{1}{2^{p-1}}
$$
为极小值，故  
$$
f(x) = x^p + (1-x)^p \geq \frac{1}{2^{p-1}}
$$



#### (b) $\frac{e^x + e^y}{2} > e^{\frac{x+y}{2}}$ ($x \neq y$)

**解：**

 $f(t) = e^t$  
$$
f'(t) = e^t \quad f''(t) = e^t > 0
$$
为凸函数  

由凸函数性质：  
$$
\frac{f(x) + f(y)}{2} \geq f\left(\frac{x+y}{2}\right) \quad (x \neq y)
$$
故  
$$
\frac{e^x + e^y}{2} > e^{\frac{x+y}{2}} \quad (x \neq y)
$$




### 19. 全面讨论下列函数的性态，并描绘出它们的图像：

#### $a) \ y = \frac{2x^2}{(1-x)^2}; $

**解：**


 定义域 $x \neq 1$  

渐近线：$x = 1$（垂直渐近线）  
水平渐近线：$\lim\limits_{x \to \infty} y = 2$，故 $y = 2$ 为水平渐近线  

单调性：$y' = \frac{4x}{(1-x)^3}$  
$x \in (-\infty, 0)$：$y' < 0$，单调递减  
$x \in (0, 1)$：$y' > 0$，单调递增  
$x \in (1, +\infty)$：$y' < 0$，单调递减  

极值：$x = 0$ 时，$y' = 0$，$y = 0$ 为极小值  

凹凸性：$y'' = \frac{4(1+x)}{(1-x)^2}$  
$x \in (-\infty, -1)$：$y'' < 0$，凹  
$x \in (-1, 1)$：$y'' > 0$，凸  
$x \in (1, +\infty)$：$y'' > 0$，凸  

图像特征：过原点，且在原点取得极小值  
在 $x=1$ 处向 $+\infty$ 发散，左侧先凹后凸，右侧始终凸  
当 $x \to -\infty$ 时趋向 $y = 2$，当 $x \to +\infty$ 时趋向 $y = 2$



#### $b) \ y = x \ln \left( e + \frac{1}{x} \right)$

**解：**

定义域 $x \in (-\infty, -\frac{1}{e}) \cup (0, +\infty)$  

单调性 $y' = \ln(e^{-\frac{1}{e}}) - \frac{1}{e^{-\frac{1}{e+1}}}$，故单调增加  

渐近线 $y = x$  

图像：整件呈一条单调递增曲线，由两支构成，中间在 $x \in (-\frac{1}{e}, 0)$ 区间缺失  
左支自 $x = -\infty$ 向右上升，趋近直线 $y = x$，在 $x = -\frac{1}{e}$ 附近趋向 $0$  
右支从 $x = 0^+$ 附近的 $0$ 开始上升，最终在 $x \to +\infty$ 时近似直线 $y = x$



### 20. 证明方程 $x^5 + 5x + 1 = 0$ 在区间 $(-1, 0)$ 内有唯一的实根，并用切线法求这个根的近似值，使误差不超过 0.01. 

**解：**

![Capture_20251210_233035](D:\Huawei Share\Huawei Share\Capture_20251210_233035.jpg)



### 21. 求方程 $\sin 2x - x = 0$ 的正实根（精确到两位小数）. 

**解：**

![Capture_20251210_233047](D:\Huawei Share\Huawei Share\Capture_20251210_233047.jpg)



## 选做题：

### 1. 证明广义罗尔定理：设 $f(x) \in D(a, b)$，且 $\lim_{x \to a^+} f(x) = \lim_{x \to a^-} f(x) = +\infty$ (或 $-\infty$)，则 $\exists \xi \in (a, b)$，使得 $f'(\xi) = 0$. 

**解：**





### 2. 设 $f(x) \in D[0, +\infty)$，且 $\forall x \in (0, +\infty)$，成立 $0 \leq f(x) \leq \ln \frac{2x+1}{x+\sqrt{1+x^2}}$. 证明：$\exists \xi \in (0, +\infty)$，使得$f'(\xi) = \frac{2}{2\xi + 1} - \frac{1}{\sqrt{1+\xi^2}}$

#### 提示：利用推广的罗尔定理，见课本 157 页例 4.5. 

**解：**





### 3. 设函数 $f(x)$ 在 $x = a$ 的某领域内 $n (\geq 3)$ 阶可导，且 $f^{(n)}(x)$ 在 $x = a$ 连续，又假设 $f''(a) = \cdots = f^{(n-1)}(a) = 0$，$f^{(n)}(a) \neq 0$，且 $f(a + h) = f(a) + hf'(a + \theta h) \quad 0 < \theta < 1$，证明：$\lim_{h \to 0} \theta = \left( \frac{1}{h} \right)^{\frac{1}{n-1}}$

**解：**





### 4. 设函数 $f(x)$ 在区间 $[0, +\infty)$ 上二阶可导，且 $f''(x) < 0$. 若 $f(0) > 0$，$f'(0) < 0$，证明：$f(x) = 0$ 在区间 $[0, +\infty)$ 上有解. 

**解：**





### 5. 设函数 $f(x)$ 在闭区间 $[0, 1]$ 上二阶可导，且满足 $f(0) = f(1) = 0$，$\max_{0 \leq x \leq 1} f(x) = 2$，证明：存在 $\xi \in (0, 1)$，使得 $f''(\xi) \leq -16$. 

**解：**





### 6. 设 $f(x)$ 在 $[a, b]$ 上三阶可导，证明：存在 $\xi \in (a, b)$，使得$f(b) = f(a) + f'\left( \frac{a+b}{2} \right)(b-a) + \frac{1}{24}(b-a)^3 f'''(\xi)$

**解：**





### 7. 设 $f(x)$ 在 $x = 0$ 的某领域内具有 $n$ 阶导数，且 $f(0) = f'(0) = \cdots = f^{(n-1)}(0) = 0$，利用柯西中值定理，证明$\frac{f(x)}{x^n} = \frac{f^{(n)}(\theta x)}{n!} \quad 0 < \theta < 1$

**解：**



