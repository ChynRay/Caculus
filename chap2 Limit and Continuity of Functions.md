# 第2章 函数的极限与连续性  
## 2.1 函数的极限
## 2.2 连续函数
## 2.3 无穷小和无穷大
1、已知 $a > 0, b > 0$ , 求 $\displaystyle \lim_{x \to +\infty} x \left( a^{\frac{1}{x}} - b^{\frac{1}{x}} \right)$。
解：令 $t = \frac{1}{x}$，原式变为： $\displaystyle \lim_{t \to 0^+} \frac{a^t - b^t}{t}$。
等价无穷小： $x \to 0$ 时，$a^x - 1 \sim x \ln a$。
经过变化可得答案为： $\ln \frac{a}{b}$。

2、计算 $\displaystyle \lim_{x \to +\infty} \left[ \sin \ln(1+x) - \sin \ln x \right]$  
**正弦和差化积**：
 $$
\sin A + \sin B = 2\sin\frac{A+B}{2}\cos\frac{A-B}{2} \\
\sin A - \sin B = 2\cos\frac{A+B}{2}\sin\frac{A-B}{2}
 $$
**余弦和差化积**：
 $$
\cos A + \cos B = 2\cos\frac{A+B}{2}\cos\frac{A-B}{2} \\
\cos A - \cos B = -2\sin\frac{A+B}{2}\sin\frac{A-B}{2}
 $$
经过化简可得答案为： $0$

## 2.4 有限闭区间上连续函数的性质
1、设 $f(x)$ 在闭区间 $[a,b]$ 上连续，求证：
（1）若 $a_1, a_2$ 为满足 $a_1 + a_2 = 1$ 的正实数，则至少存在一点 $\xi \in [a,b]$ , 使得
 $$
a_1 f(a) + a_2 f(b) = f(\xi);
 $$
（2）对任意正实数 $k_1, k_2$，至少存在一点 $\eta \in [a,b]$，使得
 $$
k_1 f(a) + k_2 f(b) = (k_1 + k_2) f(\eta).
 $$

证明：
（1）已知 $f(x)$ 在 $[a,b]$ 上连续，因此 $f(x)$ 在该区间上存在最大值 $M$ 和最小值 $m$，即
 $$
m \le f(a) \le M,\quad m \le f(b) \le M
 $$
又因为 $a_1, a_2 > 0$ 且 $a_1 + a_2 = 1$，所以
 $$
a_1 m + a_2 m \le a_1 f(a) + a_2 f(b) \le a_1 M + a_2 M = M(a_1 + a_2)
 $$
根据**介值定理**，至少存在一点 $\xi \in [a,b]$，使得
 $$
a_1 f(a) + a_2 f(b) = f(\xi)
 $$
（2） 对任意正实数 $k_1, k_2$，令
 $$
a_1 = \frac{k_1}{k_1 + k_2},\quad a_2 = \frac{k_2}{k_1 + k_2}
 $$
显然 $a_1, a_2 > 0$ 且 $a_1 + a_2 = 1$。
将其代入 (1) 的结论，可得
 $$
\frac{k_1}{k_1 + k_2} f(a) + \frac{k_2}{k_1 + k_2} f(b) = f(\eta)
 $$
两边同乘 $k_1 + k_2$，即得
 $$
k_1 f(a) + k_2 f(b) = (k_1 + k_2) f(\eta)
 $$
其中 $\eta \in [a,b]$。