# 第5章 不定积分

## 5.1 原函数与不定积分的概念

## 5.2 换元法和分部积分法

### 一、换元法

1、求不定积分： $\int \frac{\sin x}{a\cos x + b\sin x}dx$
解：
注意到： $b(a\cos x + b\sin x)-a(a\cos x + b\sin x)^{'} = (b^2+a^2)\sin x$
由此换元法易得答案为： $\frac{1}{a^2+b^2}(bx-a\ln |a\cos x + b\sin x|+C$

2、求不定积分： $\int \frac{dx}{(2x^2+1)\sqrt{x^2+1}}$ .
解：利用**三角变化**： $x=\tan t,t \in (-\frac{\pi}{2},\frac{\pi}{2})$  

$$
\begin{align*}​
\int \frac{dx}{(2x^2 + 1)\sqrt{x^2 + 1}} &= \int \frac{\sec^2 t dt}{(2\tan^2 t + 1)\sec t} \\​
&= \int \frac{\sec t dt}{2\tan^2 t + 1} \\​
&= \int \frac{\frac{1}{\cos t}}{\frac{2\sin^2 t + \cos^2 t}{\cos^2 t}} dt \\​
&= \int \frac{\cos t dt}{2\sin^2 t + \cos^2 t} \\​
&= \int \frac{\cos t dt}{\sin^2 t + 1}​
\end{align*}
$$

容易得到，答案为： $\arctan (\frac{x}{\sqrt{x^2+1}})+C.$  

### 二、分部积分法

## 5.3一些特殊被积函数的不定积分

### 一、有理函数的不定积分

1、求 $\int \frac{x^4}{(1+x^2)^2}dx$ .
解：

$$
\begin{align*}
\int \frac{x^4}{(1+x^2)^2}dx=\frac{1}{2} \int \frac{x^3}{(1+x^2)^2}d(1+x^2)=-\frac{1}{2} \int x^3 d\frac{1}{1+x^2}=-\frac{1}{2} \cdot \frac{x^3}{1+x^2}+\frac{3}{2} \int \frac{x^2}{1+x^2}dx=-\frac{x^3}{2(1+x^2)}+\frac{3}{2}x-\frac{3}{2}\arctan x +C
\end{align*}
$$

### 二、可有理化函数的不定积分

1、求 $\int \sqrt{\frac{x-a}{b-x}}dx,a \lt x \lt b$
解：
因为有恒等式 $\frac{x-a}{b-a}+\frac{b-x}{b-a} \equiv 1,$ 作变量替换： $\frac{x-a}{b-a}=\sin^2t,\frac{b-x}{b-a}=\cos^2t,t \in (0,\frac{\pi}{2}),$ 于是  

$$
\begin{align*}
\int \sqrt{\frac{x-a}{b-x}}dx &=2(b-a)\int \tan t \cos t \sin t dt \\
&=(b-a)\int (1-\cos 2t)dt \\
&=(b-a)(t-\sin t \cos t) + C \\
&=(b-a)\arcsin \sqrt{\frac{x-a}{b-a}} - \sqrt{(x-a)(b-x)} + C
\end{align*}
$$
