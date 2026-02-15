# <center>hw_6<center>

## 必做题：

### 1. 设 $f(x)$ 在 $\mathbb{R}$ 上可导，利用导数的定义计算下列各式的值  
#### a) $\lim_{x \to 0} \frac{f(x)}{x}$，其中 $f(0) = 0$;

**解：**


原式 = $\lim_{x \to 0} \frac{f(x) - f(0)}{x - 0} = f'(0)$



#### b) $\lim_{\Delta x \to 0} \frac{f(x_0 - \Delta x) - f(x_0)}{\Delta x}$

**解：**

原式 = $\lim_{\Delta x \to 0} \frac{f(x_0 - \Delta x) - f(x_0)}{\Delta x} = -f'(x_0)$



#### c) $\lim_{h \to 0} \frac{f(x_0 + h) - f(x_0 - h)}{h}$;

**解：** 
原式 = $\lim_{h \to 0} \frac{f(x_0 + h) - f(x_0 - h)}{h} = 2f'(x_0)$



#### d) $\lim_{h \to 0} \frac{f^2(x_0 + 3h) - f^2(x_0 - h)}{h}$

**解：**
原式 = $\lim_{h \to 0} \frac{f^2(x_0 + 3h) - f^2(x_0 - h)}{h} = \lim_{h \to 0} \frac{[f(x_0 + 3h) - f(x_0 - h)][f(x_0 + 3h) + f(x_0 - h)]}{h} = 4f'(x_0) \cdot 2f(x_0) = 8f(x_0)f'(x_0)$



### 2. 求下列函数在 $x_0$ 处的左、右导数，并指出它在该点的可导性。

#### a) 
$f(x) = \begin{cases} 
    \sin x, & x \geq 0 \\ 
    x^2, & x < 0
   \end{cases}$  $x_0=0$

**解：**
$$
f'_-(0) = \lim_{x \to 0^-} \frac{x^2 - 0}{x - 0} = 0
$$
$$
f'_+(0) = \lim_{x \to 0^+} \frac{\sin x - 0}{x - 0} = \cos 0 = 1
$$
$$
f'_-(0) \neq f'_+(0) \quad \text{不可导}
$$



#### b) 
$f(x) = \begin{cases} 
    \frac{x}{1+e^{\frac{1}{x}}}, & x \neq 0, \\ 
    0, & x = 0
   \end{cases}$  $x_0=0$

**解：**
$$
f'_-(0) = \lim_{x \to 0^-} \frac{\frac{x}{1+e^{1/x}} - 0}{x - 0} = \lim_{x \to 0^-} \frac{1}{1+e^{1/x}} = 1
$$

$$
f'_+(0) = \lim_{x \to 0^+} \frac{\frac{x}{1+e^{1/x}} - 0}{x - 0} = \lim_{x \to 0^+} \frac{1}{1+e^{1/x}} = 0
$$

$$
f'_-(0) \neq f'_+(0) \quad \text{不可导}
$$





#### c) 
$f(x) = \begin{cases} 
    x^2 \sin \frac{1}{x}, & x \neq 0 \\ 
    0, & x = 0
   \end{cases}$  $x_0=0$

**解：**
$$
f'_-(0) = \lim_{x \to 0^-} \frac{x^2 \sin \frac{1}{x} - 0}{x - 0} = \lim_{x \to 0^-} x \sin \frac{1}{x} = 0
$$

$$
f'_+(0) = \lim_{x \to 0^+} \frac{x^2 \sin \frac{1}{x} - 0}{x - 0} = \lim_{x \to 0^+} x \sin \frac{1}{x} = 0
$$

$$
f'_-(0) = f'_+(0) = 0 \quad \text{可导}
$$





#### d) 
$f(x) = \begin{cases} 
    x^2, & x \leq 1 \\ 
    ax + b, & x > 1
   \end{cases}$  $x_0=1$

**解：**
$$
f'_-(1) = \lim_{x \to 1^-} \frac{x^2 - 1}{x - 1} = 2
$$

$$
f'_+(1) = \lim_{x \to 1^+} \frac{ax + b - 1}{x - 1} = a
$$

$a = 2$, $b = -1$ 时可导，否则不可导



### 3. 求导数  
#### a)
$f(x) = \begin{cases} 
    x^2 e^{-x^2}, & |x| \leq 1, \\ 
    \frac{1}{e}, & |x| > 1
   \end{cases}$  

**解：**
a) $|x| > 1$  
$f'(x) = 0$  

$|x| \leq 1$  
$$
f'(x) = 2xe^{-x^2} + x^2 (-2x)e^{-x^2}
$$

$$
= (2x - 2x^3)e^{-x^2}
$$

$$
= 2x(1-x^2)e^{-x^2}
$$

$$
f'(x) = 
\begin{cases} 
2x(1-x^2)e^{-x^2}, & |x| \leq 1 \\ 
0, & |x| > 1 
\end{cases}
$$





#### b) 
$f(x) = \arccos \frac{1}{|x|}$

**解：** $\frac{1}{|x|} \in (0,1]$  
当 $x > 1$  
$$
f'(x) = -\frac{1}{\sqrt{1-\frac{1}{x^2}}} \left(-\frac{1}{x^2}\right)
$$

$$
= \frac{1}{x^2 \sqrt{1-\frac{1}{x^2}}}
= \frac{1}{\sqrt{x^4 - x^2}}
$$

当 $x < -1$  

$$
f'(x) = -\frac{1}{\sqrt{1-\frac{1}{x^2}}} \left(\frac{1}{x^2}\right)
= -\frac{1}{\sqrt{x^4 - x^2}}
$$

$$
f'(x) = 
\begin{cases} 
\frac{1}{\sqrt{x^4 - x^2}}, & x > 1 \\ 
-\frac{1}{\sqrt{x^4 - x^2}}, & x < -1 
\end{cases}
$$

$x = \pm 1$ 时不可导



### 4. 按定义求导数  
#### a) $f(x) = x^2 + 4x + 200$;

**解：**
$$
f'(x) = \lim_{\Delta x \to 0} \frac{f(x+\Delta x) - f(x)}{\Delta x}
$$

$$
= \lim_{\Delta x \to 0} \frac{(x+\Delta x)^2 + 4(x+\Delta x) + 200 - (x^2 + 4x + 200)}{\Delta x}
$$

$$
= \lim_{\Delta x \to 0} \frac{2x\Delta x + (\Delta x)^2 + 4\Delta x}{\Delta x}
$$

$$
= \lim_{\Delta x \to 0} (2x + 4 + \Delta x)
$$

$$
= 2x + 4
$$





#### b) $f(x) = x \sin x$

**解：**
$$
f'(x) = \lim_{\Delta x \to 0} \frac{f(x+\Delta x) - f(x)}{\Delta x}
$$

$$
= \lim_{\Delta x \to 0} \frac{(x+\Delta x) \sin(x+\Delta x) - x \sin x}{\Delta x}
$$

$$
= \lim_{\Delta x \to 0} \left[ x \cdot \frac{\sin(x+\Delta x) - \sin x}{\Delta x} + \sin(x+\Delta x) \right]
$$

$$
= x \cos x + \sin x
$$



### 5. 计算导数  
#### a) $y = \frac{1 - \sqrt[3]{2x - 1}}{1 + \sqrt[3]{2x - 1}}$;

**解：**
$$
y = -1 + \frac{2}{1 + \sqrt[3]{2x-1}}
$$

$$
y' = -\frac{2}{(1+\sqrt[3]{2x-1})^2} \cdot \frac{2}{3}(2x-1)^{-\frac{2}{3}} 
$$

$$
= -\frac{4}{3(2x-1)^{\frac{2}{3}}(1+\sqrt[3]{2x-1})^2}
$$



#### b) $y = \sin (\cos^2 x) \cdot \cos (\sin^2 x)$

**解：**
$$
y' = \cos(\cos^2 x) \cdot 2\cos x (-\sin x) \cdot \cos(\sin^2 x) + \sin(\cos^2 x) \cdot [-\sin(\sin^2 x) \cdot 2\sin x \cos x]
$$

$$
= -2\sin x \cos x [\cos(\cos^2 x) \cos(\sin^2 x) + \sin(\cos^2 x) \sin(\sin^2 x)]
$$

$$
= -2\sin x \cos x \cos(\cos^2 x - \sin^2 x)
$$





#### c) $y = \frac{x}{2} \sqrt{x^2 + a  }+ \frac{a^2}{2}\ln (x + \sqrt{x^2 + a^2})$;

**解：**
$$
y' = \sqrt{x^2 + a} + \frac{x}{2} \cdot \frac{1}{2\sqrt{x^2 + a}} \cdot x  + \frac{a^2}{2} \cdot \frac{1}{x + \sqrt{x^2 + a^2}} \left(1 + \frac{x}{\sqrt{x^2 + a^2}}\right)
$$

$$
= \frac{2x^2 + a}{2\sqrt{x^2 + a}}  + \frac{a^2}{2\sqrt{x^2+a^2}}
$$



#### d) $y = x \arcsin (\ln x)$

**解：**
$$
y' = \arcsin(\ln x) + x \cdot \frac{1}{\sqrt{1-(\ln x)^2}} \cdot \frac{1}{x}
$$

$$
= \arcsin(\ln x) + \frac{1}{\sqrt{1-(\ln x)^2}}
$$





#### e) $y = e^{\arctan \sqrt{x}}$;

**解：**
$$
y' = e^{\arctan \sqrt{x}} \cdot \frac{1}{1+x} \cdot \frac{1}{2\sqrt{x}}
$$





####  f) $y = 10^{x \tan x^2}$

**解：**
$$
y' = 10^{x \tan x^2} \ln 10 \cdot (\tan x^2 + x \cdot \frac{1}{\cos^2 x^2} \cdot 2x)
$$

$$
= 10^{x \tan x^2} \ln 10 \cdot (\tan x^2 + \frac{2x^2}{\cos^2 x^2})
$$





### 6. 用对数求导法求导数  
#### a) $y = \frac{(x + 1)^2 \sqrt[3]{4x + 3}}{\sqrt[3]{2x^2 + 2x + 1}}$;

**解：**
$$
\ln y = 2 \ln (x + 1) + \frac{1}{3} \ln (4x + 3) - \frac{1}{3} \ln (2x^2 + 2x + 1)
$$

$$
\frac{y'}{y} = \frac{2}{x + 1} + \frac{4}{3(4x + 3)} - \frac{4x + 2}{3(2x^2 + 2x + 1)}
$$

$$
y' = \frac{(x + 1)^2 \sqrt[3]{4x + 3}}{\sqrt[3]{2x^2 + 2x + 1}} \left[ \frac{2}{x + 1} + \frac{4}{3(4x + 3)} - \frac{4x + 2}{3(2x^2 + 2x + 1)} \right]
$$



#### b) $y = (\sin x)^{\cos x} + (\cos x)^{\sin x}$

**解：**
$y_1 = (\sin x)^{\cos x}$, $y_2 = (\cos x)^{\sin x}$
$$
\frac{y_1'}{y_1} = -\sin x \ln \sin x + \cos x \cdot \frac{\cos x}{\sin x}
$$

$$
\frac{y_2'}{y_2} = \sin x \ln \cos x + \cos x \cdot \left(-\frac{\sin x}{\cos x}\right)
$$

$$
y' = y_1' + y_2' = (\sin x)^{\cos x} \left( \frac{\cos^2 x}{\sin x} - \sin x \ln \sin x \right) + (\cos x)^{\sin x} \left(\sin x \ln \cos x -  \frac{\sin^2 x}{\cos x}) \right)
$$





#### c) $y = \left( \frac{x}{1 + x} \right)^x$;

**解：**
$$
\ln y = x \ln \left( \frac{x}{1+x} \right)
$$

$$
\frac{y'}{y} = \ln \left( \frac{x}{1+x} \right) + x \cdot \frac{1+x}{x} \cdot \frac{1}{(1+x)^2}
$$

$$
y' = \left( \frac{x}{1+x} \right)^x \left( \ln \frac{x}{1+x} + \frac{1}{1+x} \right)
$$





#### d) $y = \sqrt{x \sin x \sqrt{1 - e^x}}$

**解：**
$$
\ln y = \frac{1}{2} \ln x + \frac{1}{2} \ln \sin x + \frac{1}{4} \ln (1 - e^x)
$$

$$
\frac{y'}{y} = \frac{1}{2x} + \frac{\cos x}{2 \sin x} - \frac{e^x}{4(1 - e^x)}
$$

$$
y' = \sqrt{x \sin x \sqrt{1 - e^x}} \left[ \frac{1}{2x} + \frac{\cos x}{2 \sin x} - \frac{e^x}{4(1 - e^x)} \right]
$$



### 7. 设 $f(x)$ 是定义在 $(-1,1)$ 上的连续正值函数，且 $f(0)=1$，$f'(0)=2$，计算 
$$
\lim_{x \to 0} (f(x))^{\frac{1}{x}}
$$

**解：**

取对数：  
$$
\ln \left( (f(x))^{\frac{1}{x}} \right) = \frac{\ln f(x)}{x}
$$



当 $ x \to 0 $ 时，  
$$
f(x) = f(0) + f'(0)x + o(x) = 1 + f'(0)x + o(x)
$$

$$
\ln f(x) = \ln(1 + f'(0)x + o(x)) \sim f'(0)x + o(x)
$$

$$
\frac{\ln f(x)}{x} \sim \frac{f'(0)x + o(x)}{x} = f'(0) + o(1)
$$

所以：  
$$
\lim_{x \to 0} \frac{\ln f(x)}{x} = f'(0)=2
$$

$$
\lim_{x \to 0} (f(x))^{\frac{1}{x}} = e^2
$$



### 8. 计算函数的微分

#### a) $y = \ln \tan \frac{x}{2}$;

**解：**
$$
\frac{dy}{dx} = \frac{1}{\tan \frac{x}{2}} \cdot \frac{1}{\cos^2 \frac{x}{2}} \cdot \frac{1}{2}
$$
$$
dy = \frac{1}{2\sin \frac{x}{2} \cos \frac{x}{2}} dx = \frac{1}{\sin x} dx
$$



#### b) $y = \sqrt{x+\sqrt{x + \sqrt{x}}}$

**解：**
$$
\frac{dy}{dx} = \frac{1}{2\sqrt{x + \sqrt{x + \sqrt{x}}}} \cdot \left(1 + \frac{1}{2\sqrt{x + \sqrt{x}}} \cdot \left(1 + \frac{1}{2\sqrt{x}}\right)\right)
$$

$$
dy = \frac{1}{2\sqrt{x + \sqrt{x + \sqrt{x}}}} \left[ 1 + \frac{1}{2\sqrt{x + \sqrt{x}}} \left(1 + \frac{1}{2\sqrt{x}}\right) \right] dx
$$





#### c) $y = \arctan \frac{v}{u}$ ($v, u$ 用 $du, dv$ 表示之);

**解：**
$$
dy = \frac{1}{1 + \frac{v^2}{u^2}} d\left(\frac{v}{u}\right)
$$

$$
dy = \frac{u^2}{u^2 + v^2} \cdot \frac{udv - vdu}{u^2}
$$

$$
= \frac{udv - vdu}{u^2 + v^2}
$$





#### d) $y = \ln (\ln (x))$

**解：**
$$
dy = \frac{1}{\ln x} \cdot \frac{1}{x} dx
$$

$$
dy = \frac{1}{x \ln x} dx
$$





### 9. 证明函数 $y = f(x)$ 的反函数的二阶导数公式 
$$
\frac{d^2 x}{dy^2} = -\frac{\frac{d^2 y}{dx^2}}{\left(\frac{dy}{dx}\right)^3}
$$

**解：**
$$
\frac{d^2x}{dy^2} = \frac{d}{dy} \left( \frac{1}{\frac{dy}{dx}} \right) = \frac{d}{dx} \left( \frac{1}{\frac{dy}{dx}} \right) \frac{dx}{dy} = -\frac{\frac{d^2y}{dx^2}}{\left( \frac{dy}{dx} \right)^2} \cdot \frac{1}{\frac{dy}{dx}} = -\frac{\frac{d^2y}{dx^2}}{\left( \frac{dy}{dx} \right)^3}
$$
即
$$
\frac{d^2x}{dy^2} = -\frac{\frac{d^2y}{dx^2}}{\left( \frac{dy}{dx} \right)^3}
$$



### 10. 计算下列函数反函数的一阶导数和二阶导数

#### a) $\theta = r \arctan r$ ;

**解：**
$$
\frac{dr}{d\theta} = \frac{1}{\arctan r + \frac{r}{1+r^2}}
$$

$$
\frac{d^2 r}{d\theta^2} = -\frac{2}{(1+r^2)^2 \left( \arctan r + \frac{r}{1+r^2} \right)^3}
$$



#### b) $y = \frac{1}{2} \ln \frac{1 - x}{1 + x}$

**解：**
$$
\frac{dx}{dy} = \frac{1}{\frac{dy}{dx}} = \frac{1}{-\frac{1}{1-x^2}} = -1 + x^2
$$

$$
\frac{d^2 x}{dy^2}  = -2x(1-x^2)
$$



#### c) $y = e^{\arcsin x}$;

**解：**
$$
\frac{dx}{dy} = \frac{1}{\frac{dy}{dx}} = \frac{1}{\frac{e^{\arcsin x}}{\sqrt{1-x^2}}} = \frac{\sqrt{1-x^2}}{e^{\arcsin x}}
$$

$$
\frac{d^2 x}{dy^2}  = \frac{ - x - \sqrt{1-x^2}}{e^{2\arcsin x}}
$$





#### d) $y = 2x - \cos \frac{x}{2}$

**解：**
$$
\frac{dx}{dy} = \frac{1}{\frac{dy}{dx}} = \frac{1}{2 + \frac{1}{2}\sin\frac{x}{2}} = \frac{2}{4 + \sin\frac{x}{2}}
$$

$$
\frac{d^2 x}{dy^2} = -\frac{2\cos\frac{x}{2}}{(4 + \sin\frac{x}{2})^3}
$$


### 11.  
#### a) 设 $y = e^x \cos x$，求 $y^{(4)}$;

**解：**
$$
y = e^x \cos x
$$

$$
y' = e^x \cos x - e^x \sin x
$$

$$
y'' = (e^x \cos x - e^x \sin x) - (e^x \sin x + e^x \cos x) = -2e^x \sin x
$$

$$
y''' = -2e^x \sin x - 2e^x \cos x
$$

$$
y^{(4)} = (-2e^x \sin x - 2e^x \cos x) + (2e^x \sin x - 2e^x \cos x) = -4e^x \cos x
$$





#### b) 设 $y = (x+1)^2 e^{2x}$，求 $y^{(100)}$

**解：**$y = (x+1)^2 e^{2x}$
$$
y^{(n)} = 2^n e^{2x} \left[ (x+1)^2 + n(x+1) + \frac{n(n-1)}{4} \right]
$$

$$
y^{(100)} = 2^{100} e^{2x} \left( x^2 + 102x + 2576 \right)
$$


### 12. 求 $n$ 阶导数  
#### a) $y = \frac{1-x}{1+x}$;

**解：**
$$
y = \frac{1 - x}{1 + x} = -1 + \frac{2}{1 + x}
$$
$$
y^{(n)} = 2(-1)^n n! (1 + x)^{-n-1}
$$





#### b) $y = \frac{1}{x^2-3x+2}$

**解：**
$$
y = \frac{1}{x^2 - 3x + 2} = \frac{1}{x-2} - \frac{1}{x-1}
$$

$$
y^{(n)} = (-1)^n n! \left[ (x-2)^{-n-1} - (x-1)^{-n-1} \right]
$$





#### c) $y = x \ln x$;

**解：**
$$
y = x \ln x
$$

$$
y' = \ln x + 1, \quad y'' = \frac{1}{x}
$$

$$
y^{(n)} = (-1)^n (n-2)! x^{-n+1}, \quad n \geq 2
$$





#### d) $y = \sin^2 x$

**解：**
$$
y = \sin^2 x = \frac{1}{2} - \frac{1}{2} \cos 2x
$$
$$
y^{(n)} = -2^{n-1} \cos \left( 2x + \frac{n\pi}{2} \right)
$$



### 13.

#### (a) 设函数 $f(x)$ 在 $x=0$ 处连续，$f^2(x)$ 在 $x=0$ 处的导数为 $A$，讨论 $f(x)$ 在 $x=0$ 处的可导性;

**解：**
$$
A = f^2(0)' = 2f(0)f'(0)
$$

当 $f(0) = 0$，$A = 0$  $f(x)$ 不一定可导  

当 $f(0) \neq 0$，$f'(0) = \frac{A}{2f(0)}$  可导

 

#### (b) 设 $xf(x)$ 在 $x_0 (\neq 0)$ 处可导，证明 $f(x)$ 在 $x_0$ 处可导

**解：**
$$
g(x) = x f(x)
$$

$$
g'(x_0) = \lim_{x \to x_0} \frac{x f(x) - x_0 f(x_0)}{x - x_0}
$$

$$
= x_0 \lim_{x \to x_0} \frac{f(x) - f(x_0)}{x - x_0} + f(x_0)
$$

$x_0 \neq 0$，$g'(x)$ 存在  

故 $f(x)$ 在 $x_0$ 处可导



### 14. 设 $f(x)$ 是偶函数，且 $f'(0)$ 存在，证明: $f'(0) = 0$

**解：**
$$
f(x) = f(-x)
$$

$$
f'(-x) = -f'(x)
$$

令 $x = 0$：
$$
f'(0) = -f'(0)
$$

故
$$
f'(0) = 0
$$



## 选做题:

### 1. 若 $F(x)$ 在 $a$ 处连续，且 $F(x) \neq 0$，试讨论函数 $f(x) = |x-a|F(x)$ 在 $x=a$ 处的可导性

**解：**
$$
f'_-(a) = \lim_{x \to a^-} \frac{|x-a|F(x) - 0}{x - a} = \lim_{x \to a^-} \frac{-(x-a)F(x)}{x - a} = -F(a)
$$

$$
f'_+(a) = \lim_{x \to a^+} \frac{|x-a|F(x) - 0}{x - a} = \lim_{x \to a^+} \frac{(x-a)F(x)}{x - a} = F(a)
$$

由于 $F(a) \neq 0$, $f'_-(a) \neq f'_+(a)$

故在 $x = a$ 处不可导



### 2. 若 $\forall x,y \in \mathbb{R}$ 有 $f(x+y) = f(x) + f(y) + 2xy$，且 $f'(0)$ 存在，求 $f'(x)$

**解：**
$$
f'(x) = \lim_{\Delta x \to 0} \frac{f(x + \Delta x) - f(x)}{\Delta x}
$$

$$
= \lim_{\Delta x \to 0} \frac{[f(x) + f(\Delta x) + 2x\Delta x] - f(x)}{\Delta x}
$$

$$
= \lim_{\Delta x \to 0} \frac{f(\Delta x)}{\Delta x} + 2x
$$

$$
= f'(0) + 2x
$$



### 3. 按定义证明: 可导的偶函数的导函数是奇函数，可导的奇函数的导函数是偶函数；可导的周期函数的导函数仍然是周期函数，且周期不变

**解：** 
① 偶函数：$f(x) = f(-x)$  
$$
f'(-x) = -f'(x)
$$

② 奇函数：$f(-x) = -f(x)$  
$$
f'(-x) = f'(x)
$$

③ 周期函数：$f(x+T) = f(x)$  
$$
f'(x+T) = f'(x)
$$
