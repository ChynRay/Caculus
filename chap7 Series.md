# 第7章 级数

## 7.1 级数的收敛性及基本性质

### 一、级数收敛的定义

### 二、收敛级数的基本性质

## 7.2 正项级数

### 一、正项级数的一般性判别法

### 二、正项级数的比较判别法

### 三、正项级数的比值判别法与根植判别法

1、判别 $\displaystyle \sum^{+\infty} _{n=1}\frac{a^nn!}{n^n}$ 的敛散性。

易得 $a\ne e$ 时，其敛散性的情况。  
当 $a = e$ 时
利用**斯特林公式:**  

$$
n! \sim \sqrt{2\pi n}(\frac{n}{e})^n
$$

易得其发散。

### 四、正项级数的积分判别法

## 7.3 一般项级数的敛散性判别

### 一、交错级数

1、判断级数 $\displaystyle \sum ^{+\infty}_{n=1} \sin (\pi \sqrt{n^2+1})$ 的敛散性。
解：
由于 $\sin (n\pi -\alpha)=(-1)^{n-1}\sin \alpha,$ 将原级数转换为交错级数的格式。  
通过放缩，易得其收敛。

### 二、级数的条件收敛与绝对收敛

### 三、阿贝尔判别法与狄利克雷判别法

1、判断 $\displaystyle \sum ^{+\infty}_{n=1}\frac{\sin n \centerdot \sin n^2}{n}$ 的敛散性。

解：  
**狄利克雷判别法：**  
设数列 ${a_n}$ 单调，且 $\displaystyle _{n \to +\infty}a_n=0,$ 级数 $\displaystyle \sum ^{+\infty}_{n=1}b_n$ 的部分和有界，则级数 $\displaystyle ^{+\infty}_{n=1}a_nb_n$ 收敛。

由**和积化差**将其变化，结合**狄利克雷判别法**，易得其为收敛。

### 四、绝对收敛级数的性质

## 7.4 幂级数及其和函数

### 一、幂级数及其收敛半径

1、设 $f(x) = \displaystyle ^{\infty}_{n=0} x^n,g(x)=\int ^x_0 f(t)dt$ ,则 $f(x)$ 与 $g(x)$ 的收敛域分别为（   ）。  

解：  
**和函数的逐项可积性**  
若幂级数的收敛半径为 $r$ ，则它的和函数 $S(x)$ 在 $(-r,r)$ 的任何有限子区间 $[a,b]$ 上都可积，且有

$$
\int^b_a S(x)dx = \int^b_a \displaystyle \sum^{+\infty}_{n=0}a_nx^ndx = \displaystyle \sum^{+\infty}_{n=0} \int^b_a a_nx^ndx.
$$

由此易得答案为 $(-1,1);[-1,1]$
### 二、幂级数的分析性质

### 三、幂级数的和函数

1、求幂级数 $\displaystyle \sum ^{+\infty}_{n=1}$ 的和函数。
解：
其收敛域为 $[-1,1),$ 记 $S(x)=\displaystyle \sum^{+\infty}_{n=1}\frac{x^n}{n},$ 则求导后得

$$
S^{'}(x)=\frac{1}{1-x}
$$

同时求积，易得答案为： $-\ln (1-x)$  
也可以 **先求积后求导**

## 7.5 函数的幂级数展开

### 一、泰勒级数

1、判别级数 $\displaystyle \sum ^{\infty} _{n=2} \ln [1+\frac{(-1)^n}{\sqrt{n}}]$ 的敛散性。

对其泰勒展开

$$
\ln [1+\frac{(-1)^n}{\sqrt{n}}]=\frac{(-1)^n}{\sqrt{n}}-\frac{1}{2n}+o(\frac{1}{n})
$$

因此其易得其为发散的。  

### 二、常见函数的幂级数展开

### 三、幂级数在近似计算中的应用

## 7.6 函数项级数的一致收敛性

### 一、函数项级数

### 二、函数项级数的一致收敛性

### 三、一致收敛级数的性质

## 7.7 函数的傅里叶级数

### 一、三角级数与三角函数系的正交性

### 二、周期为 $2\pi$ 的函数的傅里叶展开

1、设 $f(x) = \begin{cases} x,0 \le x \le \frac{1}{2}, \\ 2-2x,\frac{1}{2} \lt x \le 1,\end{cases} S(x) = \frac{a_0}{2}+\displaystyle \sum^{\infty}_{n=1} a_n\cos n\pi x,-\infty \lt x \lt +\infty,$ 其中  

$$
a_n=2\int ^1_0f(x)\cos n\pi x dx(n=0,1,2,\dots),
$$

则 $S(-\frac{5}{2}) =\__. $  

解：
**狄利克雷收敛定理：**  
$S(x)$ 收敛于点的 $\frac{左极限+右极限}{2}.$  
易得答案为： $\frac{3}{4}$

### 三、一般周期函数的傅里叶展开