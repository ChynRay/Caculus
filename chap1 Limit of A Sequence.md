# 第1章 数列的极限
## 1.1数列
### 一、数列及其极限的概念
1、证明 $\displaystyle \lim_{n \to \infty}\sqrt[n]{n}=1$  
证明： $n\ge 2$时，假设 $\sqrt[n]{n}=a_n+1$  
此时，$n=(a_n+1)^n=1+na_n+\frac{n(n+1)}{2}a_n^2+\dots+a_n^n \gt \frac{n(n+1)}{2}a_n^2$  
即 $0 \lt a_n \lt \sqrt{\frac{2}{n+1}}$  
于是， $\forall \varepsilon \gt 0,\exist N= \text{max}\{2,[\frac{2}{\varepsilon^2}]+1\}$,当 $n \ge N$时，  
$|\sqrt[n]{n}-1|=a_n \lt \sqrt{\frac{2}{m-1}} \le \sqrt{\frac{2}{n-\frac{n}{2}}} =\frac{2}{\sqrt{n}} \lt \varepsilon $  
所以，$\displaystyle \lim_{n \to \infty}\sqrt[n]{n}=1$ 

### 二、收敛数列的性质与极限的四则运算法则
1、计算 $\displaystyle \lim_{n \to \infty}\frac{e^n-4^{n+1}}{2\centerdot4^n+5}$  
 $\displaystyle \lim_{n \to \infty}\frac{e^n-4^{n+1}}{2\centerdot4^n+5}$= $\displaystyle \lim_{n \to \infty}\frac{(\frac{e}{4})^n-4}{2+5\centerdot\frac{1}{4^n}}=-2$  

2、设 $x=f(x_n)$，则以下命题正确的是（）  
①若 $f(x)$单调增加，且 $x_1 \lt x_2$，则数列 ${x_n}$单调增加  
②若 $f(x)$单调增加，且 $x_1 \gt x_2$，则数列 ${x_n}$单调减小  
③若 $f(x)$单调减小，且 $x_1 \lt x_2$，则数列 ${x_n}$单调增加  
④若 $f(x)$单调减小，且 $x_1 \gt x_2$，则数列 ${x_n}$单调减小  
易得 $A$

3、利用夹逼定理求 $\displaystyle \lim_{n \to \infty}\frac{1 \centerdot 3 \centerdot 5 \dots (2n-1)}{2 \centerdot 4 \centerdot 6 \dots (2n)}$  
解：设待计算数列为 $A_n$，则易得 $A_n \gt 0$  
且 $A_n \lt \frac{2 \centerdot 4 \centerdot 6 \dots (2n)}{3 \centerdot 5 \dots (2n+1) }$ 
所以 $A_n^2 \lt \frac{1}{2n+1}$ ,$A_n \lt \frac{1}{\sqrt{2n+1}}$
由夹逼定理易得 $\displaystyle \lim_{n \to \infty}\frac{1 \centerdot 3 \centerdot 5 \dots (2n-1)}{2 \centerdot 4 \centerdot 6 \dots (2n)}=0$  

4、利用夹逼定理证明 $\displaystyle \lim_{n \to \infty}(\frac{1}{n}+\frac{1}{n+1}+\dots +\frac{1}{2n})=\text{ln2}$。  
证明：因为函数 $f(x)=\frac{1}{x}$ 在 $(0,+ \infty)$上严格递减，对于 $k \in N$，有：$\int_{k}^{k+1}\frac1x dx \le \frac1k \le \int_{k-1}^{k}\frac1x dx$。  
因此 $\sum_{k=n}^{2n}\int_{k}^{k+1}\frac1x dx \le \sum_{k=n}^{2n}\frac1k \le \sum_{k=n}^{2n}\int_{k-1}^{k}\frac1x dx$。
由夹逼定理易证。


### 三、无穷大数列

## 1.2确界原理
1、对于 $a\in \mathbb{R}$，证明： $\displaystyle \lim_{n\to \infty}\frac{a^n}{n!}=0$  
证明：先证明 $\displaystyle \lim_{n\to \infty}\frac{|a|^n}{n!}=0$  
当 $a=0$时，显然成立  
当 $a\ne 0$时，令 $b_n=\frac{|a|^n}{n!}$，则 $\frac{b_{n+1}}{b_n}=\frac{|a|}{n+1}$  
当 $n \ge |a|$时， $\frac{b_{n+1}}{b_n}=\frac{|a|}{n+1} \lt 1$  
因此其在有限项后单调递减，易得 $b_n \gt 0$，其有下界，因此收敛。  
假设 $\displaystyle \lim_{n\to \infty}b_n=b$  
则 $b=\frac{|a|}{n+1}b_n$，易得 $b=0$  
 $\displaystyle \lim_{n\to \infty}b_n=0$  
又因为 $-b_n \le \frac{a^n}{n!} \le b_n$，由夹逼定理可得  
 $\displaystyle \lim_{n\to \infty}\frac{a^n}{n!}=0$ 

## 1.3柯西准则
