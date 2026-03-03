# 第3章 导数与微分
## 3.1 导数的概念
1、设 $f(x)$ 满足 $f(0)=0$，且 $f^{'}(0)$ 存在，则 $\displaystyle \lim_{x \to 0} \frac{f(1-\sqrt{\cos x})}{\ln (1 - x \sin x)} =$ _____.
解：
原式 $= \displaystyle \lim_{x \to 0} \frac{f(1-\sqrt{\cos x}) - f(0)}{(1-\sqrt{\cos x}) - 0} \cdot \displaystyle \lim_{x \to 0} \frac{1-\sqrt{\cos x}}{\ln (1 - x \sin x)} = f^{'}(0) \cdot \displaystyle \lim_{x \to 0} \frac{1-\sqrt{\cos x}}{\ln (1 - x \sin x)} = -\frac{1}{4} f^{'}(0)$   

## 3.2 导数的四则运算与反函数的导数
### 一、导数的四则运算
### 二、反函数的求导法则
1、已知 $f^{'}(x) = A e^x$（ $A$ 为正常数），则 $f(x)$ 的反函数的二阶导数为____.
解：设 $y = f(x)$，则

$$
\frac{dx}{dy} = \frac{1}{f'(x)}\\
\frac{d^2 x}{dy^2} = \frac{d}{dy}\left( \frac{dx}{dy} \right) = \frac{d}{dx}\left( \frac{1}{f'(x)} \right) \cdot \frac{dx}{dy} = -\frac{f''(x)}{\left[ f'(x) \right]^2} \cdot \frac{1}{f'(x)} = -\frac{1}{A^2 e^{2x}}
$$

## 3.3 复合函数的求导法——链式法则
## 3.4 参数式函数的导数
## 3.5 高阶导数
## 3.6 微分
### 一、微分的概念与运算
### 二、一阶微分的形式不变性
### 三、利用微分作近似计算和误差估计