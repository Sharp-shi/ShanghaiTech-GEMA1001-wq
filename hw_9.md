# <center>hw_9<center>

## 1. 求下列不定积分（可考虑利用三角恒等式化简后凑微分）

### a)  $\displaystyle\int \cos^2 \frac{x}{2} dx$

**解：** 
$$
\begin{aligned}
\text{原式} &= \int \frac{1 + \cos x}{2} \, dx \\
&= \frac{1}{2}x + \frac{1}{2}\sin x + C
\end{aligned}
$$



### b)  $\displaystyle\int \frac{\cos 2x}{\cos x + \sin x} dx$

**解：**
$$
\begin{aligned}
\text{原式} &= \int \frac{\cos^2 x - \sin^2 x}{\cos x + \sin x} \, dx \\
&= \int (\cos x - \sin x) \, dx \\
&= \sin x + \cos x + C
\end{aligned}
$$




### c)  $\displaystyle\int \frac{1 + \cos^2 x}{1 + \cos 2x} dx$

**解：**
$$
\begin{aligned}
\text{原式} &= \int \frac{1 + \cos^2 x}{2\cos^2 x} \, dx \\
&= \int \left( \frac{1}{2} + \frac{1}{2\cos^2 x} \right) dx \\
&= \frac{1}{2}x + \frac{1}{2}\tan x + C
\end{aligned}
$$




### d)  $\displaystyle\int \frac{dx}{\cos^2 x \sin^2 x}$

**解：**
$$
\begin{aligned}
\text{原式} &= \int \left( \frac{1}{\cos^2 x} + \frac{1}{\sin^2 x} \right) dx \\
&= \tan x - \cot x + C
\end{aligned}
$$




## 2. 求下列不定积分（可化简后（利用换元）凑微分）

### a)  $\displaystyle\int \frac{dx}{e^x - e^{-x}}$

**解：**
令 $ u = e^x $  
则 $ x = \ln u $，$ dx = \frac{du}{u} $

$$
\begin{aligned}
\text{原式} &= \int \frac{du}{u^2 - 1} \\
&= \int \frac{1}{2} \left( \frac{1}{u - 1} - \frac{1}{u + 1} \right) du \\
&= \frac{1}{2} \ln \left| \frac{u - 1}{u + 1} \right| + C
\end{aligned}
$$




### b)  $\displaystyle\int \frac{2x - 5}{(x^2 - 5x + 8)^2} dx$

**解：**
令 $ u = x^2 - 5x + 8 $  
则 $ du = (2x - 5)\,dx $
$$
\begin{aligned}
\text{原式} &= \int \frac{du}{u^2} \\
&= -\frac{1}{u} + C \\
&= -\frac{1}{x^2 - 5x + 8} + C
\end{aligned}
$$




### c)  $\displaystyle\int \frac{x^2}{\sqrt[3]{1 - 2x^3}} dx$

**解：**

令 $ u = \sqrt[3]{1 - 2x^3} $  
则 $ u^3 = 1 - 2x^3 $  
$ 3u^2\,du = -6x^2\,dx $  
$ x^2\,dx = -\frac{1}{2}u^2\,du $

$$
\begin{aligned}
\text{原式} &= \int \frac{-u^2}{2u} \, du \\
&= \int -\frac{1}{2}u \, du \\
&= -\frac{1}{4}u^2 + C \\
&= -\frac{1}{4}(1 - 2x^3)^{\frac{2}{3}} + C
\end{aligned}
$$



### d)  $\displaystyle\int e^x \sin (e^x) dx$

**解：**
令 $ u = e^x $  
则 $ du = e^x\,dx $
$$
\begin{aligned}
\text{原式} &= \int \sin u \, du \\
&= -\cos u + C \\
&= -\cos(e^x) + C
\end{aligned}
$$




### e)  $\displaystyle\int \frac{\sin x + \cos x}{\sqrt[3]{\sin x - \cos x}} dx$

**解：**
令 $ u = \sin x - \cos x $  
则 $ du = (\cos x + \sin x)\,dx $

$$
\begin{aligned}
\text{原式} &= \int \frac{du}{u^{\frac{1}{3}}} \\
&= \frac{3}{2} u^{\frac{2}{3}} + C \\
&= \frac{3}{2} (\sin x - \cos x)^{\frac{2}{3}} + C
\end{aligned}
$$



### f)  $\displaystyle\int \frac{\arctan \sqrt{x}}{\sqrt{x}(1 + x)} dx$

**解：**
令 $ u = \sqrt{x} $  
则 $ x = u^2 $，$ dx = 2u\,du $
$$
\begin{aligned}
\text{原式} &= \int \frac{2 \arctan u}{1 + u^2} \, du \\
\text{令 } t &= \arctan u \\
dt &= \frac{1}{1 + u^2} \, du
\end{aligned}
$$

$$
\begin{aligned}
\text{原式} &= \int 2t \, dt \\
&= t^2 + C \\
&= (\arctan \sqrt{x})^2 + C
\end{aligned}
$$



### g)  $\displaystyle\int \frac{dx}{x \ln x}$

**解：**
令 $ u = \ln x $  
则 $ du = \frac{dx}{x} $
$$
\begin{aligned}
\text{原式} &= \int \frac{du}{u} \\
&= \ln |u| + C \\
&= \ln |\ln x| + C
\end{aligned}
$$



### h)  $\displaystyle\int \frac{x^2}{4 + x^6} dx$

**解：**
令 $ u = x^3 $  
则 $ du = 3x^2\,dx $

$$
\begin{aligned}
\text{原式} &= \int \frac{1}{3} \cdot \frac{du}{4 + u^2} \\
&= \frac{1}{6} \arctan \frac{u}{2} + C \\
&= \frac{1}{6} \arctan \frac{x^3}{2} + C
\end{aligned}
$$




## 3. 求下列不定积分（最好直接变量替换后化简整理成简单积分）

### a)  $\displaystyle\int e^x \sqrt{1 - e^{2x}} dx$

**解：**
令 $ u = e^x $  
则 $ du = e^x\,dx $
$$
\begin{aligned}
\text{原式} &= \int \sqrt{1 - u^2} \, du \\
\text{令 } u &= \sin t \\
du &= \cos t \, dt
\end{aligned}
$$

$$
\begin{aligned}
\text{原式} &= \int \cos^2 t \, dt \\
&= \int \frac{1 + \cos 2t}{2} \, dt \\
&= \frac{1}{2}t + \frac{\sin 2t}{4} + C \\
&= \frac{1}{2} \arcsin(e^x) + \frac{1}{4} \cdot 2 \sin t \cos t + C \\
&= \frac{1}{2}( \arcsin(e^x) + e^x \sqrt{1 - e^{2x}} )+ C
\end{aligned}
$$



### b)  $\displaystyle\int \frac{dx}{\sqrt{1 + e^x}}$

**解：**

令 $ \sqrt{1 + e^x} = u $  
则 $ 1 + e^x = u^2 $  
$ e^x\,dx = 2u\,du $  
又 $ e^x = u^2 - 1 $，故 $ dx = \frac{2u}{u^2 - 1}\,du $

$$
\begin{aligned}
\text{原式} &= \int \frac{2\,du}{u^2 - 1} \\
&= \ln \left| \frac{u - 1}{u + 1} \right| + C \\
&= \ln  \frac{\sqrt{1 + e^x} - 1}{\sqrt{1 + e^x} + 1}  + C
\end{aligned}
$$





### c)  $\displaystyle\int \frac{dx}{1 + e^x}$

**解：**
$$
\text{原式} = \int \frac{e^{-x}}{e^{-x} + 1} \, dx
$$

令 $ u = 1 + e^{-x} $  
则 $ du = -e^{-x}\,dx $

$$
\begin{aligned}
\text{原式} &= \int \frac{-du}{u} \\
&= -\ln |u| + C \\
&= -\ln(1 + e^{-x}) + C
\end{aligned}
$$



### d)  $\displaystyle\int \frac{1 + \ln x}{(x \ln x)^2} dx$

**解：**
令 $ u = x \ln x $  
则 $ du = (\ln x + 1)\,dx $
$$
\begin{aligned}
\text{原式} &= \int \frac{du}{u^2} \\
&= -\frac{1}{u} + C \\
&= -\frac{1}{x \ln x} + C
\end{aligned}
$$



### e)  $\displaystyle\int \frac{x^2}{(x + 1)^{100}} dx$

**解：**
令 $ u = x + 1 $  
则 $ du = dx $
$$
\begin{aligned}
\text{原式} &= \int \frac{u^2 - 2u + 1}{u^{100}} \, du \\
&= \int \left( u^{-98} - 2u^{-99} + u^{-100} \right) du \\
&= -\frac{u^{-97}}{97} + \frac{u^{-98}}{49} - \frac{u^{-99}}{99} + C \\
&= -\frac{1}{97(x+1)^{97}} + \frac{1}{49(x+1)^{98}} - \frac{1}{99(x+1)^{99}} + C
\end{aligned}
$$



### f)  $\displaystyle\int \frac{\sqrt{3 + 2x}}{x} dx$

**解：**
令 $ u = \sqrt{3 + 2x} $  
则 $ u^2 = 3 + 2x $，$ dx = u\,du $  
解得 $ x = \frac{u^2 - 3}{2} $

$$
\begin{aligned}
\text{原式} &= \int \frac{2u^2}{u^2 - 3} \, du \\
&= \int \left( 2 + \frac{6}{u^2 - 3} \right) du \\
&= \int \left( 2 + \frac{6}{(u - \sqrt{3})(u + \sqrt{3})} \right) du
\end{aligned}
$$

$$
\begin{aligned}
&= \int \left( 2 + \frac{\sqrt{3}}{u - \sqrt{3}} - \frac{\sqrt{3}}{u + \sqrt{3}} \right) du \\
&= 2u + \sqrt{3} \ln \left| \frac{u - \sqrt{3}}{u + \sqrt{3}} \right| + C \\
&= 2\sqrt{3 + 2x} + \sqrt{3} \ln  \frac{\sqrt{3 + 2x} - \sqrt{3}}{\sqrt{3 + 2x} + \sqrt{3}}  + C
\end{aligned}
$$



## 4. 求下列定积分

### a)  $\displaystyle\int_1^4 \frac{dx}{x(1 + \sqrt{x})}$

**解：**

令 $ u = \sqrt{x} $  
则 $ u^2 = x $，$ dx = 2u\,du $

$$
\begin{aligned}
\int \frac{dx}{x(1 + \sqrt{x})} &= \int \frac{2u\,du}{u^2(1 + u)} \\
&= \int \frac{2\,du}{u(1 + u)} \\
&= 2 \ln \left| \frac{u}{1 + u} \right| + C
\\
&= 2 \ln  \frac{\sqrt{x}}{1 + \sqrt{x}}  + C
\end{aligned}
$$

$$
\begin{aligned}
\text{原式} &= 2 \left( \ln 2 - \ln 3 - \ln 1 + \ln 2 \right) \\
&= 2 \left( 2\ln 2 - \ln 3 \right) \\
&= 2 \ln \frac{4}{3}
\end{aligned}
$$





### b)  $\displaystyle\int_0^{\frac{\pi}4} \frac{\sin x}{1 + \sin x} dx$

**解：**
$$
\int \frac{\sin x}{1 + \sin x} \, dx
$$

$$
\begin{aligned}
&= \int \left( 1 - \frac{1}{1 + \sin x} \right) dx \\
&= \int \left( 1 - \sec^2 x + \tan x \sec x \right) dx \\
&= x - \tan x + \sec x + C
\end{aligned}
$$



$$
\begin{aligned}
\text{原式} &= \left[ x - \tan x + \sec x \right]_0^{\frac{\pi}{4}} \\
&= \left( \frac{\pi}{4} - 1 + \sqrt{2} \right) - (0 - 0 + 1) \\
&= \frac{\pi}{4} - 1 + \sqrt{2} - 1 \\
&= \frac{\pi}{4} - 2 + \sqrt{2}
\end{aligned}
$$





## 5. 求下列不定积分（用三角替换处理比较适宜）

### a)  $\displaystyle\int \frac{dx}{\sqrt{(1-x^2)^3}}$

**解：**
令 $ x = \sin t $  
则 $ dx = \cos t\,dt $

$$
\begin{aligned}
\text{原式} &= \int \frac{\cos t\,dt}{\cos^3 t} \\
&= \int \frac{1}{\cos^2 t}\,dt \\
&= \int \sec^2 t\,dt \\
&= \tan t + C \\
&= \frac{\sin t}{\cos t} + C \\
&= \frac{x}{\sqrt{1 - x^2}} + C
\end{aligned}
$$



### b)  $\displaystyle\int \frac{dx}{x\sqrt{a^2-x^2}} \quad (a>0)$

**解：**

令 $ x = a \sin t $  
则 $ dx = a \cos t\,dt $

$$
\begin{aligned}
\text{原式} &= \int \frac{a \cos t\,dt}{a \sin t \cdot a \cos t} \\
&= \int \frac{dt}{a \sin t} \\
&= \frac{1}{a} \int \csc t\,dt \\
&= \frac{1}{a} \ln \left| \tan \frac{t}{2} \right| + C\\
&= \frac{1}{a} \ln \left| \frac{a - \sqrt{a^2 - x^2}}{x} \right| + C
\end{aligned}
$$






### c)  $\displaystyle\int \frac{dx}{x^2\sqrt{1+x^2}}$

**解：**

令 $ x = \tan t $  
则 $ dx = \frac{dt}{\cos^2 t} $

$$
\begin{aligned}
\text{原式} &= \int \frac{\cos t}{\sin^2 t} \, dt \\
&= -\frac{1}{\sin t} + C \\
&= -\frac{1}{\sin t} + C\\
&= -\frac{\sqrt{1 + x^2}}{x} + C
\end{aligned}
$$



### d)  $\displaystyle\int \frac{\sqrt{x^2-9}}{x}dx$

**解：**

令 $ x = 3 \sec t $  
则 $ dx = 3 \sec t \tan t\,dt $

$$
\begin{aligned}
\text{原式} &= \int 3 \tan^2 t\,dt \\
&= 3 \int (\sec^2 t - 1)\,dt \\
&= 3(\tan t - t) + C\\
&= 3 \left( \frac{\sqrt{x^2 - 9}}{3} - \arccos\left( \frac{3}{x} \right) \right) + C\\
&= \sqrt{x^2 - 9} - 3 \arccos\left( \frac{3}{x} \right) + C
\end{aligned}
$$



### e)  $\displaystyle\int \frac{x^2}{\sqrt{a^2-x^2}}dx \quad (a>0)$

**解：**

令 $ x = a \sin t $  
则 $ dx = a \cos t\,dt $

$$
\begin{aligned}
\text{原式} &= \int a^2 \sin^2 t\,dt \\
&= a^2 \int \sin^2 t\,dt \\
&= a^2 \int \frac{1 - \cos 2t}{2}\,dt \\
&= \frac{a^2}{2} \left( t - \frac{\sin 2t}{2} \right) + C\\
&= \frac{a^2}{2} \left( \arcsin\left( \frac{x}{a} \right) - \frac{1}{2} \cdot \frac{2x \sqrt{a^2 - x^2}}{a^2} \right) + C \\
&= \frac{a^2}{2} \arcsin\left( \frac{x}{a} \right) - \frac{x}{2} \sqrt{a^2 - x^2} + C
\end{aligned}
$$



### f)  $\displaystyle\int \frac{dx}{1+\sqrt{1-x^2}}$

**解：**

$$
\begin{aligned}
\text{原式} &= \int \frac{1 - \sqrt{1 - x^2}}{x^2} \, dx \\
&= -\frac{1}{x} + \frac{\sqrt{1 - x^2}}{x} + C
\end{aligned}
$$





## 6. 求下列不定积分（分部积分法比较适合）

### a)  $\displaystyle\int xe^{2x}dx$

**解：**
令 $ u = x $, $ dv = e^{2x} dx $  
则 $ du = dx $, $ v = \frac{1}{2} e^{2x} $

$$
\begin{aligned}
\text{原式} &= \frac{1}{2} x e^{2x} - \frac{1}{2} \int e^{2x} dx \\
&= \frac{1}{2} x e^{2x} - \frac{1}{2} \cdot \frac{1}{2} e^{2x} + C \\
&= \frac{1}{2} x e^{2x} - \frac{1}{4} e^{2x} + C \\
&= \frac{1}{4} e^{2x} (2x - 1) + C
\end{aligned}
$$





### b)  $\displaystyle\int \arctan xdx$

**解：**
令 $ u = \arctan x $, $ dv = dx $  
则 $ du = \frac{1}{1 + x^2} dx $, $ v = x $

$$
\begin{aligned}
\text{原式} &= x \arctan x - \int \frac{x}{1 + x^2} dx \\
&= x \arctan x - \frac{1}{2} \ln(1 + x^2) + C
\end{aligned}
$$





### c)  $\displaystyle\int x^2\arctan xdx$

**解：**
令 $ u = \arctan x $, $ dv = x^2 dx $  
则 $ du = \frac{1}{1 + x^2} dx $, $ v = \frac{1}{3} x^3 $
$$
\begin{aligned}
\text{原式} &= \frac{1}{3} x^3 \arctan x - \frac{1}{3} \int \frac{x^3}{1 + x^2} dx \\
&= \frac{1}{3} x^3 \arctan x - \frac{1}{3} \int \left( x - \frac{x}{1 + x^2} \right) dx \\
&= \frac{1}{3} x^3 \arctan x - \frac{1}{3} \left( \frac{x^2}{2} - \frac{1}{2} \ln(1 + x^2) \right) + C \\
&= \frac{1}{3} x^3 \arctan x - \frac{1}{6} x^2 + \frac{1}{6} \ln(1 + x^2) + C
\end{aligned}
$$




### d)  $\displaystyle\int x^2\ln xdx$

**解：**
令 $ u = \ln x $, $ dv = x^2 dx $  
则 $ du = \frac{1}{x} dx $, $ v = \frac{1}{3} x^3 $

$$
\begin{aligned}
\text{原式} &= \frac{1}{3} x^3 \ln x - \frac{1}{3} \int x^2 dx \\
&= \frac{1}{3} x^3 \ln x - \frac{1}{3} \cdot \frac{x^3}{3} + C \\
&= \frac{1}{3} x^3 \ln x - \frac{x^3}{9} + C
\end{aligned}
$$




### e)  $\displaystyle\int e^{-2x}\sin \frac{x}{2}dx$

**解：**
令 $ u = \sin \frac{x}{2} $, $ dv = e^{-2x} dx $  
则 $ du = \frac{1}{2} \cos \frac{x}{2} dx $, $ v = -\frac{1}{2} e^{-2x} $
$$
\begin{aligned}
\text{原式} &= -\frac{1}{2} e^{-2x} \sin \frac{x}{2} + \frac{1}{4} \int e^{-2x} \cos \frac{x}{2} dx
\end{aligned}
$$

对 $ \displaystyle\int e^{-2x} \cos \frac{x}{2} dx $ 再次积分：  
令 $ u = \cos \frac{x}{2} $, $ dv = e^{-2x} dx $  
则 $ du = -\frac{1}{2} \sin \frac{x}{2} dx $, $ v = -\frac{1}{2} e^{-2x} $
$$
\begin{aligned}
\int e^{-2x} \cos \frac{x}{2} dx &= -\frac{1}{2} e^{-2x} \cos \frac{x}{2} - \frac{1}{4} \int e^{-2x} \sin \frac{x}{2} dx \\
&= -\frac{1}{2} e^{-2x} \cos \frac{x}{2} - \frac{1}{4} \cdot \text{原式}
\end{aligned}
$$

代入原式：

$$
\begin{aligned}
\text{原式} &= -\frac{1}{2} e^{-2x} \sin \frac{x}{2} + \frac{1}{4} \left( -\frac{1}{2} e^{-2x} \cos \frac{x}{2} - \frac{1}{4} \text{原式} \right) \\
&= -\frac{1}{2} e^{-2x} \sin \frac{x}{2} - \frac{1}{8} e^{-2x} \cos \frac{x}{2} - \frac{1}{16} \text{原式}
\end{aligned}
$$

移项整理：

$$
\begin{aligned}
\text{原式} + \frac{1}{16} \text{原式} &= -\frac{1}{2} e^{-2x} \sin \frac{x}{2} - \frac{1}{8} e^{-2x} \cos \frac{x}{2} \\
\frac{17}{16} \text{原式} &= -\frac{1}{2} e^{-2x} \sin \frac{x}{2} - \frac{1}{8} e^{-2x} \cos \frac{x}{2} \\
\text{原式} &= \frac{16}{17} \left( -\frac{1}{2} e^{-2x} \sin \frac{x}{2} - \frac{1}{8} e^{-2x} \cos \frac{x}{2} \right) \\
&= -\frac{8}{17} e^{-2x} \sin \frac{x}{2} - \frac{2}{17} e^{-2x} \cos \frac{x}{2} + C \\
&= -\frac{2}{17} e^{-2x} \left( 4 \sin \frac{x}{2} + \cos \frac{x}{2} \right) + C
\end{aligned}
$$



### f)  $\displaystyle\int \frac{\arcsin x}{\sqrt{1-x}}dx$

**解：**

令 $ u = \arcsin x $, $ dv = \frac{dx}{\sqrt{1 - x}} $  
则 $ du = \frac{1}{\sqrt{1 - x^2}} dx $, $ v = -2 \sqrt{1 - x} $
$$
\begin{aligned}
\text{原式} &= -2 \arcsin x \cdot \sqrt{1 - x} + 2 \int \frac{\sqrt{1 - x}}{\sqrt{1 - x^2}} dx \\
&= -2 \arcsin x \cdot \sqrt{1 - x} + 2 \int \frac{\sqrt{1 - x}}{\sqrt{(1 - x)(1 + x)}} dx \\
&= -2 \arcsin x \cdot \sqrt{1 - x} + 2 \int \frac{1}{\sqrt{1 + x}} dx \\
&= -2 \arcsin x \cdot \sqrt{1 - x} + 2 \cdot 2 \sqrt{1 + x} + C \\
&= -2 \arcsin x \cdot \sqrt{1 - x} + 4 \sqrt{1 + x} + C
\end{aligned}
$$





### g)  $\displaystyle\int \ln(x+\sqrt{1+x^2})dx$

**解：**

令 $ u = \ln(x + \sqrt{1 + x^2}) $, $ dv = dx $  
则 $ du = \frac{dx}{\sqrt{1 + x^2}} $, $ v = x $

$$
\begin{aligned}
\text{原式} &= x \ln(x + \sqrt{1 + x^2}) - \int \frac{x}{\sqrt{1 + x^2}} dx \\
&= x \ln(x + \sqrt{1 + x^2}) - \sqrt{1 + x^2} + C
\end{aligned}
$$




### h)  $\displaystyle\int \frac{\ln(\cos x)}{\cos^2 x}dx$

**解：**
令 $ u = \ln(\cos x) $, $ dv = \sec^2 x\,dx $  
则 $ du = -\tan x\,dx $, $ v = \tan x $
$$
\begin{aligned}
\text{原式} &= \tan x \cdot \ln(\cos x) + \int \tan^2 x\,dx \\
&= \tan x \cdot \ln(\cos x) + \int (\sec^2 x - 1)\,dx \\
&= \tan x \cdot \ln(\cos x) + \tan x - x + C
\end{aligned}
$$




### i)  $\displaystyle\int \sin x \ln(\tan x)dx$

**解：** 
令 $ u = \ln(\tan x) $, $ dv = \sin x\,dx $  
则 $ du = \frac{dx}{\sin x \cos x} $, $ v = -\cos x $

$$
\begin{aligned}
\text{原式} &= -\cos x \cdot \ln(\tan x) + \int \frac{\cos x}{\sin x \cos x}\,dx \\
&= -\cos x \cdot \ln(\tan x) + \int \frac{1}{\sin x}\,dx \\
&= -\cos x \cdot \ln(\tan x) + \int \csc x\,dx \\
&= -\cos x \cdot \ln(\tan x) + \ln \left| \tan \frac{x}{2} \right| + C
\end{aligned}
$$




### j)  $\displaystyle\int \frac{\arcsin x}{x^2}dx$

**解：**
令 $ u = \arcsin x $, $ dv = x^{-2} dx $  
则 $ du = \frac{1}{\sqrt{1 - x^2}} dx $, $ v = -\frac{1}{x} $
$$
\begin{aligned}
\text{原式} &= -\frac{\arcsin x}{x} + \int \frac{1}{x \sqrt{1 - x^2}} dx \\
&= -\frac{\arcsin x}{x} + \ln \left( \frac{1 + \sqrt{1 - x^2}}{x} \right) + C
\end{aligned}
$$




## 7. 求下列不定积分（有理分式展开或其它方法）

### a)  $\displaystyle\int \frac{dx}{x^2-2x+2}$

**解：**
$$
\begin{aligned}
\text{原式} &= \int \frac{dx}{(x - 1)^2 + 1} \\
&= \arctan(x - 1) + C
\end{aligned}
$$




### b)  $\displaystyle\int \frac{x+1}{x^2-3x+2}dx$

**解：**
$$
\begin{aligned}
\text{原式} &= \int \frac{x + 1}{(x - 1)(x - 2)} dx \\
&= \int \left( \frac{-2}{x - 1} + \frac{3}{x - 2} \right) dx \\
&= -2 \ln |x - 1| + 3 \ln |x - 2| + C
\end{aligned}
$$




### c)  $\displaystyle\int \frac{2x+3}{(x^2-1)(x^2+1)}dx$

**解：**
$$
\begin{aligned}
\text{原式} &= \int \left( \frac{1}{2(x - 1)} - \frac{1}{2(x + 1)} + \frac{1}{x^2 + 1} \right) dx \\
&= \frac{1}{2} \ln \left| \frac{x - 1}{x + 1} \right| + \arctan x + C
\end{aligned}
$$




### d)  $\displaystyle\int \frac{x^5+x^4-8}{x^3+x}dx$

**解：**
$$
\begin{aligned}
\text{原式} &= \int \left( x^2 + x - 1 - \frac{8}{x} + \frac{x}{x^2 + 1} \right) dx \\
&= \frac{1}{3} x^3 + \frac{1}{2} x^2 - x - 8 \ln |x| + \frac{1}{2} \ln(1 + x^2) + C
\end{aligned}
$$





### e)  $\displaystyle\int \frac{x^4+1}{(x-1)(x^2+1)}dx$

**解：**
$$
\begin{aligned}
\text{原式} &= \int \left( x + 1 + \frac{1}{x - 1} - \frac{x - 1}{x^2 + 1} \right) dx \\
&= \frac{1}{2} x^2 + x + \ln |x - 1| - \frac{1}{2} \ln(1 + x^2) + C
\end{aligned}
$$




### f)  $\displaystyle\int \frac{dx}{(x-1)(x+1)^2}$

**解：**
$$
\begin{aligned}
\text{原式} &= \int \left( \frac{1}{4(x - 1)} - \frac{1}{4(x + 1)} - \frac{1}{2(x + 1)^2} \right) dx \\
&= \frac{1}{4} \ln |x - 1| - \frac{1}{4} \ln |x + 1| + \frac{1}{2(x + 1)} + C
\end{aligned}
$$




## 8. 利用定积分的几何意义计算下列积分

### a)  $\displaystyle\int_{-1}^1 |x|dx$

**解：**
$$
\text{原式} = 2 \times 1 \times \frac{1}{2} = 1
$$



### b)  $\displaystyle\int_{-\pi}^{\pi} \sin xdx$

**解：**
$$
\text{原式} = 0
$$



## 9. 已知  $\displaystyle\int_{0}^{\pi} \sin x dx = 2$，计算极限

$$
\lim_{n \to \infty} \frac{1}{n} \left[ \sin \frac{\pi}{n} + \sin \frac{2\pi}{n} + \cdots + \sin \frac{(n-1)\pi}{n} \right]
$$

**解：**
$$
\begin{aligned}
\text{原式} &= \lim_{n \to \infty} \frac{1}{n} \sum_{k=1}^{n-1} \sin \frac{k\pi}{n} \\
&= \frac{1}{\pi} \lim_{n \to \infty} \frac{\pi}{n} \sum_{k=1}^{n-1} \sin \left( \frac{k\pi}{n} \right) \\
&= \frac{1}{\pi} \int_0^\pi \sin x\,dx \\

&= \frac{2}{\pi}
\end{aligned}
$$




## 10. 已知  $\displaystyle\int_{1}^{2} \ln x dx = 2 \ln 2 - 1$，求极限

$$
\lim_{n \to \infty} \frac{\sqrt[n]{(n+1)(n+2) \cdots (2n)}}{n}
$$

**解：**
令原式 $ = t $
$$
\begin{aligned}
\ln t &= \lim_{n \to \infty} \frac{1}{n} \sum_{k=n+1}^{2n} \ln \frac{k}{n} \\
&= \int_1^2 \ln x\,dx \\
&= \left[ x \ln x - x \right]_1^2 \\
&= (2 \ln 2 - 2) - (0 - 1) \\
&= 2 \ln 2 - 1
\end{aligned}
$$

$$
\text{原式} = t = \frac{4}{e}
$$






## 11. 设 $ f, g \in C[a, b] $，证明：若 $f(x) \geq g(x) $($ x \in [a, b] $)，且$ f(x) $ 不恒为 $ g(x) $，则$\displaystyle\int_{a}^{b} f(x) dx > \displaystyle\int_{a}^{b} g(x) dx$

**解：**
令 $ h(x) = f(x) - g(x) \geq 0 $，$ x \in [a, b] $

存在 $ x_0 $，使得 $ h(x_0) > 0 $

又 $ h(x) \in C[a, b] $

则存在区间 $ [x_0 - \delta, x_0 + \delta] \subset [a, b] $，  
使得 $ h(x) > 0 $

$$
\int_a^b h(x)\,dx = \int_a^b [f(x) - g(x)]\,dx > 0
$$

$$
\Rightarrow \int_a^b f(x)\,dx > \int_a^b g(x)\,dx
$$




## 12. 比较下列各组中积分的大小. 

### a)  $\displaystyle\int_{0}^{\frac{\pi}{2}} \sin^{2} x dx$与  $\displaystyle\int_{0}^{\frac{\pi}{2}} \sin^{4} x dx$

**解：**
$$
0 \leq \sin x \leq 1
$$
$$
\sin^4 x \leq \sin^2 x
$$
$$
\int_0^{\frac{\pi}{2}} \sin^4 x\,dx < \int_0^{\frac{\pi}{2}} \sin^2 x\,dx
$$



### b)  $\displaystyle\int_{1}^{e} \ln x dx$，  $\displaystyle\int_{1}^{e} (\ln x)^{2} dx$，  $\displaystyle\int_{1}^{e} \ln (x^{2}) dx$

**解：**
$$
\ln x \in [0, 1] \quad \text{故} \quad (\ln x)^2 \leq \ln x
$$
$$
\text{又} \quad \ln(x^2) = 2 \ln x
$$
$$
(\ln x)^2 \leq \ln x \leq \ln(x^2)
$$
$$
\int_1^e (\ln x)^2 dx < \int_1^e \ln x\,dx < \int_1^e \ln(x^2)\,dx
$$




## 13. 证明不等式  $\frac{1}{2} < \displaystyle\int_{\frac{\pi}{4}}^{\frac{\pi}{2}} \frac{\sin x}{x} dx < \frac{\sqrt{2}}{2}$

**解：**
$$
\int_{\frac{\pi}{4}}^{\frac{\pi}{2}} \frac{\sin x}{x} dx < \int_{\frac{\pi}{4}}^{\frac{\pi}{2}} \frac{dx}{x} = \ln 2 < \frac{\sqrt{2}}{2}
$$

$$
\int_{\frac{\pi}{4}}^{\frac{\pi}{2}} \frac{\sin x}{x} dx > \frac{2}{\pi} \left( \frac{\pi}{2} - \frac{\pi}{4} \right) = \frac{1}{2}
$$

故成立




## 14. 求下列极限

### a)  $\displaystyle\lim_{n \to \infty} \displaystyle\int_{0}^{\frac{1}{2}} \frac{x^{n}}{1+x} dx$

**解：** 
$$
0 < \lim_{n \to \infty} \int_0^{\frac{1}{2}} \frac{x^n}{1 + x}\,dx < \lim_{n \to \infty} \int_0^{\frac{1}{2}} x^n\,dx = \lim_{n \to \infty} \frac{\left( \frac{1}{2} \right)^{n+1}}{n+1} = 0
$$

故原式 $ = 0 $



### b)  $\displaystyle\lim_{n \to \infty} \displaystyle\int_{n^{2}}^{n^{2}+n} \frac{1}{\sqrt{x}} e^{-\frac{1}{x}} dx$

**解：**
$$
\text{原式} = \lim_{n \to \infty} \int_{n^2}^{n^2 + n} \frac{dx}{\sqrt{x}}
$$
$$
= \lim_{n \to \infty} 2 \left( \sqrt{n^2 + n} - n \right)
$$
$$
= \lim_{n \to \infty} \frac{2n}{\sqrt{n^2 + n} + n} = 1
$$




## 15. 求下列函数 $ y = y(x) $ 的导数 $ \frac{dy}{dx} $

### a)  $y = \displaystyle\int_{\cos x}^{\sin x} e^{-t^{2}} dt$

**解：**
$$
y' = e^{-\sin^2 x} \cos x + e^{-\cos^2 x} \sin x
$$





### b)  $y = \left( \displaystyle\int_{0}^{\sqrt{x}} \ln (1+t^{2}) dt \right)^{2}$

**解：**
$$
y' = 2 \left( \int_0^{\sqrt{x}} \ln(1 + t^2)\,dt \right) \cdot \frac{\ln(1 + x)}{2\sqrt{x}}
$$
$$
= \frac{\ln(1 + x)}{\sqrt{x}} \int_0^{\sqrt{x}} \ln(1 + t^2)\,dt
$$




### c)  $\displaystyle\int_{0}^{xy} e^{t} dt + \displaystyle\int_{0}^{y} \sin t dt = 0$

**解：**
$$
e^{xy} (y + x y') + \sin y + y' = 0
$$
$$
 y' = -\frac{y e^{xy}}{x e^{xy} + \sin y}
$$



### d)  
$$
\begin{cases}
x = \int_{1}^{t} \ln u du \\
y = \int_{1}^{t} u \ln u du 
\end{cases}
$$

**解：**
$$
\frac{dy}{dx} = \frac{t \ln t}{\ln t} = t
$$




## 16. 求下列极限

### a)  $\displaystyle\lim_{x \to 0} \frac{\displaystyle\int_{cosx}^1 e^{-t^2} dt}{x^2}$

**解：**
$$
\text{原式} = \lim_{x \to 0} \frac{e^{-\cos^2 x} \sin x}{2x}
$$
$$
= \lim_{x \to 0} \frac{e^{-\cos^2 x}}{2} = \frac{1}{2e}
$$




### b)  $\displaystyle\lim_{x \to 0} \frac{\displaystyle\int_0^x \ln(1+t^2) dt}{\ln \frac{\sin x}{x}}$

**解：**
$$
\text{原式} = \lim_{x \to 0} \frac{\ln(1 + x^2)}{\frac{\cos x}{\sin x} - \frac{1}{x}}
$$
$$
= \lim_{x \to 0} \frac{x^2 + o(x^2)}{-\frac{x}{3} + o(x)} = 0
$$





## 17. 设函数  
$$
f(x) = \begin{cases} 
x^2, & 0 \leq x < 1 \\ 
x - 2, & 1 \leq x \leq 2 
\end{cases}
$$
## 求  $\Phi(x) = \displaystyle\int_0^x f(t)dt$在$[0, 2]$ 上的表达式. 

**解：**
当 $ x \in [0, 1) $ 时，  
$$
\phi(x) = \frac{1}{3} x^3
$$

当 $ x \in [1, 2] $ 时，  
$$
\phi(x) = \frac{1}{3} + \int_1^x (t - 2)\,dt = \frac{1}{2}x^2 - 2x + \frac{11}{6}
$$


$$
\phi(x) = 
\begin{cases}
\dfrac{1}{3} x^3, & x \in [0, 1) \\
\dfrac{1}{2}x^2 - 2x + \dfrac{11}{6}, & x \in [1, 2]
\end{cases}
$$




## 18. 设函数 $ f \in C[a, b] $，且 $ f(x) > 0$ ($ x \in [a, b] $)，记  $F(x) = \displaystyle\int_a^x f(t)dt + \displaystyle\int_b^x \frac{dt}{f(t)} \quad (x \in [a, b])$
## 证明：
### a)  $F'(x) \geq 2$

**解：**
$$
F'(x) = f(x) + \frac{1}{f(x)} \geq 2
$$



### b) 方程$ F(x) = 0 $ 在区间 $ (a, b) $ 内有且仅有一根. 

**解：**
$ F(x) $ 连续，$ F'(x) > 0 $，故 $ F(x) $ 单调增加。  

又 $ F(a) < 0 $，$ F(b) > 0 $，  
故方程 $ F(x) = 0 $ 在区间 $ (a, b) $ 内有且仅有一根.



## 19. 设函数 $ f \in C[a, b] $，且 $ f(x) > 0 $ ($ x \in [a, b]$). 证明：至少存在一个点 $\xi \in [a, b]$，使得  $\displaystyle\int_a^\xi f(x)dx = \displaystyle\int_\xi^b f(x)dx = \frac{1}{2} \displaystyle\int_a^b f(x)dx$

**解：**
令 $ F(x) = \displaystyle\int_a^x f(t)\,dt $

则 $ F(a) = 0 $，$ F(b) = \displaystyle\int_a^b f(t)\,dt > 0 $

又 $ f(x) > 0 $，故 $ F(x) $ 单调增加

令 $ k = \frac{1}{2} \displaystyle\int_a^b f(t)\,dt $

存在 $ \xi \in [a, b] $，使得 $ F(\xi) = \displaystyle\int_a^\xi f(t)\,dt = k $

$$
\int_\xi^b f(t)\,dt = \int_a^b f(t)\,dt - \int_a^\xi f(t)\,dt = k
$$

故成立




## 20. 设函数 $ f \in C[0, 1] \cap D(0, 1) $，且  $3 \displaystyle\int_0^{\frac{1}{3}} e^{1-x^2} f(x)dx = f(1)$
## 证明：至少存在一点 $\xi \in (0, 1)$，使得$f'(\xi) = 2\xi f(\xi) $. 

**解：**

令 $ F(x) = e^{-x^2} f(x) $

则 $ F(1) = e^{-1} f(1) $

故  
$$
3 \int_0^{\frac{1}{3}} f(x)\,dx = e^{-1} f(1) = F(1)
$$

又存在 $ \eta \in \left[0, \frac{1}{3}\right] $，使得  
$$
\int_0^{\frac{1}{3}} f(x)\,dx = \frac{1}{3} F(\eta)
$$

故  
$$
F(\eta) = F(1)
$$

在区间 $[\eta, 1]$ 上，$ F(\eta) = F(1) $

故存在 $ \xi \in (\eta, 1) \subset (0,1) $，使得  
$$
F'(\xi) = 0
$$

代入，得  
$$
f'(\xi) = 2\xi f(\xi)
$$



## 21. 设函数  $S(x) = \displaystyle\int_0^x |\cos t| dt$

### (a) 当 $( n \in \mathbb{N}_+ $，且 $( n\pi \leq x < (n+1)\pi$ 时，证明：$ 2n \leq S(x) < 2(n+1) $. 

**解：** 
$$
S(x) = \int_0^x |\cos t|\,dt = \sum_{k=0}^{n-1} \int_{k\pi}^{(k+1)\pi} |\cos t|\,dt + \int_{n\pi}^x |\cos t|\,dt = 2n + \int_{n\pi}^x |\cos t|\,dt
$$

由于 $ \displaystyle\int_{n\pi}^x |\cos t|\,dt \in [0, 2) $

故  
$$
2n \leq S(x) < 2(n+1)
$$



### (b) 求极限  $\displaystyle\lim_{x \to +\infty} \frac{S(x)}{x}$

**解：**
$$
2n \leq S(x) < 2(n+1)
$$

两边同除以 $ x $，注意 $ x \in [n\pi, (n+1)\pi) $，所以  
$$
\frac{2n}{(n+1)\pi} \leq \frac{S(x)}{x} \leq \frac{2(n+1)}{n\pi}
$$

当 $ x \to \infty $ 时，$ n \to \infty $，夹逼得：  
$$
\lim_{x \to \infty} \frac{S(x)}{x} = \frac{2}{\pi}
$$





## 22. 证明：$\displaystyle\int_0^x f(t)(x-t)dt = \displaystyle\int_0^x \left( \displaystyle\int_0^t f(x)dx \right) dt$

**解：**
令 $ x - t = \displaystyle\int_t^x 1\,ds $

$$
\int_0^x f(t)(x - t)\,dt = \int_0^x \left( \int_t^x f(t)\,ds \right) dt
$$
$$
= \int_0^x \left( \int_0^s f(t)\,dt \right) ds
$$
$$
= \int_0^x \left( \int_0^t f(s)\,ds \right) dt
$$




## 23. 设非负函数 $ f \in R[a, b] $，证明不等式：
$$
\left( \int_a^b f(x) \cos x dx \right)^2 + \left( \int_a^b f(x) \sin x dx \right)^2 \leq \left( \int_a^b f(x) dx \right)^2
$$
**提示**：利用柯西-施瓦茨不等式. 

**解：**
左边 $ \leq \left( \displaystyle\int_a^b f(x) \sqrt{\cos^2 x + \sin^2 x} \,dx \right)^2 $

​	$= \left( \displaystyle\int_a^b f(x)\,dx \right)^2$

故成立




## 24. 设 $ f \in C[a, b]$，且$ f(a) $ 和 $ f(b) $ 分别是 $ f(x) $ 在 $[a, b]$ 上最大值和最小值.   证明：至少存在一点$\xi \in [a, b]$，使得  $\displaystyle\int_a^b f(x) dx = f(a)(\xi - a) + f(b)(b - \xi)$

**提示**：先利用积分中值公式，然后构造函数并利用零点定理之类. 

**解：**
令 $ F(\xi) = f(a)(\xi - a) + f(b)(b - \xi) - \displaystyle\int_a^b f(x)\,dx $

则  
$$
F(a) = f(b)(b - a) - \int_a^b f(x)\,dx \leq 0
$$

$$
F(b) = f(a)(b - a) - \int_a^b f(x)\,dx \geq 0
$$

故存在 $ \xi \in [a, b] $，使得 $ F(\xi) = 0 $




## 25. 设 $ f \in C[a, b] \cap D(a, b) $)，且 $ f'(x) \geq 0 (x \in (a, b)) $，求证$\displaystyle\int_a^b xf(x) dx \geq \frac{a + b}{2} \displaystyle\int_a^b f(x) dx$

**提示**：能否让 $ b$ 动起来，从而转变为对函数求导以判别单调性的问题？

**解：**
令 $ g(x) = x - \frac{a+b}{2} $

则  
$$
\int_a^b x f(x)\,dx - \frac{a+b}{2} \int_a^b f(x)\,dx = \int_a^b g(x) f(x)\,dx
$$

当 $ x \in \left[a, \frac{a+b}{2}\right] $ 时，$ g(x) \leq 0 $，且 $ f(x) \leq f\left(\frac{a+b}{2}\right) $

当 $ x \in \left[\frac{a+b}{2}, b\right] $ 时，$ g(x) \geq 0 $，且 $ f(x) \geq f\left(\frac{a+b}{2}\right) $

故  
$$
\int_a^b g(x) f(x)\,dx \geq \int_a^b g(x) f\left(\frac{a+b}{2}\right)\,dx = f\left(\frac{a+b}{2}\right) \int_a^b g(x)\,dx
$$

又  
$$
\int_a^b g(x)\,dx = \int_a^b \left(x - \frac{a+b}{2}\right)\,dx = \frac{b^2 - a^2}{2} - \frac{a+b}{2}(b - a) = 0
$$

故  
$$
\int_a^b g(x) f(x)\,dx \geq 0
$$

因此  
$$
\int_a^b x f(x)\,dx \geq \frac{a+b}{2} \int_a^b f(x)\,dx
$$

