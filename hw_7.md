# <center>hw_7<center>

## 必做题
### 1. 利用微分计算下列近似值：

#### a) $\sqrt[3]{9}$;  

**解：**
$$
f(x) = x^{\frac{1}{3}}
$$
$$
f'(x) = \frac{1}{3}x^{-\frac{2}{3}}
$$
$$
\sqrt[3]{9} \approx f(8) + f'(8) \cdot 1 = 2 + \frac{1}{12} = \frac{25}{12}
$$


#### b) $\arctan 1.04$;

**解：**
$$
f(x) = \arctan x
$$
$$
f'(x) = \frac{1}{1+x^2}
$$
$$
\arctan 1.04 \approx \frac{\pi}{4} + \frac{1}{2} \times 0.04 = \frac{\pi}{4} + 0.02
$$


#### c) $\lg 11$

**解：**
$$
f(x) = \lg x
$$
$$
f'(x) = \frac{1}{x \ln 10}
$$
$$
\lg 11 \approx 1 + \frac{1}{10 \ln 10}
$$



### 2. 已知单摆的周期 $T = 2\pi \sqrt{\frac{l}{g}}$，其中 $g = 980\text{cm/s}^2$，$l$ 为摆长（单位：cm），且原摆长为 20cm，为使周期 $T$ 增大 0.05s，摆长约需增长多少？

**解：**2. 
$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

$$
\frac{dT}{dL} = \frac{\pi}{\sqrt{gL}}
$$

$$
\Delta L \approx \Delta T \cdot \frac{\sqrt{gL}}{\pi} = 0.05 \cdot \frac{\sqrt{980 \times 20}}{\pi} \approx \frac{7}{\pi} \text{ cm}
$$





### 3. 利用一阶微分的形式不变性，计算下列函数的导数 $\frac{dy}{dx}$，其中 $u, v$ 都是 $x$ 的函数。

#### a) $y = \ln \sqrt{u^2 + v^2}$;

**解：**
$$
dy = \frac{1}{2} \cdot \frac{2u du + 2v dv}{u^2 + v^2} = \frac{u du + v dv}{u^2 + v^2}
$$

$$
\frac{dy}{dx} = \frac{u \frac{du}{dx} + v \frac{dv}{dx}}{u^2 + v^2}
$$


#### b) $y = \arctan \frac{v}{u}$

**解：**
$$
y = \arctan \frac{v}{u}
$$

$$
dy = \frac{1}{1 + \left(\frac{v}{u}\right)^2} d\left(\frac{v}{u}\right) = \frac{u^2}{u^2 + v^2} \cdot \frac{u dv - v du}{u^2} = \frac{u dv - v du}{u^2 + v^2}
$$

$$
\frac{dy}{dx} = \frac{u \frac{dv}{dx} - v \frac{du}{dx}}{u^2 + v^2}
$$



### 4. 计算下面的微商，并用复合函数求导的链式法则加以解释：
#### a) $\frac{d(x^3 - 2x^6 - x^9)}{d(x^3)}$;  

**解：**令 $z = x^3$
$$
y = z - 2z^2 - z^3
$$

$$
\frac{dy}{dz} = 1 - 4z - 3z^2
$$

原式 $= 1 - 4x^3 - 3x^6$





#### b) $\frac{d\arcsin x}{d\arccos x}$

**解：**原式 $= \frac{d(\arcsin x)}{dx} \cdot \frac{dx}{d(\arccos x)} = \frac{\frac{1}{\sqrt{1-x^2}}}{-\frac{1}{\sqrt{1-x^2}}} = -1$




### 5. 求下列极限（可用洛必达法则，无穷小替换或泰勒展开。）
#### a) $\lim_{x \to \infty} \frac{x^2 \sin \frac{1}{x}}{2x - 1}$;

**解：**原式 $= \lim_{x \to \infty} \frac{x^2 \cdot \frac{1}{x}}{2x - 1} = \frac{1}{2}$



#### b) $\lim_{x \to 0} \frac{x \cos x - \sin x}{x^3}$

**解：**原式 $= \lim_{x \to 0} \frac{x(1 - \frac{x^2}{2} + o(x^2)) - (x - \frac{x^3}{6} + o(x^3))}{x^3} = -\frac{1}{3}$



#### c) $\lim_{x \to 0} \frac{x - \arctan x}{\tan x - x}$;

**解：**原式 $= \lim_{x \to 0} \frac{x - (x - \frac{x^3}{3} + o(x^3))}{\tan x - x} = \lim_{x \to 0} \frac{\frac{x^3}{3} + o(x^3)}{x + \frac{x^3}{3} + o(x^3) - x} = 1$



#### d) $\lim_{x \to 0} \frac{\ln (1 + x + x^2) + \ln (1 - x + x^2)}{\sec x - \cos x}$

**解：**原式 $= \lim_{x \to 0} \frac{(x + x^2 - \frac{x^2}{2} + o(x^2)) + (-x + x^2 - \frac{x^2}{2} + o(x^2))}{\sec x - \cos x} = \lim_{x \to 0} \frac{x^2 + o(x^2)}{x^2} = 1$



#### e) $\lim_{x \to 0} \left( \frac{1}{x} - \frac{1}{e^x - 1} \right)$;

**解：**原式 $= \lim_{x \to 0} \left( \frac{1}{x} - \frac{1}{x + \frac{x^2}{2} + o(x^2)} \right) = \frac{1}{2}$



#### f) $\lim_{x \to 1^-} \ln x \cdot \ln (1 - x)$

**解：**令 $t = 1 - x$

原式  
$$
\lim_{t \to 0^+} \ln (1-t) \ln t = \lim_{t \to 0^+} (-t) \ln t = 0
$$




#### g) $\lim_{x \to \frac{\pi}{4}} (\tan x)^{\tan 2x}$;

**解：**
令 $u = x - \frac{\pi}{4}$

原式  
$$
\lim_{x \to \frac{\pi}{4}} e^{\tan 2x \ln (\tan x)}
$$
$$
= \lim_{u \to 0} e^{\frac{1}{2u} \ln (1+2u)}
$$
$$
= e^{-1} = \frac{1}{e}
$$



#### h) $\lim_{x \to 0^+} x^{\frac{1}{\ln (e^{x-1})}}$

**解：**
原式  
$$
= \lim_{x \to 0^+} x^{\frac{1}{x-1}}
$$
$$
= \lim_{x \to 0^+} e^{\frac{\ln x}{x-1}}
$$
$$
= +\infin
$$



### 6. 确定常数 $a, b$ 使得

$f(x) =
\begin{cases} 
\frac{\sin x}{x}, & x > 0 \\ 
ax^2 + bx + 1, & x \leq 0 
\end{cases}$ 二阶可导，并求 $f''(x)$。

**解：**
$$
\lim_{x \to 0^+} \frac{\sin x}{x} = 1 \quad \Rightarrow \quad f(0) = 1
$$

由连续性：$f(0^+) = f(0^-) \Rightarrow 1 = 1$，成立

一阶导数连续：
$$
\lim_{x \to 0^+} \frac{\frac{\sin x}{x} - 1}{x} = \lim_{x \to 0^+} \frac{\sin x - x}{x^2} = 0
$$
$$
\lim_{x \to 0^-} \frac{ax^2 + bx + 1 - 1}{x} = b = 0
$$

二阶导数连续：
$$
\frac{\sin x}{x} = 1 - \frac{x^2}{6} + o(x^2)
$$
$$
\lim_{x \to 0^+} \frac{\frac{\sin x}{x} - 1}{x^2} = -\frac{1}{6}
$$
$$
\lim_{x \to 0^-} \frac{ax^2 - 0}{x^2} = a = -\frac{1}{6}
$$

故 $a = -\frac{1}{6}, b = 0$

$$
f''(x) = 
\begin{cases} 
\frac{-x^2\sin x - 2x\cos x + 2\sin x}{x^3}, & x > 0 \\
-\frac{1}{3}, & x \leq 0 
\end{cases}
$$




### 7. 讨论函数 

$f(x) = \begin{cases}
\left[ \frac{(1+x)^{\frac{1}{x}}}{e} \right]^{\frac{1}{x}}, & x > 0 \\ 
e^{-\frac{1}{2}}, & x \leq 0 
\end{cases}$ 在点 $x = 0$ 处的连续性。

**解：** $x \to 0^+$
$$
f(x) = \left[ \frac{(1+x)^{\frac{1}{x}}}{e} \right]^{\frac{1}{x}} = e^{\frac{1}{x} \ln \frac{(1+x)^{\frac{1}{x}}}{e}} = e^{\frac{1}{x} \left( \frac{\ln (1+x)}{x} - 1 \right)}
$$

$$
\ln (1+x) = x - \frac{x^2}{2} + \frac{x^3}{3} + o(x^3)
$$

$$
\frac{\ln (1+x)}{x} - 1 = -\frac{x}{2} + \frac{x^2}{3} + o(x^2)
$$

$$
\frac{1}{x} \left( \frac{\ln (1+x)}{x} - 1 \right) = -\frac{1}{2} + \frac{x}{3} + o(x)
$$

$$
\lim_{x \to 0^+} f(x) = e^{-\frac{1}{2}} = f(0)
$$

故连续



### 8. 设函数 $f(x)$ 在 $x = 0$ 的某领域内二阶可导，且 $\lim_{x \to 0} \frac{\sin x + xf(x)}{x^3} = 0$，求 $f(0), f'(0), f''(0)$。

**解：**
$$
f(x) = f(0) + f'(0)x + \frac{1}{2}f''(0)x^2 + o(x^2)
$$

$$
\sin x + x f(x) = \left(x - \frac{x^3}{6}\right) + x\left(f(0) + f'(0)x + \frac{1}{2}f''(0)x^2\right) + o(x^3)
$$


$f(0) =-1$

$ f'(0) = 0$

$ f''(0) = \frac{1}{3}$






### 9. 求下列方程所确定的隐函数 $y = y(x)$ 的导数 $\frac{dy}{dx}$：
#### a) $e^{2x+y} - \cos (xy) = e - 1$;

**解：**对 $e^{2x+y} - \cos(xy) = e - 1$ 两边求导：
$$
e^{2x+y}(2 + y') + \sin(xy)(y + xy') = 0
$$

$$
y'(e^{2x+y} + x\sin(xy)) = -2e^{2x+y} - y\sin(xy)
$$

$$
y' = -\frac{2e^{2x+y} + y\sin(xy)}{e^{2x+y} + x\sin(xy)}
$$





#### b) $y \sin x - \cos (x - y) = 0$

**解：**对 $y\sin x - \cos(x-y) = 0$ 两边求导：
$$
y'\sin x + y\cos x + \sin(x-y)(1 - y') = 0
$$

$$
y'(\sin x - \sin(x-y)) + y\cos x + \sin(x-y) = 0
$$

$$
y' = -\frac{y\cos x + \sin(x-y)}{\sin x - \sin(x-y)}
$$



### 10. 求曲线 $x^3 + y^3 - 3xy = 0$ 在点 $(\sqrt[3]{2}, \sqrt[3]{4})$ 处的切线方程和法线方程。

**解：** 
对 $x^3 + y^3 - 3xy = 0$ 两边求导：
$$
3x^2 + 3y^2 y' - 3y - 3xy' = 0
$$

$$
y'(3y^2 - 3x) = 3y - 3x^2
$$

$$
y' = \frac{y - x^2}{y^2 - x}
$$

在点 $(\sqrt[3]{2}, \sqrt[3]{4})$ 处：
$$
y' = \frac{\sqrt[3]{4} - (\sqrt[3]{2})^2}{(\sqrt[3]{4})^2 - \sqrt[3]{2}} = \frac{\sqrt[3]{4} - \sqrt[3]{4}}{\sqrt[3]{16} - \sqrt[3]{2}} = 0
$$

切线方程：
$$
y - \sqrt[3]{4} = 0
$$

法线方程：
$$
x = \sqrt[3]{2}
$$





### 11. 求下列方程所确定隐函数 $y = y(x)$ 的二阶导数 $\frac{d^2y}{dx^2}$：

#### a) $e^{x+y} = xy$;

**解：**
$$
|| \cdot (a)
$$

$$
e^{x+y} (1+y) = y + xy
$$

$$
y' = \frac{y - e^{x+y}}{e^{x+y} - x}
$$

$$
y'' = \frac{\left( \frac{y - e^{x+y}(1+y)}{e^{x+y} - x} \right) \left( e^{x+y} - x \right) - \left( \frac{y - e^{x+y}(1+y)}{e^{x+y} - x} \right) \left( e^{x+y} (1+y) - 1 \right)}{\left( e^{x+y} - x \right)^2}
$$



#### b) $\arctan \frac{x}{y} = \ln \sqrt{x^2 + y^2}$

**解：**
$$
\frac{y - x y}{x^2 + y^2} = \frac{x + y y^2}{x^2 + y^2}
$$

$$
y' = \frac{y - x}{x + y}
$$

$$
y'' = \frac{(y' - 1)(x + y) - (y - x)(1 + y')}{(x + y)^2}
$$

$y'$带入



### 12. 求下列参数方程所确定函数的一阶导数 $\frac{dy}{dx}$ 和二阶导数 $\frac{d^2y}{dx^2}$：
#### a) $\begin{cases} x = a \cos^3 t \\ y = a \sin^3 t \end{cases}$;

**解：**

$$
\frac{dy}{dx} = \frac{-3a\cos^2 t \sin t}{3a \sin^2 t \cos t} = - \tan t
$$

$$
\frac{d^2 y}{dx^2} = \frac{1}{3a \cos^4 t \sin t}
$$



#### b) $\begin{cases} x = t - \ln (1 + t^2) \\ y = \arctan t \end{cases}$;

**解：**
$$
\frac{dy}{dx} = \frac{1 - \frac{2t}{1 + t^2}}{\frac{1}{1 + t^2}} = \frac{1}{(t - 1)^2}
$$

$$
\frac{d^2 y}{dx^2} = -\frac{2(1 + t^2)}{(t - 1)^5}
$$





#### c) $\begin{cases} x = f'(t) \\ y = tf'(t) - f(t) \end{cases}$

**解：**
$$
\frac{dy}{dx} = \frac{f'(t)}{tf(t)} = t
$$

$$
\frac{d^2 y}{dx^2} = \frac{1}{f''(t)}
$$



### 13. 求下列参数方程表示的曲线在给定处的切线方程和法线方程：

#### a) $\begin{cases} x = a(\cos t + t \sin t) \\ y = a(\sin t - t \cos t) \end{cases}$, $t = \frac{\pi}{4}$;

**解：**
$$
\frac{dy}{dx} = \frac{at\ sint}{a t\ cost} = tan t
$$

$$
x_0 = a \cdot \frac{\sqrt{2}}{2}(1+\frac{\pi}{4}) \quad y_0 = a \cdot \frac{\sqrt{2}}{2}(1-\frac{\pi}{4})
$$

切: $y - y_0 = (x-x_0)$

法: $y - y_0 = -(x-x_0)$



#### b) $\begin{cases} x = 2e^t \\ y = e^{-t} \end{cases}$, $t = 0$

**解：**
$$
\frac{dy}{dx} = -\frac{e^{-t}}{2e^t}
$$

切: $y-1 = -\frac{1}{2}(x-2)$

法: $y-1 = 2(x-2)$



### 14. 验证 $y = e^t \cos t$, $x = e^t \sin t$ 所确定的函数 $y = y(x)$ 满足微分方程

$$
y''(x + y)^2 = 2(xy' - y)
$$
**解：**
$$
y' = \frac{dy}{dx} = \frac{e^t (\cos t - \sin t)}{e^t (\sin t + \cos t)} = \frac{\cos t - \sin t}{\sin t + \cos t}
$$

$$
y' = \frac{u}{v}
$$

$$
y'' = \frac{d}{d\lambda}(y') = \frac{dy'}{dt} \cdot \frac{dt}{dx} = -\frac{2}{e^t v^3}
$$

代入，左边=右边



### 15. 设 $y = y(x)$ 是由 $\begin{cases} x = t^2 - 2t - 3 \\ e^y \sin t - y + 1 = 0 \end{cases}$ 所确定的函数，求 $\frac{dy}{dx}$ 及 $\frac{dy}{dx}|_{t=0}$。

**解：**
$$
\frac{dy}{dx} = \frac{-e^y \cos t}{(e^y \sin t - 1)(2t - 2)}
$$

$$
\frac{dy}{dx} |_{t=0} = -\frac{e}{2}
$$



### 16. 求下列极坐标方程表示的曲线在指定点处的切线和法线方程：

#### a) $r = \cos \theta + \sin \theta$, $\theta = \frac{\pi}{4}$;

**解：**
$$
 r = r(\theta)
$$

$$
\frac{dy}{dx} = \frac{r'(\theta) \sin \theta + r \cos \theta}{r(\theta) \sin \theta - r \sin \theta}
$$

$$
\frac{dy}{dx} = -\frac{1}{\tan \theta} \left| \frac{\pi}{4} \right. = -1
$$

$$
y = -x + 2
$$




#### b) $r = a \sin 2\theta (a > 0)$, $\theta = \frac{\pi}{4}$

**解：**
$$
\frac{dy}{dx} = -1
$$

$$
y - \frac{a\sqrt{2}}{2} = -(x - \frac{a\sqrt{2}}{2})
$$





### 17. 写出下列函数在指定点的泰勒公式

#### (a) $f(x) = x^3 - 2x^2 + 3x - 4$ 在点 $x_0 = -2$ 处；(可不用求导计算)

**解：**
$$
f(x) = -26 + 23(x+2) - 8(x+2)^2 + (x+2)^3
$$



#### (b) $f(x) = \frac{1}{x}$ 在点 $x_0 = -1$ 处的 $n$ 阶泰勒公式；

**解：**
$$
T_h(x) = -\sum_{k=0}^n (x+1)^k
$$



#### (c) $f(x) = x^2 \ln x$ 在点 $x_0 = 1$ 处的 $n$ 阶泰勒公式；

**解：**
$$
T_h(x) = \sum_{k=1}^n (-1)^{k-1} \frac{(x-1)^k}{k} + 2 \sum_{k=1}^{n-1} (-1)^{k-1} \frac{(x-1)^{k-1}}{k} + \sum_{k=1}^{n-2} (-1)^{k-1} \frac{(x-1)^{k-2}}{k}
$$





#### (d) $f(x) = \sqrt{x}$ 在点 $x_0 = 4$ 处的 $n$ 阶泰勒公式

**解：**

$$
T_h(x) = 2 \sum_{k=0}^n \binom{ \frac{1}{2}}{k}   \left( \frac{x-4}{4} \right)^k
$$



### 18. 利用泰勒公式求 $\sqrt[3]{30}$ 和 $\ln 1.2$ 的近似值（精确到 0.001）

**解：**

$(a)$ 原式 = $3 + \frac{1}{27} \cdot 3$ $\approx$ 3.107  

$(b)$ 原式 = $0.2 - \frac{0.2^3}{2} + \frac{0.2^3}{3} - \cdots \approx 0.1823$



### 19. 利用泰勒公式求下列极限：

#### (a) $\lim_{x \to 0} \frac{e^x \sin x - x(1 + x)}{x^3}$;

**解：**

原式 = 
$$
\lim_{x \to 0} \frac{x + x^2 + \frac{x^3}{3} + o(x^3) - x - x^2}{x^3}
$$
$$
= \frac{1}{3}
$$







#### (b) $\lim_{x \to \infty} \left[ x - x^2 \ln \left( 1 + \frac{1}{x} \right) \right]$;

**解：**
原式 = 
$$
\lim_{x \to \infty} \left[ x - x + \frac{1}{2} - o(1) \right]
$$
$$
= \frac{1}{2}
$$



#### (c) $\lim_{x \to +\infty} \left( \sqrt[5]{x^5 + x^4} - \sqrt[5]{x^5 - x^4} \right)$

**解：** 
原式 = 
$$
\lim_{x \to +\infty}x \left[ (1 + \frac{1}{x})^{\frac{1}{5}} - (1 - \frac{1}{x})^{\frac{1}{5}} \right]
$$
$$
= \frac{2}{5}
$$



### 20. 求极限：

#### a) $\lim_{x \to +\infty} \left[ \ln (1 + 2^x) \ln \left( 1 + \frac{3}{x} \right) \right]$;

**解：**
$$
\quad 原式 = \lim_{x \to +\infty} x \ln2 \cdot \frac{3}{x}
$$

$$
= 3 \ln2
$$



#### b) $\lim_{x \to 0} \left( \frac{3^{x+1} - 2^{x+1}}{x+1} \right)^{\frac{1}{x}}$

**解：**
$$
\quad 原式 = \lim_{x \to 0} \left[ 1 + x (3 \ln3 - 2\ln2 - 1) + o(x) \right]^{\frac{1}{x}}
$$

$$
= e^{3 \ln3 - 2\ln2 - 1} = \frac{27}{4e}
$$





## 选做题：

### 1. 如下图所示的电缆 $AOB$ 的长度为 $s$，跨度为 $2L$。电缆的最低点 $O$ 与杆顶连线 $AB$ 的距离为 $f$，则电缆长可按下列公式计算
$$
s = 2L \left( 1 + \frac{2f^2}{3L^2} \right)
$$
<img src="C:\Users\ss\AppData\Roaming\Typora\typora-user-images\image-20251123210045992.png" alt="image-20251123210045992" style="zoom:50%;" />

当 $f$ 变化了 $\Delta f$ 时，电缆长的变化约为多少？

**解：**
$$
S = 2L \left( 1 + \frac{2f^2}{2L^2} \right)
$$

$$
ds = \frac{8f}{3L} df
$$

$$
\Delta s \approx \frac{8f}{3L} \Delta f
$$



### 2. 求证：星型线 $x^{\frac{2}{3}} + y^{\frac{2}{3}} = a^{\frac{2}{3}}$ ($a > 0$) 在两坐标轴间的切线长度为常数

**解：**

2. $\frac{2}{3} \cdot x^{-\frac{1}{3}} + \frac{2}{3} y^{-\frac{1}{3}} = 0$  
$$
y' = (-\frac{x}{y})
$$
$$
y - y_0 = -(\frac{x_0}{y_0})^{\frac{1}{3}}(x - x_0)
$$

令 $y = 0$  
$$
x = x_0 + \frac{y_0^{\frac{1}{3}}}{x_0^{\frac{1}{3}}}
$$

令 $x = 0$  
$$
y = y_0 + \frac{x_0^{\frac{1}{3}}}{y_0^{\frac{1}{3}}}
$$

$$
l = \sqrt{x^2 + y^2} = (x_0^{\frac{4}{3}} + y_0^{\frac{4}{3}}) \frac{\sqrt{x_0^{\frac{2}{3}} + y_0^{\frac{2}{3}}}}{(x_0 y_0)^{\frac{1}{3}}}
$$

$$
= (x_0^{\frac{4}{3}} + y_0^{\frac{4}{3}}) \frac{a^{\frac{1}{3}}}{(x_0 y_0)^{\frac{1}{3}}}
$$

$$
= (\frac{a}{x_0 y_0})^{\frac{1}{3}} \left( a^{\frac{4}{3}} - (x_0 y_0)^{\frac{2}{3}} \right)
$$

$$
x_0^{\frac{2}{3}} + y_0^{\frac{2}{3}} = a^{\frac{2}{3}}
$$

$$
a^{\frac{4}{3}} - (x_0 y_0)^{\frac{2}{3}} = a^{\frac{4}{3}} \left( 1 - \frac{(x_0 y_0)^{\frac{2}{3}}}{a^{\frac{4}{3}}} \right)
$$

故 $l = a^{\frac{1}{3}} \cdot a^{\frac{2}{3}} = a$



### 3. 当 $x \to +\infty$ 时，$\frac{\pi}{2} - \arctan x$ 和 $\frac{1}{x}$ 是否为等价无穷小？证明你的结论

**解：**为等价无穷，  
$$
\arctan x + \arctan\frac{1}{x} = \frac{\pi}{2}
$$
$$
\frac{\pi}{2} - \arctan x = \arctan\frac{1}{x} \sim \frac{1}{x}
$$
为等价无穷



### 4. 设函数 $y = y(x)$ 由方程 $xe^{f(y)} = Ce^y$ 确定（其中 $C$ 为非零常数），设 $f$ 具有二阶导数，且 $f'(y) \neq 1$，求 $\frac{dy}{dx}, \frac{d^2y}{dx^2}$

**解：**
$$
e^{f(y)} + x e^{f(y)} f'_{(y)} \frac{dy}{dx} = Ce^{y} \frac{dy}{dx}
$$

$$
e^{f(y)} + x e^{f(y)} f'_{(y)} y' = x e^{f(y)} y'
$$

$$
e^{f(y)} = x e^{f(y)}(1-f'_{(y)}) y'
$$

$$
\frac{dy}{dx} = \frac{1}{x (1-f'_{(y)})}
$$

$$
\frac{d^2 y}{dx^2} = \frac{f''(y) - (1-f'_{(y)})^2}{x^2 (1-f'_{(y)})^3}
$$



### 5. 设 $f(x) = (a + b \cos x) \sin x - x$ 在 $x \to 0$ 时是 $x$ 的五阶无穷小，求常数 $a$ 和 $b$

**解：**

$$
f(x) = (a+b-1)x - \frac{a+b}{6}x^3 - \frac{b}{2}x^3 + O(x^5)
$$

$$
= (a+b-1)x - \frac{a+b}{6}x^3 + O(x^5)
$$

$$
\begin{cases} 
a+b-1 = 0 \\ 
a+4b = 0 \\ 
\end{cases}
$$

$$
a = \frac{4}{3} 
b = -\frac{1}{3}
$$



### 6. 设函数 $f(x)$ 满足 $f(0) = 0$，且 $f'(0)$ 存在，证明：$\lim_{x \to 0^+} x^{f(x)} = 1$

**解：**
$$
\lim_{x \to 0^+} x^{f(x)}
$$

$$
= \lim_{x \to 0^+} e^{f(x)/hx}
$$

$$
= \lim_{x \to 0^+} e^{(f'(0)x + o(x))/hx}
$$

$$
= \lim_{x \to 0^+} e^0 = 1
$$




### 7. 计算下面极限
#### a) $\lim_{x \to 0} \frac{\sin(e^x - 1) - (e^{\sin x} - 1)}{\sin^4 3x}$  

**解：**
原式 = 
$$
\lim_{x \to 0} \frac{-\frac{x^4}{12} + o(x^5)}{(3x)^4 + o(x^6)}
$$
$$
= -\frac{1}{972} 
$$





#### b) $\lim_{x \to 0} \sqrt[x^3]{1 - x + \sin x}$

**解：**
原式 = 
$$
\lim_{x \to 0} e^{\frac{\ln{(1-x+\sin x)}}{x^3}}
$$
$$
= \lim_{x \to 0} e^{\frac{\ln{(1-\frac{x^3}{6}+o(x^5))}}{x^3}}
$$
$$
= \lim_{x \to 0} e^{\frac{-\frac{x^3}{6}}{x^3}}
$$
$$
= e^{-\frac{1}{6}}
$$



### 8. 设 $f(x) = (1 + x)^{\frac{1}{x}}$ 在 $x = 0$ 处连续，证明：当 $x \to 0$ 时，成立

$$
f(x) = e + Ax + Bx^2 + o(x^2)
$$
并计算 $A, B$ 的值

**解：**
$$
f(x) = e^{\frac{\ln f(x)}{x}}
$$
$$
= e^{\frac{\ln(1+x)}{x}}
$$
$$
= e^{1 - \frac{x}{2} + \frac{x^2}{3} + O(x^3)} 
$$
$$
= e (1 - \frac{x}{2} + \frac{11}{24}x^2 + o(x^2))
$$

A = -$\frac{e}{2}$  
B = $\frac{11e}{24}$



### 9.

#### (a) 证明：对 $n = 0, 1, 2, \cdots$ 方程 $e^x + x^{2n+1} = 0$ 有唯一实根 $x_n$

**解：**
$$
f_n(x) = e^x + x^{2n+1}
$$

$$
f_n'(x) = e^x + (2n+1)x^{2n} > 0 \quad f_n(x_n) \text{单调增加}
$$

$$
\lim_{x \to -\infty} f_n(x) = -\infty \quad f_n(0) = 1 > 0
$$

故 $\exists x, t(-\infty, 0) \quad s.t. \quad f_n(x_n) = 0$





#### (b) 证明：$\lim_{n \to \infty} x_n$ 的极限存在

**解：**
$$
e^{\lambda n} + x_n^{2n+1} = 0
$$

$$
f_{n+1}(x_n) = e^{x_n} +x_n^{2n+3} = x_n^{2n+1} \quad (1 + x_n^2) < 0
$$

$$
f_n(x_n) \text{单调增加} \quad f_n(x_n) < 0
$$

故 $\lim_{n \to \infty} x_n$ 存在



#### (c) 记 $\lim_{n \to \infty} x_n = A$，证明：$x_n - A$ 和 $\frac{1}{n}$ 是同阶无穷小

**解：**

$$
\quad |A| < 1 \quad x_{n}^{2n+1} \to 0 \quad e^A = 0
$$

$$
\begin{array}{ccc}
|A| > 1 & |x_{n}^{2n+1}| & \text{发散} \\
\end{array}
$$

故 $|A| = 1$，$A = -1$

令 $\chi_n = -1 + \epsilon_n (\epsilon_n > 0)$

$$
e^{-1+\epsilon_n} + (-1 + \epsilon_n)^{2n+1} = 0
$$

$$
e^{-1+\epsilon_n} = (1-\epsilon_n)^{2n+1}
$$

$$
-1 + \epsilon_n = (2n+1)|h(1-\epsilon_n)
$$

$$
\ln(1-\epsilon_n) = -\epsilon_n + O(\epsilon_n^2)
$$

$$
-1 + \epsilon_n = (2n+1)(-\epsilon_n + O(\epsilon_n^2))
$$

$$
-1 + \epsilon_n \approx -(2n+1)\epsilon_n
$$

$$
\epsilon_n \approx \frac{1}{2n+2} \sim \frac{1}{2n}(n \to \infty)
$$

$x_n - (-1) = x_{n+1} = \epsilon \quad \text{与} \quad \frac{1}{n} \quad \text{同阶无穷小;}$
