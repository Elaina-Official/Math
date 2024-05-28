# 高考数学常用技巧

***笔者注：笔者能力不足，文中可能出现多出错误，请读者注意辨别。另外，此文仅供拓展学习使用，不建议备考高考的学生过于追求此文所述内容。***

## 常用数据

以下数据常用于估算 $ , $ 一般情况下只需记忆至小数点后3或4位即可.

-  $ \pi=3.141,592,6\cdot\cdot\cdot\  $ 
-  $ e=2.718,281,8\cdot\cdot\cdot\  $ 
-  $ e^2=7.389,056,0\cdot\cdot\cdot\  $ 
-  $ \ln{2}=0.693,147,1\cdot\cdot\cdot\  $ 
-  $ \ln{3}=1.098,612,2\cdot\cdot\cdot\  $ 
-  $ \ln{5}=1.609,437,9\cdot\cdot\cdot\  $ 
-  $ \sqrt{2}=1.414,213,5\cdot\cdot\cdot\  $ 
-  $ \sqrt{3}=1.732,050,8\cdot\cdot\cdot\  $ 
-  $ \sqrt{5}=2.236,067,9\cdot\cdot\cdot\  $ 

## 集合与逻辑

### 集合

### 简单逻辑关系

## 函数与不等式

### 不等式

#### 均值不等式

- 定义

   $ H_n \leqslant G_n \leqslant A_n \leqslant Q_n, $ 即调和平均数不超过几何平均数 $ , $ 几何平均数不超过算术平均数 $ , $ 算术平均数不超过平方平均数 $ , $ 简记为“调几算方”.

- 详细内容
  $$
  \begin{aligned}
  H_n &= \frac{n}{\sum\limits_{i=1}^n \frac{1}{x_i}} = \frac{n}{\frac{1}{x_1}+\frac{1}{x_2}+\cdot\cdot\cdot+\frac{1}{x_n}},被称为调和平均数 \\
  G_n &= \sqrt[n]{\prod\limits_{i=1}^n x_i} = \sqrt[n]{x_1x_2\cdot\cdot\cdot x_n},被称为几何平均数 \\
  A_n &= \frac{\sum\limits_{i=1}^{n}x_i}{n} = \frac{x_1+x_2+\cdot\cdot\cdot+x_n}{n},被称为算数平均数 \\
  Q_n &= \sqrt{\frac{\sum\limits_{i=1}^{n}x_i^2}{n}} = \sqrt{\frac{x_1^2+x_2^2+\cdot\cdot\cdot+x_n^2}{n}},被称为平方平均数
  \end{aligned}
  $$
  
- 常见二维形式

  当且仅当 $ n=2 $ 时 $ , $ 设 $ x_1=a,x_2=b $  $ , $ 则有
  $$
  \frac{2ab}{a+b} \leqslant \sqrt{ab} \leqslant \frac{a+b}{2} \leqslant \sqrt{\frac{a^2+b^2}{2}}.
  $$

#### 柯西不等式

其一般形式为
$$
\sum_{i=1}^{n}a_i^2 \sum_{i=1}^{n}b_i^2 \geqslant \left( \sum_{i=1}^{n} a_ib_i \right) ^2\\
等号成立条件:\\
\frac{a_1}{b_1} = \frac{a_2}{b_2} = \cdots = \frac{a_n}{b_n}\\
或\\
a_i,b_i,i = 1,2,3,\cdots,n中至少有一方全为零.
$$
其常用二维形式为
$$
(a^2 + b^2)(c^2 + d^2) \geqslant (ac + bd)^2\\
当且仅当\frac{a}{c} = \frac{b}{d}时,等号成立.
$$

例1：已知 $ x+2y+3z = 1, $ 求 $ x^2+y^2+z^2 $ 的最小值.
$$
由柯西不等式可得: \\
(x^2+y^2+z^2)(1^2+2^2+3^2) \geqslant x+2y+3z = 1 \\
当x = \frac{y}{2} = \frac{z}{3},即x=\frac{1}{14},y=\frac{1}{7},z=\frac{3}{14}时,等号成立.
$$

例2：求函数 $ y = 5\sqrt{x-1} + \sqrt{10-2x} $ 的最大值.
$$
由柯西不等式可得:\\
\begin{aligned}
y &= 5\sqrt{x-1} + \sqrt{10-2x} \\
&= 5\sqrt{x-1} + \sqrt{2}\sqrt{5-x} \\
&\leqslant\sqrt{5^2+(\sqrt{2})^2} \sqrt{(\sqrt{x-1})^2+(\sqrt{5-x})^2}\\
&= \sqrt{27*4} \\
&= 6\sqrt{3} \\
\end{aligned} \\
当\frac{5}{\sqrt{2}} = \frac{\sqrt{x-1}}{\sqrt{5-x}},即x = \frac{127}{27}时等号成立.
$$

例3：已知 $ a,b,c \in {\mathbb{R^*}}, $  且 $ 3a^2 + 3b^2 + 4c^2 = 60, $ 求 $ a+b+c $ 的最大值.
$$
由柯西不等式可得:\\
(3a^2 + 3b^2 + 4c^2)(\frac{1}{3}+\frac{1}{3}+\frac{1}{4}) \geqslant (a+b+c)^2\\
所以(a+b+c)^2 \leqslant 55\\
所以a+b+c \leqslant \sqrt{55}\\
当
\frac{\sqrt{3}a}{\frac{1}{\sqrt{3}}} = \frac{\sqrt{3}b}{\frac{1}{\sqrt{3}}}  =\frac{2c}{\frac{1}{2}}时,有\\
3a = 3b = 4c\\
设3a = 3b = 4c = k,则a = b = \frac{k}{3},c = \frac{k}{4}\\
此时3a^2 + 3b^2 + 4c^2 = \frac{11}{12}k^2 = 60,k = \frac{12\sqrt{55}}{11}\\
即a = b = \frac{4\sqrt{55}}{11}, c = \frac{3\sqrt{55}}{11}时,等号成立.
$$

#### 对数均值不等式(对均不等式)

- 定义

  对于两个正数 $ a,b>0 $  $ , $ 其对数平均数为 $ \displaystyle L(a,b) = \frac{a-b}{\ln{a}-\ln{b}}(a>0,b>0,a\neq b) $  $ , $ 满足 $ \displaystyle \sqrt{ab} < L(a,b) < \frac{a+b}{2} $ .
  
- 证明

  左边思路：
  $$
  a>b>0时,欲证\sqrt{ab}<\frac{a-b}{\ln{a}-\ln{b}}，即证\ln{\frac{a}{b}}<\frac{a-b}{\sqrt{ab}} \\
  即证\ln{\frac{a}{b}}<\frac{a}{\sqrt{ab}}-\frac{b}{\sqrt{ab}}=\sqrt{\frac{a}{b}}-\sqrt{\frac{b}{a}} \\
  设t=\sqrt{\frac{a}{b}}(t>1),即证\ln{t^2}-t+\frac{1}{t}<0 \\
  构造函数f(t)=2\ln{t}-t+\frac{1}{t},证明f(t)<0(t>1)即可.
  $$
  左边证明：
  $$
  设f(x) = 2\ln{x}-x+\frac{1}{x}(x>1) \\
  则f'(x) = -\frac{(x-1)^2}{x^2}<0 \\
  故f(x)在(1,+\infty)递减,f(x)<f(1) = 0 \\
  设a>b>0,则f(\sqrt{\frac{a}{b}}) = \ln\frac{a}{b}-\sqrt{\frac{a}{b}}+\sqrt{\frac{b}{a}}<0 \\
  所以\frac{a-b}{\ln{a}-\ln{b}}>\sqrt{ab}
  $$
  右边思路：
  $$
  a>b>0时,欲证\frac{a-b}{\ln{a}-\ln{b}}<\frac{a+b}{2},即证\ln\frac{a}{b}>\frac{2(a-b)}{a+b} \\
  即证\ln{\frac{a}{b}}-\frac{2(a-b)}{a+b}=\ln{\frac{a}{b}}-\frac{2(\frac{a}{b}-1)}{\frac{a}{b}+1} >0 \\
  设t=\frac{a}{b}(t>1),即证\ln{t}-\frac{2(t-1)}{t+1}>0 \\
  构造函数f(t)=\ln{t}-\frac{2(t-1)}{t+1},证明f(t)>0(t>1)即可.
  $$
  右边证明：
  $$
  设f(x) = \ln{x}-\frac{2(x-1)}{x+1}(x>1) \\
  则f'(x) = \frac{(x-1)^2}{x(x+1)^2}>0 \\
  故f(x)在(1,+\infty)递增,f(x)>f(1) = 0 \\
  设a>b>0,则f(\frac{a}{b}) = \ln{\frac{a}{b}} - \frac{2(\frac{a}{b}-1)}{\frac{a}{b}-1}>0 \\
  所以\frac{a-b}{\ln{a}-\ln{b}}<\frac{a+b}{2}
  $$

- 使用场景

  对均不等式多用于极值点偏移类问题 $ , $ 解题时可先标注说明并使用 $ , $ 并在解题过程末尾给出对均不等式的证明即可.

#### 琴生不等式

#### 权方和不等式

### 函数

#### 三角函数

##### 和差化积与积化和差

- 和差化积公式
$$
\sin \alpha + \sin \beta = 2\sin \left[\frac{(\alpha + \beta)}{2}\right] \cos \left[\frac{(\alpha - \beta)}{2}\right] \\
\sin \alpha - \sin \beta = 2\cos \left[\frac{(\alpha + \beta)}{2}\right] \sin \left[\frac{(\alpha - \beta)}{2}\right] \\
\cos \alpha + \cos \beta = 2\cos \left[\frac{(\alpha + \beta)}{2}\right] \cos \left[\frac{(\alpha - \beta)}{2}\right] \\
\cos \alpha - \cos \beta = -2\sin \left[\frac{(\alpha + \beta)}{2}\right] \sin \left[\frac{(\alpha - \beta)}{2}\right] \\
$$

- 积化和差公式

$$
\sin \alpha \cdot \cos \beta = \frac{1}{2}[\sin(\alpha + \beta)+\sin(\alpha - \beta)] \\
\cos \alpha \cdot \sin \beta = \frac{1}{2}[\sin(\alpha + \beta)-\sin(\alpha - \beta)] \\
\cos \alpha \cdot \cos \beta = \frac{1}{2}[\cos(\alpha + \beta)+\cos(\alpha - \beta)] \\
\sin \alpha \cdot \sin \beta = -\frac{1}{2}[\cos(\alpha + \beta)-\cos(\alpha - \beta)] \\
$$


##### 三角换元法（参数方程）

基本原理：
$$
\sin^2\alpha + \cos^2\alpha = 1
$$


例：若实数 $ x,y $ 满足 $ x^2 -xy + y^2 = 1 $  $ , $ 求 $ x+y $ 的最小值.
$$
原式 = (x-\frac{y}{2})^2 + (\frac{\sqrt{3}}{2}y)^2  = 1\\
设\cos\alpha = x-\frac{y}{2},\sin \alpha = \frac{\sqrt{3}}{2}y\\
则x=\frac{\sqrt{3}}{3}\sin\alpha + \cos\alpha,y=\frac{2\sqrt{3}}{3}\sin\alpha\\
\begin{aligned}
所以x+y &= \sqrt{3} \sin \alpha + \cos \alpha \\
&= 2(\sin \alpha  \cos \frac{\pi}{6} + \cos \alpha \sin \frac{\pi}{6})\\
&= 2\sin(\alpha + \frac{\pi}{6})\\
\end{aligned}\\
所以x+y \in [ -2,2 ]\\
故x+y的最小值为-2
$$



#### 数列


##### n阶等差数列通项公式

 $ n $ 阶等差公式可视为最高次项为 $ ax^n,n \in \mathbb{N^*} $ 的函数.

 $ n $ 阶等差数列是指其图像符合 $ ax^n + bx^{n-1}+···+z,n \in N^* $ 的图像 $ , $ 若在数列中满足对其反复进行 $ a_{n+1} - a_n $ 的操作 $ , $ 且进行 $ n-1 $ 次后仍为等差数列 $ , $ 则分别代入 $ x = 1,2,···, n+1 $ 即可求出参数值 $ , $ 进而得到通项公式.

例： $ a_n = \{ 4, 12, 32, 70, 132, 224 ,\cdot\cdot\cdot\} $ 

进行第 1 次求差操作后：

 $ b_n = \{ 8, 20, 38, 62, 92,\cdot\cdot\cdot\} $ 

进行第 2 次求差操作后：

 $ c_n = \{ 12, 18, 24, 30,\cdot\cdot\cdot\} $ 

易知 $ c_n $ 为等差数列 $ , $ 故 $ a_n $ 为三阶等差数列 $ , $ 其方程满足 $ an^3 + bn^2 + cn +d. $ 

分别令 $ n = 1, 2, 3, 4, $ 可得方程组：
$$
\\
\begin{cases}
a + b + c + d = 4\\
8a + 4b + 2c + d = 12\\
27a + 9b + 3c + d = 32\\
64a + 16b + 4c + d = 70\\
\end{cases}\\
解得\\
\begin{cases}
a = 1\\
b = 0\\
c = 1\\
d = 2\\
\end{cases}\\
所以\\
a_n = n^3 + n + 2, x \in \mathbb{N^*}
$$

##### 特征根

- 简介

  若存在数列 $ \{a_n\} $ 满足 $ \displaystyle a_n=\sum_{i=1}^k\lambda_i a_{n-i}(n>k) = \lambda_1 a_{n-1} + \lambda_2 a_{n-2} + \lambda_3 a_{n-3} + \cdot\cdot\cdot +\lambda_k a_{n-k}, $ 则我们称数列 $ \{a_n\} $ 为 $ k $ 阶线性递推数列.

- 步骤

  - 列出特征根方程 $ \displaystyle x^k=\sum_{i=1}^k\lambda_i x^{k-i} = \lambda_1 x^{k-1} + \lambda_2 x^{k-2} + \cdot\cdot\cdot + \lambda_{k-1}x^{1} + \lambda_k $ 
  - 解上述方程 $ , $ 得方程根 $ x_1,x_2,\cdot\cdot\cdot x_k $ 
  - 若 $ x_1\neq x_2\neq \cdot\cdot\cdot \neq x_k, $ 则 $ \displaystyle a_n = \sum_{i=1}^k \gamma_ix_i^n = \gamma_1x_1^n + \gamma_2x_2^n+\cdot\cdot\cdot+\gamma_kx_k^n,(\gamma_i为常数) $ 
  - **若出现任意的 $ x_m=x_n, $ 此时 $ a_n $ 不满足上述公式 $ , $ 为特殊情况. 鉴于高考往往最多考察 $ k=2 $ 的情形 $ , $ 此处给出 $ k=2,x_1=x_2 $ 时 $ ,a_n=(\gamma_1 n+\gamma_2)x_1^n,(\gamma_1,\gamma_2均为常数). $ **

例1：若数列 $ \{a_n\} $ 是斐波那契数列 $ , $ 即 $ a_n=1,1,2,3,5,8 \cdot\cdot\cdot\, $ 试求 $ \{a_n\} $ 的通项公式.
$$
对于斐波那契数列,有a_n = a_{n-1}+a_{n-2} \\
其特征根方程为x^2 = x+1 \\
解得x_1 = \frac{1+\sqrt{5}}{2},x_2= \frac{1-\sqrt{5}}{2} \\
则设a_n = \gamma_1 x_1^n + \gamma_2 x_2^n = \gamma_1\left(\frac{1+\sqrt{5}}{2}\right)^n + \gamma_2\left(\frac{1-\sqrt{5}}{2}\right)^n \\
又知a_1 = a_2 = 1,故 \\
\begin{cases}
\gamma_1\left(\frac{1+\sqrt{5}}{2}\right) + \gamma_2\left(\frac{1-\sqrt{5}}{2}\right) = 1 \\
\gamma_1\left(\frac{1+\sqrt{5}}{2}\right)^2 + \gamma_2\left(\frac{1-\sqrt{5}}{2}\right)^2 = 1 \\
\end{cases} \\
解得\gamma_1=\frac{\sqrt{5}}{5}, \gamma_2=-\frac{\sqrt{5}}{5} \\
故a_n = \frac{\sqrt{5}}{5}\left[\left(\frac{1+\sqrt{5}}{2}\right)^n-\left(\frac{1-\sqrt{5}}{2}\right)^n\right]
$$
例2：若数列 $ \{a_n\} $ 满足 $ a_1=10,a_5=2, $ 且 $ a_{n+2}-2a_{n+1}+a_n=0(n\in\mathbb{N^*}), $ 试求 $ \{a_n\} $ 的通项公式.
$$
a_n的特征根方程为x^2-2x+1=(x-1)^2=0 \\
解得x-1=x_2=1\\
满足上文所述特殊情况,按照特殊方式处理,即设 \\
a_n=(\gamma_1 n+\gamma_2)1^n = \gamma_1 n+\gamma_2 \\
\begin{cases}
a_1 = \gamma_1+\gamma_2=10 \\
a_5 = 5\gamma_1+\gamma_2=2 \\
\end{cases} \\
解得\gamma_1=-2,\gamma_2=12 \\
故a_n = (-2n+12)1^n = 12-2n
$$

##### 不动点

- 原理

  设 $ x_0 $ 是 $ y=f(x) $ 的不动点 $ , $ 且 $ f(x) $ 是多项式函数或分式多项式函数 $ , $ 可得 $ f(x_0)-x_0=0. $ 设函数 $ p(x)=f(x)-x_0, $ 则 $ p(x) $ 满足 $ p(x_0)=f(x_0)-x_0=0. $ 又因为 $ x_0 $ 是 $ f(x)=x $ 的根 $ , $ 故 $ p(x) $ 必然包含因式 $ (x-x_0), $ 设 $ p(x)=\Gamma\cdot(x-x_0), $ 其中 $ \Gamma $ 为某多项式.则有 $ \displaystyle f(x)-x_0=\Gamma\cdot(x-x_0) $  $ , $  $ \Gamma=\frac{f(x)-x_0}{x-x_0}. $ 若存在数列 $ a_n $ 满足 $ f(x)=a_{n+1},x=a_n, $ 即 $ \displaystyle \Gamma=\frac{a_{n+1}-x_0}{a_n-x_0}. $ 

- 步骤

  - 首先 $ , $ 根据数列递推方程解出不动点 $ x_0 $ 

  - 其次 $ , $ 将递推公式整理成形如 $ a_{n+1}=\Gamma $ 的式子 $ , $ 其中 $ \Gamma $ 是包含 $ a_n $ 的多项式

  - 然后 $ , $ 在方程两边同时减去 $ x_0 $ 进行构造 $ , $ 得到 $ a_{n+1}-x_0=\Gamma-x_0 $ 

  - 最后 $ , $ 根据构造的等式通过作商 $ , $ 取对数 $ , $ 取倒数等变换推出通项公式
  
- 注意

  若解出不动点 $ x_0\in\mathbb{C}, $ 即 $ x_0 $ 为虚数 $ , $ 请正常进行解题.若解得 $ a_n $ 的模长为 $ 1, $ 则该数列为周期数列.

例1：已知数列 $ \{a_n\} $ 满足 $ a_1=2,a_{n+1}=a_n^2+2a_n(n\in\mathbb{N^*}), $ 求 $ \{a_n\} $ 的通项公式.
$$
观察得不动点方程x=x^2+2x,解得x=-1或x=0(无意义,舍去) \\
方程两边同时减去-1得:a_{n+1}+1 = a_n^2+2a_n+1=(a_n+1)^2 \\
对等式两边取对数得:\ln{(a_{n+1}+1)} = 2\ln{(a_n+1)} \\
又a_1=2,\ln{(a_1+1)}=\ln{3},故\ln{(a_{n}+1)} = \ln{3}\cdot2^{n-1} = \ln{3^{2^{n-1}}} \\
即a_n+1=3^{2^{n-1}},a_n=3^{2^{n-1}}-1. \\
$$
例2：已知数列 $ \{a_n\} $ 满足 $ \displaystyle a_1=3,a_{n+1}=\frac{3a_n-4}{a_n-2}(n\in\mathbb{N^*}), $ 求 $ \{a_n\} $ 的通项公式.
$$
观察得不动点方程x=\frac{3x-4}{x-2},解得x=4或x=1 \\
对于x=4时,方程两边同时减去4得:a_{n+1}-4=\frac{3a_n-4}{a_n-2}-4=\frac{-(a_n-4)}{a_n-2}\cdot\cdot\cdot\cdot\cdot\cdot(1) \\
对于x=1时,方程两边同时减去1得:a_{n+1}-1=\frac{3a_n-4}{a_n-2}-1=\frac{2(a_n-4)}{a_n-2}\cdot\cdot\cdot\cdot\cdot\cdot(2) \\
对(1)(2)式作商得: \\
\frac{a_{n+1}-4}{a_{n+1}-1}=-\frac{1}{2}\cdot\frac{a_{n}-4}{a_{n}-1} \\
不妨设b_n=\frac{a_{n}-4}{a_{n}-1},b_1=\frac{a_{1}-4}{a_{1}-1}=-\frac{1}{2} \\
b_{n+1}=-\frac{1}{2}b_n,故b_n=b_1\cdot\left(-\frac{1}{2}\right)^{n-1}=\left(-\frac{1}{2}\right)^{n} \\
即a_n-4=\left(-\frac{1}{2}\right)^{n}(a_n-1),a_n=\frac{4-\left(-\frac{1}{2}\right)^{n}}{1-\left(-\frac{1}{2}\right)^{n}}=\frac{4(-2)^n-1}{(-2)^n-1}.
$$
例3：已知数列 $ \{a_n\} $ 满足 $ \displaystyle a_1=2,a_{n+1}=\frac{a_n+1}{-a_n+3}(n\in\mathbb{N^*}), $ 求 $ \{a_n\} $ 的通项公式.
$$
观察得不动点方程x=\frac{x+1}{-x+3},解得x=1 \\
方程两边同时减去1得:a_{n+1}-1=\frac{a_n+1}{-a_n+3}-1=\frac{2a_n-2}{-a_n+3} \\
等式两边同时取倒数得:\frac{1}{a_{n+1}-1} = \frac{-a_n+3}{2a_n-2} = \frac{-(a_n-1)+2}{2a_n-2} = -\frac{1}{2}+\frac{1}{a_n-1} \\
不妨设b_n = \frac{1}{a_n-1},b_1=\frac{1}{a_1-1}=1 \\
b_{n+1}=-\frac{1}{2}+b_n,故b_{n}=1-\frac{1}{2}(n-1)=\frac{3-n}{2} \\
即\frac{1}{a_n-1}=\frac{3-n}{2},a_n=\frac{5-n}{3-n}.
$$

#### 导数

##### 端点效应

- 原理

  通过分析函数在端点处的函数值 $ , $ 各阶导数值来分析使题设条件恒成立的必要条件 $ , $ 从而缩小参量区间 $ , $ 从而得到答案 $ . $ 再验证其充分性 $ , $ 即可求出题目所需的取值或取值范围.

例1：(2007全国1卷理科数学)设函数 $ f(x) = e^x-e^{-x}, $ 若对于所有 $ x=0 $ 都有 $ f(x)\geqslant ax,求 $  $ a $ 的取值范围.
$$
设g(x) = e^x-e^{-x}-ax,x\geqslant 0 \\
g'(x) = e^x+e^{-x}-a,且g(0) = 0 \\
若g'(0)<0,则必然存在x_0\in(0,+\infty),f'(x)<0,f(x)单调递减 \\
故存在一点x_m \in (0,x_0)使得f(x_m)<0,不满足题意 \\
故g'(0)=2-a \geqslant 0,解得a\leqslant2,这是满足题意的必要条件. \\
接下来证明其充分性. \\
当a\leqslant2时,有g'(x) = e^x+e^{-x}-a \geqslant e^x+e^{-x}-2 \geqslant 0.(均值不等式) \\
所以g(x)_{min} = g(0) = 0,满足题意. \\
综上所述,a \in (-\infty, 2].
$$

##### 隐零点

利用隐零点解题 $ , $ 或采用换元法简化计算.

例1：已知函数 $ f(x) = axe^x(a \ne 0), g(x) = x + \ln x + 1. $ 若对于任意的 $ x > 0, f(x) \geqslant g(x) $ 恒成立 $ , $ 求实数 $ a $ 的取值范围.

法一（隐零点）：
$$
由题可得:\\
axe^x - x - \ln x - 1 \geqslant 0 \\
a \geqslant \frac{x + \ln x + 1}{xe^x} \\
设h(x) = \frac{x + \ln x + 1}{xe^x} \\
h'(x) = \frac{e^x(x+1)(-x-\ln x)}{(xe^x)^2} \\
设p(x) = -x-\ln x \\
p'(x) = -1-\frac{1}{x}<0 \\
\therefore p(x)在(0,+\infty)上单调递减 \\
p(1) = -1 < 0, p(\frac{1}{e}) = 1- \frac{1}{e} > 0 \\
\therefore 存在x_0 \in (\frac{1}{e}, 1) \\
p(x_0) = 0,即x_0 + \ln x_0 = 0 \\
\therefore 在(0, x_0)上p(x)>0,h'(x)>0,h(x)单调递增 \\
在(0, x_0)上p(x)<0,h'(x)<0,h(x)单调递减 \\
h(x)_{max} = h(x_0) = \frac{x_0 + \ln x_0 + 1}{x_0 e^{x_0}} = 1 \\
\therefore a \geqslant 1
$$
法二（换元法）：
$$
设xe^x =t,\ln x + x = \ln t \\
at \geqslant \ln t + 1, t \in (0, +\infty) \\
a \geqslant \frac{\ln t + 1}{t} \\
设h(t) = \frac{\ln t + 1}{t} \\
h'(t) = \frac{-\ln t}{t^2} \\
\therefore h(t)在(0,1)上单调递增,在(1,+\infty)上单调递减 \\
\therefore h(t)_{max} = h(1) = 1 \\
\therefore a \geqslant 1
$$

##### 含 $ e^x $ 和 $ \ln x $ 的解法技巧

**注意：含 $ e^x $ 的函数应适当转换成 $ e^xf(x) $ 和 $ \frac{e^x}{f(x)} $ 的形式 $ , $ 含 $ \ln x $ 的函数应适当转换成 $ f(x) \pm lnx $ 的形式.**

例1：已知函数 $ f(x) = (x-1)e^x + a(2e - e^x). $ 若不等式 $ f(x)>0 $ 对 $ x \in (2,+\infty) $ 恒成立 $ , $ 求整数 $ a $ 的最大值.
$$
由题可得:\\
(x-1)e^x + a(2e - e^x) > 0 \\
a < \frac{(x-1)e^x}{e^x-2e} \\
设g(x) = \frac{(x-1)e^x}{e^x-2e} \\
g'(x) = \frac{e^x(e^x-2ex)}{(e^x-2e)^2} \\
设h(x) = e^x-2ex \\
h'(x) = e^x-2e>0 \\
\therefore h(x)单调递增 \\
h(2) = e^2 - 4e < 0 \\
h(3) = e^3 - 6e > 0 \\
\therefore 存在x_0 \in (2,3)使h(x_0) = 0 \\
故在(2, x_0)上,h(x) < 0, g'(x) < 0, g(x)单调递减 \\
在(2, x_0)上,h(x) > 0, g'(x) > 0, g(x)单调递增 \\
h(x_0) = e^{x_0} - 2ex_0 = 0 \\
\therefore g(x)_{min} = g(x_0) = \frac{(x-1)e^{x_0}}{e^{x_0}-2e} 
 = \frac{(x_0 - 1)2ex_0}{2e(x_0) - 1} = x_0 \in (2,3) \\
 \therefore a_{max} < g(x)_{min} \\
 \therefore a_{max} < 2 \\
$$
例2：已知函数 $ f(x) = (2x-1)\ln x + x - 1. $ 求证 $ :f(x) > -1 $ 
$$
由题可得: \\
(2x-1)\ln x + x > 0 \\
设g(x) = (2x-1)\ln x + x \\
g'(x) = \frac{1}{x} - \frac{1}{(2x-1)^2} = \frac{(4x-1)(x-1)}{x(2x-1)^2} \\
①若2x-1>0,只需证明\ln x + \frac{x}{2x-1}>0,x>\frac{1}{2} \\
此时g(x)在(\frac{1}{2},1)上单调递减,在(1,+\infty)上单调递增\\
\therefore g(x)_{min} = g(1) = 1 > 0 ,满足题意\\
②若2x-1<0,只需证明\ln x + \frac{x}{2x-1}<0,x<\frac{1}{2} \\
此时g(x)在(0,\frac{1}{4})上单调递增,在(\frac{1}{4},\frac{1}{2})上单调递减\\
\therefore g(x)_{max} = g(\frac{1}{4}) = -\ln 4 - \frac{1}{2} < 0 ,满足题意\\
③若2x-1=0,只需证明\ln x + \frac{x}{2x-1}=0,x=\frac{1}{2} \\
此时g(x) = g(\frac{1}{2}) = -\frac{1}{2} > -1,满足题意.\\
故f(x) > -1 \\
$$

##### 同构

**同时出现 $ e^x $ 与 $ \ln x $ 结构的函数极有可能使用同构的方法解题**

例1：对任意的实数 $ x>0, $ 不等式 $ 2ae^{ax}-\ln x+ \ln a \geqslant 0 $ 恒成立 $ , $ 求实数 $ a $ 的最小值.
$$
2ae^{ax}\geqslant \ln a -\ln x \\
2xe^{2x} \geqslant \frac{x}{a}\ln{\frac{x}{a}} = \ln{\frac{x}{a}} e^{\ln{\frac{x}{a}}} \\
设f(x) = xe^x,则f(2x)>f(\ln{\frac{x}{a}}) \\
f'(x) = (x+1)e^x > 0,所以f(x)在(0,+\infty)单调递增 \\
2x \geqslant \ln{\frac{x}{a}} = \ln x - \ln a , \ln a \geqslant \ln x - 2x \\
设g(x) = \ln x - 2x, g'(x) = \frac{1}{x} - 2 = \frac{1-2x}{x} \\
故g(x)在(0,\frac{1}{2})上单调递增,在(\frac{1}{2},+\infty)上单调递减 \\
\therefore g(x)_{max} = g(\frac{1}{2}) = \ln{\frac{1}{2}} - \ln e = \ln{\frac{1}{2e}} \\
\therefore a \geqslant \frac{1}{2e},即a_{min} = \frac{1}{2e}
$$
例2：已知 $ a>0, $ 关于 $ x $ 的不等式 $ e^x-a\ln(ax-a)+a>0 $ 恒成立 $ , $ 求实数 $ a $ 的取值范围.
$$
\frac{e^x}{a} > \ln(a(x-1))-1 \\
e^{x-\ln a} > \ln a + \ln(x-1) - 1 \\
e^{x-\ln a} + x - \ln a > \ln(x-1) + x - 1 = e^{\ln(x-1)} + \ln(x-1) \\
设f(x) = e^x + x,则f(x-\ln a) > f(\ln(x-1)) \\
f'(x) = e^x + 1 > 0,所以f(x)在R上单调递增 \\
\therefore x - \ln a > \ln(x-1) \\
\ln a < x - \ln(x-1) \\
设g(x) = x - \ln(x-1) \\
g'(x) = 1 - \frac{1}{x-1} = \frac{x-2}{x-1} \\
\therefore g(x)在(-\infty,2)上单调递减,在(2,+\infty)上单调递增 \\
\therefore g(x)_{min} = g(2) = 2 \\
\therefore a < e^2
$$
例3：已知 $ f(x) = e^x-x $ 与 $ g(x) = x - \ln x $ 有相同的最小值 $ . $ 证明：存在直线 $ y=b, $ 其与两条曲线 $ y=f(x) $ 和 $ y=g(x) $ 共有三个不同的交点 $ , $ 并且从左到右三个交点的横坐标成等差数列.
$$
分析图像可知,当y=f(x)和y=g(x)有三个交点时,b有且仅有一个定值.\\
设f(x)=b的两点横坐标分别为x_1,x_2;g(x)=b的两点横坐标分别为x_2,x_3; \\
其中f(x)与g(x)交点的横坐标为x_2 \\
f(x_1) = f(x_2) = g(x_2) = g(x_3) = b \\
e^{x_1}-x_1 = e^{x_2}-x_2 = x_2 - \ln{x_2} = x_3 - \ln{x_3} = b \\
\because e^{x_1}-x_1 = e^{x_1} - \ln{e^{x_1}} = x_2 - \ln{x_2} \\
\therefore x_2 = e^{x_1} \\
\because x_3 - \ln{x_3} = e^{\ln{x_3}} - \ln{x_3} = e^{x_2} - x_2 \\
\therefore x_2 = \ln{x_3} \\
\therefore x_1 + x_3 = \ln{x_2} + e^{x_2} = x_2 - b + x_2 + b = 2x_2 ,证毕.\\
$$

##### 洛必达法则

洛必达法则可以用来求一些函数不定式的极限.

**定义**

- 零比零型

  若函数 $ f(x) $ 与 $ g(x) $ 满足 $ \displaystyle \lim_{x\to a}{f(x)=0},\lim_{x\to a}{g(x)=0}, $ 在点 $ a $ 的附近 $ f(x) $ 与 $ g(x) $ 均 $ n $ 阶可导 $ ,g^{(n)}(x)\neq0,则 $ 

   $ \displaystyle \lim_{x\to a}{\frac{f(x)}{g(x)}} = \lim_{x\to a}{\frac{f'(x)}{g'(x)}} = \lim_{x\to a}{\frac{f''(x)}{g''(x)}} = \cdot\cdot\cdot = \lim_{x\to a}{\frac{f^{(n)}(x)}{g^{(n)}(x)}} $ 

- 无穷比无穷型
  若函数 $ f(x) $ 与 $ g(x) $ 满足 $ \displaystyle \lim_{x\to a}{f(x)=\infty},\lim_{x\to a}{g(x)=\infty}, $ 在点 $ a $ 的附近 $ f(x) $ 与 $ g(x) $ 均 $ n $ 阶可导 $ ,g^{(n)}(x)\neq0,则 $ 

   $ \displaystyle \lim_{x\to a}{\frac{f(x)}{g(x)}} = \lim_{x\to a}{\frac{f'(x)}{g'(x)}} = \lim_{x\to a}{\frac{f''(x)}{g''(x)}} = \cdot\cdot\cdot = \lim_{x\to a}{\frac{f^{(n)}(x)}{g^{(n)}(x)}} $ 

例1：试分析函数 $ f(x) = x\ln{x} $ 的图像.
$$
f'(x) = \ln{x}+1,易知函数在(0,\frac{1}{e})单调递减,在(\frac{1}{e},+\infty)单调递增. \\
显然f(\frac{1}{e}) = -\frac{1}{e},f(1) = 0,\lim_{x\to +\infty}{f(x)} = +\infty. \\
而对于x\to 0的情况,其极限不易直接得出,此时可利用洛必达法则. \\
\begin{aligned}
\lim_{x\to 0^+}{f(x)} &= \lim_{x\to 0^+}{x\ln{x}} \\
&= \lim_{x\to 0^+}{\frac{\ln{x}}{\frac{1}{x}}} \\
&= \lim_{x\to 0^+}{\frac{(\ln{x})'}{(\frac{1}{x})'}} \\
&= \lim_{x\to 0^+}{\frac{\frac{1}{x}}{-\frac{1}{x^2}}} \\
&= \lim_{x\to 0^+}{(-x)} \\
&= 0
\end{aligned} \\
$$
例2：设函数 $ f(x)=e^x-1-x-ax^2. $ 若当 $ x\geqslant0 $ 时 $ f(x)\geqslant0, $ 求 $ a $ 的取值范围.
$$
本题洛必达法则并非最优解,但却能较好地展示洛必达法则的使用. \\
由题可知f(0)=0. \\
当x\geqslant0时,f(x)\geqslant0等价于a\leqslant\frac{e^x-x-1}{x^2} \\
设g(x) = \frac{e^x-x-1}{x^2},则g'(x) = \frac{xe^x-2e^x+x+2}{x^3}. \\
设h(x) = xe^x-2e^x+x+2,则h'(x) = xe^x-e^x+1,h''(x) = xe^x\geqslant0. \\
易知h'(x)在(0,+\infty)单调递增,h'(x)\geqslant h'(0)=0. \\
易知h(x)在(0,+\infty)单调递增,h(x)\geqslant h(0)=0,g'(x)\geqslant0. \\
易知g(x)在(0,+\infty)单调递增,g(x)\geqslant g(0). \\
发现利用初等数学知识无法求出g(0),故考虑使用洛必达法则. \\
\lim_{x\to0^+}{g(x)} = \lim_{x\to0^+}{\frac{e^x-x-1}{x^2}} = \lim_{x\to0^+}{\frac{e^x-1}{2x}} = \lim_{x\to0^+}{\frac{e^x}{2}} = \frac{1}{2}. \\
故a\leqslant\frac{1}{2}. \\
综上,a的取值范围为\left(-\infty,\frac{1}{2}\right].
$$
**注：虽然洛必达法则是十分有用的定理 $ , $ 然而其作用却较为局限 $ , $ 在高中阶段除了分析函数图像之外 $ , $ 往往也只有某些题目分离参数后才会遇到 $ , $ 而这类题现在也难以出现 $ , $ 因此不建议盲目使用洛必达法则.**



**附:洛必达法则的证明**



##### 函数的凹凸性



#### 中值定理

##### 罗尔中值定理

##### 拉格朗日中值定理

- 基本概念

  若 $ f(x) $ 满足 $ ①f(x)在闭区间[a,b]内连续,②f(x)在开区间(a,b)上可导, $ 则存在 $ \displaystyle \xi \in (a,b),f'(\xi) = \frac{f(b)-f(a)}{b-a}. $ 

- 几何意义

  在满足定理条件的曲线 $ f(x) $ 上至少存在一点 $ P(\xi,f(\xi)), $ 该曲线在该点的切线平行与曲线两端的连线 $ AB $ .

例1：(2009年辽宁卷理21题)已知函数 $ \displaystyle f(x)=\frac{1}{2}x^2-ax+(a-1)\ln{x},a>1. $ 

​		(Ⅰ)讨论函数 $ f(x) $ 的单调性 $ ; $ 
$$
f'(x) = x-a+\frac{a-1}{x} = \frac{x^2-ax+a-1}{x} = \frac{(x-1)(x+1-a)}{x} \\
若a-1=1,即a=2,则 \\
f'(x) = \frac{(x-1)^2}{x},故f(x)在(0,+\infty)单调递增. \\
若a-1<1,且a>1,故1<a<2时,则f(x)在(0,a-1),(1,+\infty)单调递增,在(a-1,1)单调递减. \\
若a-1>1,则a>2,此时f(x)在(0,1),(a-1,+\infty)单调递增,在(1,a-1)单调递减.
$$
​		(Ⅱ)证明：若 $ a<5, $ 则对任意 $ x_1,x_2 \in (0,+\infty), x_1 \neq x_2,  $ 有 $ \displaystyle \frac{f(x_1)-f(x_2)}{x_1-x_2} > -1. $ 
$$
欲证\frac{f(x_1)-f(x_2)}{x_1-x_2} > -1成立,只需证f(\xi)=\xi -a +\frac{a-1}{\xi}>-1. \\
即设g(\xi) = \xi^2-(a-1)\xi+a-1,则\Delta = (a-1)^2-4(a-1) = (a-1)(a-5). \\
因为1<a<5,所以g(\xi)>0,即\xi^2-(a-1)\xi+a-1>0. \\
所以\xi^2-a\xi+a-1>-\xi. \\
又因为\xi \in (x_1,x_2),且x_1,x_2\in(0,+\infty),故\xi>0. \\
所以\frac{\xi^2-a\xi+a-1}{\xi}=\xi-a+\frac{a-1}{\xi} > -1.\\
因此\frac{f(x_1)-f(x_2)}{x_1-x_2} > -1.
$$

##### 柯西中值定理

#### 切/割线夹(放缩)

##### 形如 $ x_1+x_2<a $ 的不等式证明

##### 形如 $ x_1-x_2<a $ 的不等式证明

- 该类型通常可以构造函数的两条切线进行放缩.

  例1：已知函数 $ f(x)=(x+1)(e^x-1), $ 若方程 $ f(x)=m $ 有两个实数根 $ x_1,x_2, $ 且 $ x_1<x_2, $ 证明： $ \displaystyle x_2-x_1\leqslant 1+\frac{m(1-2e)}{1-e} $ .
  $$
  f'(x)=(x+2)e^x-1,f'(-1)=\frac{1}{e}-1,f'(0)=1 \\
  f''(x)=e^x(x+3),x\in(-3,+\infty),f''(x)>0,函数为凹函数 \\
  设点(-1,f(-1))处的切线方程为g(x)=(\frac{1}{e}-1)(x+1) \\
  设点(0,f(0))处的切线方程为h(x)=x \\
  易得f(x)\geqslant g(x),f(x)\geqslant h(x) \\
  设直线y=m分别交g(x)于点P\left(-1+\frac{em}{1-e},m\right)和点Q(m,m) \\
  设x_3=x_P=-1+\frac{em}{1-e},x_4=x_Q=m \\
  易知x_3\leqslant x_1 \leqslant x_2 \leqslant x_4,即x_2-x_1\leqslant x_4-x_3 \\
  又x_4-x_3=1+\frac{m(1-2e)}{1-e},故x_2-x_1\leqslant 1+\frac{m(1-2e)}{1-e},证毕.
  $$

  例2：已知函数 $ f(x)=3x-e^x+1, $ 其中 $ e=2.71828... $ 是自然对数的底数.
  
  (1)设曲线 $ y=f(x) $ 与 $ x $ 轴正半轴相交于点 $ P(x_0,0), $ 曲线在点 $ P $ 处的切线为 $ l, $ 求证：曲线 $ y=f(x) $ 上的点都不在直线 $ l $ 的上方 $ ; $ 
  $$
  由题,P在f(x)上,满足f(x_0)=3x_0-e^{x_0}+1=0,即e^{x_0}=3x_0+1 \\
  又f'(x)=3-e^x,f'(x_0)=3-e^{x_0} \\
  切线方程y-f(x_0)=f'(x_0)(x-x_0) \\
  即y=(2-3x_0)(x-x_0)\\
  设g(x)=(2-3x_0)(x-x_0)-f(x) = (-1-3x_0)x+e^x+3x_0^2-2x_0-1 \\
  则g'(x)=e^x-3x_0-1,不难发现g'(x_0)=0 \\
  x\in(-\infty,x_0)时,g'(x)<0,g(x)递减 \\
  x\in(x_0,+\infty)时,g'(x)>0,g(x)递增 \\
  故g(x)\geqslant g(x_0)=0
  $$
  (2)若关于 $ x $ 的方程 $ f(x)=m $ ( $ m $ 为正实数)有两个不等实根 $ x_1,x_2(x_1<x_2), $ 求证： $ \displaystyle x_2-x_1<2-\frac{3}{4}m. $ 
  $$
  由(1),g(x)=e^x-(3x_0+1)x+3x_0^2-2x_0-1\geqslant f(x) \\
  易知f(x)在原点处的切线为y=2x,设h(x)=2x,显然h(x)\geqslant f(x) \\
  设h(x),g(x)分别和直线y=m交于点x_3,x_4 \\
  由f(x)图像知x_3\leqslant x_1 < x_2 \leqslant x_4,则x_2-x_1<x_4-x_3 \\
  分别令h(x)=m,g(x)=m得x_3=\frac{m}{2},x_4=x_0+\frac{m}{2-3x_0} \\
  则x_4-x_3=x_0+\frac{m}{2-3x_0}-\frac{m}{2} \\
  设s(x_0)=x_4-x_3=x_0+\frac{m}{2-3x_0}-\frac{m}{2} \\
  s'(x_0)=1+\frac{3mx_0}{(2-3x_0)^2}>0 \\
  由题知m,x_0>0,故s(x_0)在(0,+\infty)递增 \\
  对于f(x),易知f(2)=6-e^2+1<0,故x_0<2 \\
  故s(x_0)<s(2)=2+\frac{m}{2-6}-\frac{m}{2}=2-\frac{3}{4}m \\
  故x_2-x_1<x_4-x_3<2-\frac{3}{4}m
  $$

#### 泰勒公式

泰勒公式是一个用函数在某点的信息描述其附近取值的公式.

设 $ n $ 是一个正整数.如果定义一个包含 $ a $ 的区间上的函数 $ f $ 在 $ a $ 点处 $ n+1 $ 次可导 $ , $ 那么对于这个区间上的任意 $ x, $ 都有:

 $ \displaystyle f(x)=f(a)+\frac{f'(a)}{1!}(x-a)+\frac{f''(a)}{2!}(x-a)^2+\cdot\cdot\cdot+\frac{f^{(n)}(a)}{n!}(x-a)^n+R_n(x). $ 

其中的多项式称为函数在 $ a $ 处的**泰勒展开式** $ , $ 剩余的 $ R_n(x) $ 是泰勒公式的余项 $ , $ 是 $ (x-a)^n $ 的高阶无穷小.

#### 麦克劳林公式

麦克劳林公式是泰勒公式的一种特殊形式.在不需要余项的精确表达式时 $ , $ 令 $ a=0, $ 则 $ n $ 阶泰勒公式也可近似写成

 $ \displaystyle f(x)=f(0)+f'(0)+\frac{f''(0)}{2!}x^2+\cdot\cdot\cdot+\frac{f^{(n)}(0)}{n!}x^n. $ 

**常见麦克劳林公式如下**

 $ \displaystyle e^x=\sum_{n=0}^{\infty}\frac{x^n}{n!}=1+x+\frac{x^2}{2}+\frac{x^3}{6}+\cdot\cdot\cdot+\frac{x^k}{k!}+\cdot\cdot\cdot $ 

 $ \displaystyle \ln(1+x)=\sum_{n=0}^{\infty}\frac{(-1)^n}{n+1}x^{n+1}=x-\frac{x^2}{2}+\frac{x^2}{3}-\frac{x^4}{4}+\cdot\cdot\cdot+\frac{(-1)^kx^{k+1}}{k+1}+\cdot\cdot\cdot,x\in(-1,1] $ 

 $ \displaystyle \sin{x}=\sum_{n=0}^{\infty}\frac{(-1)^n}{(2n+1)!}x^{2n+1}=x-\frac{x^3}{6}+\frac{x^5}{120}-\cdot\cdot\cdot\frac{(-1)^k}{(2k+1)!}x^{2k+1}+\cdot\cdot\cdot $ 

 $ \displaystyle \cos{x}=\sum_{n=0}^{\infty}\frac{(-1)^n}{(2n)!}x^{2n}=1-\frac{x^2}{2}+\frac{x^4}{24}-\cdot\cdot\cdot\frac{(-1)^k}{(2k)!}x^{2k}+\cdot\cdot\cdot $ 

 $ \displaystyle \sqrt{1+x}=\sum_{n=1}^{\infty}\frac{(-1)^{n-1}(2n)!}{2^{2n}(n!)^2(2n-1)}x^{2n}=1+\frac{x}{2}-\frac{x^2}{8}+\frac{x^3}{16}-\cdot\cdot\cdot+\frac{(-1)^{k-1}(2k)!}{2^{2k}(k!)^2(2k-1)}x^{2k}+\cdot\cdot\cdot $ 

#### 用定积分解决函数与数列不等式问题

**定积分概念**

设函数 $ f(x) $ 在区间 $ [a,b] $ 上连续 $ , $ 用分点 $ a=x_0<x_1<···<x_{i-1}<x_i<···<x_n=b $ 将区间 $ [a,b] $ 等分成 $ n $ 个小区间 $ , $ 在每个小区间 $ [x_{i-1},x_i] $ 上取任意一点 $ \xi_i(i=1,2,···,n), $ 作和式
$$
\sum_{i=1}^n{f(\xi_i)\Delta x} = \frac{b-a}{n}\sum_{i=1}^n{f(\xi_i)}
$$
当 $ n\to +\infty $ 时 $ , $ 上述和式若能无限接近某个常数 $ , $ 则把这个常数叫做函数 $ f(x) $ 在区间 $ [a,b] $ 上的定积分 $ , $ 记作 $ \displaystyle \int_a^b{f(x)\mathrm{d}x}, $ 即 $ \displaystyle \int_a^b{f(x)\mathrm{d}x} = \lim_{n \to +\infty} \frac{b-a}{n}\sum_{i=1}^n{f(\xi_i)}. $  

这里 $ a $ 与 $ b $ 的分别叫做积分下限与积分上限 $ , $ 区间 $ [a,b] $ 叫做积分区间 $ , $ 函数 $ f(x) $ 叫做被积函数 $ ,x $ 叫做积分变量 $ ,f(x)\mathrm{d}x $ 叫做被积式 $ . $ 

**微积分基本定理**

用定积分的定义计算定积分太复杂 $ , $ 但计算定积分可用微积分基本定理 $ , $ 也叫做牛顿-莱布尼茨公式 $ . $ 

若 $ F'(x) = f(x), $ 则 $ \displaystyle \int_a^b{f(x)\mathrm{d}x} = F(x)\Bigg\vert_a^b = F(b) - F(a). $ 

**定积分的性质**

(1) $ \displaystyle \int_a^bkf(x)\mathrm{d}x = k\int_a^bf(x)\mathrm{d}x(k为常数) $ 

(2) $ \displaystyle \int_a^b{(f(x) \pm g(x))\mathrm{d}x} = \int_a^bf(x)\mathrm{d}x \pm \int_a^bg(x)\mathrm{d}x $ 

(3) $ \displaystyle \int_a^bf(x)\mathrm{d}x = \int_a^cf(x)\mathrm{d}x + \int_b^cf(x)\mathrm{d}x(其中a<c<b) $ 

**用定积分求曲边梯形面积**

定积分表示函数 $ f(x) $ 与 $ x $ 轴围成的面积 $ . $ 由三条直线 $ x=a,x=b(a<b),x $ 轴及曲线 $ y = f(x)(f(x)\geqslant 0) $ 围成的曲边梯形的面积 $ S= \displaystyle \int_a^b{f(x)\mathrm{d}x}. $ 

多个曲边梯形和差面积可由不同函数定积分和差求出 $ . $ 



例1：(2004年复旦大学保送生考试第二题第5题)求证：

$$
1 + \frac{1}{2\sqrt{2}} + \frac{1}{3\sqrt{3}} + \cdot\cdot\cdot + \frac{1}{n\sqrt{n}} < 3 (n \in {\mathbb{N^*}}).
$$
注意：本题的常规解法是放缩法 $ , $ 但难以想到 $ , $ 而使用定积分则可以简化问题 $ . $ 
$$
证明:下面只证n \geqslant 2 时成立. \\
设f(x) = \frac{1}{n\sqrt{n}}(x>0),易知函数f(x)时减函数. \\
作图发现在区间[i,i+1]上曲边梯形的面积大于矩形的面积,得\int_i^{i+1}f(x)\mathrm{d}x > f(i+1)(i>0), \\
所以(-2x^{-\frac{1}{2}}) \Bigg \vert_i^{i+1} > \frac{1}{(i+1)\sqrt{i+1}}(i>0), \\
即\frac{1}{(i+1)\sqrt{i+1}}(i>0) < 2\left( \frac{1}{\sqrt{i}} - \frac{1}{\sqrt{i+1}} \right)(i>0). \\
令i = 1,2,\cdot\cdot\cdot,n-1后,相加便得\frac{1}{2\sqrt{2}} + \frac{1}{3\sqrt{3}} + \cdot\cdot\cdot + \frac{1}{n\sqrt{n}} < 2\left( 1 - \frac{1}{n} \right), \\
所以1 + \frac{1}{2\sqrt{2}} + \frac{1}{3\sqrt{3}} + \cdot\cdot\cdot + \frac{1}{n\sqrt{n}} < 1 + 2\left( 1 - \frac{1}{\sqrt{n}} \right) < 3.
得欲证成立.
$$

例2：(2010湖北理21(3))求证：
$$
1+\frac{1}{2}+\frac{1}{3}+\cdot\cdot\cdot+\frac{1}{n} > \ln(n+1) + \frac{n}{2(n+1)} (n \in {\mathbb{N^*}})
$$

$$
证明:设f(x) = \frac{1}{x}(x>0),易知函数f(x)是减函数且是下凸函数. \\
在[i,i+1]上曲边梯形面积小于梯形面积,得 \\
\int_i^{i+1}{f(x)\mathrm{d}x} < \frac{1}{2}[f(i)+f(i+1)](i>0) \\
即[f(i)+f(i+1)] > 2[\ln(i+1)-\ln{i}](i>0) \\
\sum_{i=1}^n{[f(i)+f(i+1)]} > \sum_{i=1}^n{2[\ln(i+1)-\ln{i}]} \\
2(1+\frac{1}{2}+\frac{1}{3}+\cdot\cdot\cdot+\frac{1}{n})-1+\frac{1}{n+1} > 2\ln(n+1) \\
1+\frac{1}{2}+\frac{1}{3}+\cdot\cdot\cdot+\frac{1}{n} > \ln(n+1) + \frac{n}{2(n+1)},证毕.
$$

## 立体几何

### 向量叉乘计算法向量

运用向量的叉乘（外积）即可快速求法向量.
$$
设有向量\vec a = (x_1,y_1,z_1), \vec b = (x_2,y_2,z_2) \\
设\vec c为向量\vec a 和\vec b的法向量 \\
分别将x_1,y_1,z_1与x_2,y_2,z_2横着写两遍 \\
即 \\
\begin{array}{c}
& x_1 & x_2 & x_3 & x_1 & x_2 & x_3 \\
& y_1 & y_2 & y_3 & y_1 & y_2 & y_3 \\
\end{array} \\
然后选取中间四列，分别进行左上乘右下减右上乘左下的操作即可得到\vec c \\
即
\vec c = (x_2y_3 - x_3y_2, \; x_3y_1 - x_1y_3, \; x_1y_2 - x_2y_1)
$$

例： $ \vec a = (1,2,4), \vec b = (3,1,2),\vec c \perp \vec a且\vec c \perp \vec b,求\vec c的一个解. $ 
$$
\\
\begin{array}{c}
& 1 & 2 & 4 & 1 & 2 & 4 \\
& 3 & 1 & 2 & 3 & 1 & 2 \\
\end{array}
\\
\begin{aligned} 
\vec c &= (2*2-1*4,4*3 - 2*1,1*1-3*2)\\
&= (0,10,-5)\\
&= (0,2,-1)\\
\end{aligned}
$$

### 平面方程与点到平面距离公式

引入：

我们都知道直线方程 $ Ax+By+C = 0, $ 其中直线的法向量为 $ \vec n = (A,B). $ 

类似地 $ , $ 我们可以根据平面的法向量引入平面方程 $ , $ 即设平面方程 $ Ax+By+Cz+D = 0, $ 其中平面的法向量为 $ \vec n = (A,B,C). $ 

#### 平面方程

平面上任何一点坐标均满足平面方程 $ . $ 

一般式： $ Ax+By+Cz+D = 0, $ 其中 $ \vec{n} = (A,B,C) $ 为该平面的法向量 $ . $ 

点法式： $ A(x-x_0)+B(y-y_0)+C(z-z_0) = 0, $ 其中 $ (x_0,y_0,z_0) $ 为平面上任意一点坐标 $ . $ 

#### 点到平面距离公式

 $ \displaystyle d =  \frac{\left| Ax_1+By_1+Cz_1+D\right| }{\sqrt{A^2+B^2+C^2}} , $ 其中 $ (x_1,y_1,z_1) $ 为非平面上任意一点坐标 $ . $ 



例1：在正方体 $ ABCD-A_1B_1C_1D_1 $ 中 $ , $ 点 $ A(0,0,0),B(1,0,0),C(1,1,0),D(0,1,0) \\ A_1(0,0,1),B_1(1,1,0),C_1(1,1,1),D_1(0,1,1), $  $ P $ 是 $ B_1C $ 中点 $ , $ 求点 $ A_1 $ 到平面 $ BDP $ 的距离.
$$
设平面BDP法向量为\vec{n},易知\vec{n} = (1,1,-2). \\
所以平面BDP方程为x+y-2z-1 = 0\\
点A_1(0,0,1)到平面BDP的距离为d = \frac{\left| -2-1 \right| }{\sqrt{1+1+4}} = \frac{\sqrt{6}}{2}
$$

### 球体的体积与表面积公式推导

**所需前置知识：基本初等函数的定积分。**

- 体积公式的推导

  球体体积是两个半球体积之和.对于水平放置的半球 $ , $ 沿水平方向切成无数个小圆柱 $ , $ 所有圆柱的体积和即为半球体积.

$$
不妨设半球体半径为r,以半球心为顶点，竖直向上的距离为x.\\
对于每一个小圆柱,其底面积为\pi(r^2-x^2).\\
圆柱的高为x的微分,即\mathrm{d}x.\\
故每个小圆柱的体积为\pi(r^2-x^2)\mathrm{d}x.\\
其在[0,r]上的积分即为半球体积.\\
设半球体积为V'.\\
\begin{aligned}
V'&=\int_0^r(\pi(r^2-x^2)\mathrm{d}x)\\
&=\pi{r^3}-\int_0^r{x^2\mathrm{d}x}\\
&=\pi{r^3}-\frac{1}{3}\pi{r^3}\\
&=\frac{2}{3}\pi{r^3}.
\end{aligned}\\
所以球体体积V=2V'=\frac{4}{3}\pi{r^3}.
$$

- 表面积公式的推导

  对于球体 $ , $ 将其以球心为顶点切成无数个小圆锥 $ , $ 所有小圆锥的地面面积和即为球体表面积 $ S $ .同时 $ , $ 球体的体积可视为所有小圆锥的体积之和 $ , $ 有 $ \displaystyle \frac{1}{3}Sr=V=\frac{4}{2}\pi{r^3} $  $ , $ 易解得 $ S=4\pi{r^2} $ .

## 平面几何

### 复数与复平面



### 平面向量与解三角形

#### 极化恒等式

定理内容及推导：
$$
(\vec a + \vec b)^2 = |\vec a |^2 + 2\vec a \cdot \vec b + |\vec b |^2 ① \\
(\vec a - \vec b)^2 = |\vec a |^2 - 2\vec a \cdot \vec b + |\vec b |^2 ② \\
① - ②得: \\
\vec a \cdot \vec b = \frac{(\vec a + \vec b)^2}{4} - \frac{(\vec a - \vec b)^2}{4}
$$
例1：

在 $ \Delta ABC $ 中 $ \displaystyle ,AC=3,BC=4,C=\frac{\pi}{2},P\in $ 平面 $ ABC,PC=1, $ 则 $ \vec{PA}\cdot \vec{PB} $ 范围为多少
$$
本题的常规方法是参数方程、向量法等,但极化恒等式能够有效简化计算. \\
设D为AB中点. \\
\vec{PA}\cdot \vec{PB} = \frac{(\vec{PA}+\vec{PB})^2}{4} - \frac{(\vec{PA}-\vec{PB})^2}{4} \\
\vec{PA}+\vec{PB} = 2\vec{PD}, \vec{PA}-\vec{PB} = \vec{BA} \\
由题可知|\vec{BA}| = 5, \\
所以\vec{PA}\cdot \vec{PB} = |\vec{PD}|^2 - \frac{25}{4} \\
|PD| \in [|OD| - |PC|, |OD| + |PC|], \\
即|\vec{PD}| \in [\frac{3}{2},\frac{7}{2}], \\
\therefore \vec{PA}\cdot \vec{PB} \in [-4,6].
$$

#### 向量叉乘计算平行四边形和三角形面积

设向量 $ \vec{v_1},\vec{v_2} $ 的起点都在原点 $ O $ 处 $ , $ 则 $ \vec{v_1} $ 所在的直线方程为 $ \displaystyle l:y = \frac{y_1}{x_1}x $  $ , $ 化简得 $ y_1x-x_1y = 0 $  $ , $ 由点到直线距离公式 $ , $  $ \vec{v_2} $ 的终点到直线 $ l $ 的距离 $ \displaystyle d = \frac{|x_1y_2-x_2y_1|}{\sqrt{x_1^2+y_1^2}}; $ 又 $ |\vec{v_1}|=\sqrt{x_1^2+y_1^2}, $ 则有：
$$
S = d\cdot|\vec{v_1}| = \sqrt{x_1^2+y_1^2} = |x_1y_2-x_2y_1|.
$$
故平面中叉乘公式为 $ |\vec{v_1}\times\vec{v_2|} = |x_1y_2-x_2y_1|, $ 此公式即为平面中平行四边形面积.

注意：上式中两个 $ |\cdot\cdot\cdot| $ 意义不同 $ , $ 等号左边表示**向量的模** $ , $ 右边表示**绝对值**.

三角形面积为平行四边形的一半 $ , $ 故三角形面积公式为 $ S_{\triangle} = \frac{1}{2}|\vec{v_1}\times\vec{v_2|} = \frac{1}{2}|x_1y_2-x_2y_1|. $ 

#### 张角定理

### 平面解析几何

#### 直线的参数方程

- 定义：在直线 $ l $ 上，若存在一点 $ P(x_0,y_0) $  $ , $ 则可以设直线方程为
  $$
  \begin{cases}
  x = x_0 + tcos\theta \\
  y = y_0 + tsin\theta 
  \end{cases}
  $$
  其中 $ ,|t| $ 为直线上的点到 $ P $ 的长度.
  
  若 $ t>0, $ 则表示的点在 $ P $ 的上方 $ ; $ 
  
  若 $ t<0, $ 则表示的点在 $ P $ 的下方 $ ; $ 
  
  若 $ t=0, $ 则表示的点即为 $ P $ .

例1：已知直线 $ l $ 经过点 $ P(1,-3\sqrt{3}), $ 倾斜角为 $ \displaystyle \frac{\pi}{3}, $ 求直线 $ l $ 和圆 $ x^2+y^2=16 $ 的两个交点 $ A,B $ 与 $ P $ 点的距离之积.
$$
设直线l的方程为l:
\begin{cases}
\displaystyle x=1+\frac{1}{2}t \\
\displaystyle y=-3\sqrt{3}+\frac{\sqrt{3}}{2}t
\end{cases} \\
代入圆的方程x^2+y^2=16得: \\
(1+\frac{1}{2}t)^2 + (-3\sqrt{3}+\frac{\sqrt{3}}{2}t)^2 = 16 \\
整理得:t^2-8t+12=0 \\
易知\Delta>0,有|t_1| = |PA|, |t_2| = |PB|, \\
故|PA|\cdot|PB| = |t_1 t_2| = 12.
$$

例2：已知椭圆 $ \displaystyle C:\frac{x^2}{4}+\frac{y^2}{3}=1, $ 过点 $ P(-1,1) $ 且相互垂直的两条直线 $ l_1,l_2 $ 分别交椭圆 $ C $ 于 $ M,N $ 两点及 $ S,T $ 两点.求 $ \displaystyle \frac{|PM||PN|}{|PS||PT|} $ 的取值范围.
$$
设直线l1:
\begin{cases}
x=-1+t\cos\alpha \\
y=1+t\sin\alpha \\
\end{cases} \\
直线l2:
\begin{cases}
x=-1+t\cos(\alpha+\frac{\pi}{2}) \\
y=1+t\sin(\alpha+\frac{\pi}{2}) \\
\end{cases} \\
联立椭圆C和直线l_1得: \\
3(t\cos\alpha-1)^2+4(t\sin\alpha+1)^2 = 12 \\
整理得:(3\cos^2\alpha+4\sin^2\alpha)t^2+(8t\sin\alpha-6t\cos\alpha)t-5=0 \\
设t_1,t_2分别为M,N的参数,则有 \\
|PM||PN|=|t_1t_2|=\frac{5}{4\sin^2\alpha+3\cos^2\alpha} \\
同理可得|PS||PT|=\frac{5}{4\sin^2(\alpha+\frac{\pi}{2})+3\cos^2(\alpha+\frac{\pi}{2})}=\frac{5}{3\sin^2\alpha+4\cos^2\alpha} \\
故\frac{|PM||PN|}{|PS||PT|} = \frac{3\sin^2\alpha+4\cos^2\alpha}{4\sin^2\alpha+3\cos^2\alpha} \\
若\alpha=\frac{\pi}{2},则\frac{|PM||PN|}{|PS||PT|} = \frac{3}{4} \\
若\alpha \neq \frac{\pi}{2},则\frac{|PM||PN|}{|PS||PT|} = \frac{3\tan^2\alpha+4}{3+4\tan^2\alpha} = \frac{\frac{3}{4}(3+4\tan^2\alpha)+\frac{7}{4}}{3+4\tan^2\alpha} = \frac{3}{4}+\frac{7}{4(3+\tan^2\alpha)}\in \left(\frac{3}{4},\frac{4}{3}\right] \\
综上,\frac{|PM||PN|}{|PS||PT|} \in \left[\frac{3}{4},\frac{4}{3}\right] \\
$$

#### 曲线系

- 定义

  具有某种共同性质的曲线的集合，称为曲线系。在高中阶段，曲线系的共同性质一般是过几个定点。

- 一次曲线系(直线系)

  过定点 $ (m,n) $ 的直线系方程为 $ \lambda(x-m)+\mu(y-n)=0; $ 

  设直线 $ l_1,l_2, $ 则过这两条直线交点的直线系方程为 $ \lambda{l_1}+\mu{l_2}=0, $ 若所求直线不是 $ l_2, $ 可略去参数 $ \mu, $ 设方程为 $ \lambda{l_1}+l_2=0. $ 

- 二次曲线系

  - 退化二次曲线方程

    直线 $ l_1,l_2 $ 的集合为 $ l_1\cdot l_2=0. $ 显然方程展开后是二次方程 $ , $ 这就是退化二次曲线方程(两条直线的方程) $ . $ 

  - 圆系方程

    设圆 $ C_1,C_2, $ 则 $ \lambda{C_1}+\mu{C_2}=0 $ 为过两圆交点的圆系方程 $ . $ 当所求圆不是 $ C_2 $ 时 $ , $ 可略去参数 $ \mu, $ 设方程为 $ \lambda{C_1}+{C_2}=0.\lambda=-1 $ 时 $ , $ 该方程表示两圆的根轴方程.此时若两圆相交 $ , $ 则该方程表示两圆的交点弦方程 $ ; $ 若两圆相切 $ , $ 则该方程表示两圆的公切线方程 $ ; $ 若两圆相离 $ , $ 则该方程表示垂直于两圆连线的一条直线.

    设直线 $ l, $ 圆 $ C, $ 则经过直线与圆交点的圆系方程为 $ C+\lambda l=0. $ 

  - 其他方程
  
    与椭圆共焦点的曲线系方程为 $ \displaystyle \frac{x^2}{a^2+\lambda}+\frac{y^2}{b^2+\lambda} = 1; $ 
  
    与双曲线共焦点的曲线系方程为 $ \displaystyle \frac{x^2}{a^2+\lambda}-\frac{y^2}{b^2-\lambda} = 1; $ 
  
    同离心率圆锥曲线的曲线系为 $ \displaystyle \frac{x^2}{a^2} + \frac{y^2}{b^2} = \lambda; $ 
  
    过二次曲线 $ E_1:f_1(x,y)=0 $ 与 $ E_2:f_2(x,y)=0 $ 交点的曲线系方程为 $ \lambda{E_1}+\mu{E_2}=0, $ 若所求曲线不是 $ E_2, $ 可略去参数 $ \mu, $ 设方程为 $ \lambda{E_1}+E2=0. $ 
  
    若圆锥曲线 $ C $ 与直线 $ l_1,l_2 $ 相交 $ , $ 则过这些交点的曲线系方程为 $ l_1\cdot l_2+\lambda{C}=0. $ 
  
    若圆锥曲线 $ C $ 与直线 $ l $ 相交 $ , $ 则过这些交点的曲线系方程为 $ l^2+\lambda{C}=0. $ 

引例：若存在圆 $ C_1:x^2+y^2+6x-4=0 $ 和 $ C_2:x^2+y^2+6y-28=0, $ 求过这两个圆的交点且圆心在直线 $ x-y-4=0 $ 的圆的方程.
$$
不妨设过这两个圆的圆系方程x^2+y^2+6x-4+\lambda(x^2+y^2+6y-28)=0 \\
化简得(\lambda+1)x^2+(\lambda+1)y^2+6x+6\lambda{y}-28\lambda-4=0 \\
其圆心为(-\frac{3}{\lambda+1},-\frac{3\lambda}{\lambda+1}),满足直线方程x-y-4=0, \\
所以有-\frac{3}{\lambda+1}+\frac{3\lambda}{\lambda+1}-4=0, \\
解得\lambda=-7. \\
故所求圆的方程即为x^2+y^2-x+7y-32=0.
$$


例1：已知椭圆 $ \displaystyle C:\frac{x^2}{2}+y^2 = 1 $ 的一个顶点为 $ P(0,1). $ 过点 $ P $ 作斜率为 $ k_{1} $ 的直线 $ l_1 $ 交椭圆 $ C $ 于另一点 $ A, $ 过点 $ P $ 作斜率为 $ k_{2}(k_2\neq k_1) $ 的直线 $ l_2 $ 交椭圆 $ C $ 于另一点 $ B. $ 若 $ k_1k_2=1, $ 求证：直线 $ AB $ 经过定点.
$$
设直线l_{AB}:kx-y+m=0,l_1:k_1x-y+1=0,l_2:k_2x-y+1=0. \\
又点P处切线为y=1,故设经过P,A,B三点的曲线系方程为: \\
\lambda(y-1)(kx-y+m)+(k_1x-y+1)(k_2x-y+1) = 0 \\
其中x^2系数:k_1k_2,y^2系数:1-\lambda,常数项:1-m\lambda \\
又椭圆C:x^2+2y^2-2 = 0 \\
比对系数可得: \\
\frac{k_1k_2}{1-\lambda} = \frac{1}{2},\frac{k_1k_2}{1-m\lambda} = -\frac{1}{2},且k_1k_2=1 \\
可解得\lambda = -1,m=-3. \\
即l_{AB}:kx-y-3 = 0,易知该直线恒过点(0,-3). \\
$$
例2：(2011全国卷)已知 $ O $ 为坐标原点 $ ,F $ 为椭圆 $ \displaystyle x^2+\frac{y^2}{2}=1 $ 在 $ y $ 轴正半轴上的焦点 $ , $ 过 $ F $ 且斜率为 $ -\sqrt{2} $ 的直线 $ l $ 与 $ C $ 交于 $ A,B $ 两点 $ , $ 点 $ P $ 满足 $ \vec{OA}+\vec{OB}+\vec{OC}=\vec{0}. $ 若有一点 $ \displaystyle P(-\frac{\sqrt{2}}{2},-1), $ 设点 $ P $ 关于点 $ O $ 的对称点为 $ Q, $ 证明： $ A,P,B,Q $ 四点在同一圆上.
$$
易知直线AB的方程为l_{AB}:\sqrt{2}x+y-1=0,直线PQ的方程为l_{PQ}:\sqrt{2}x-y=0, \\
所以设过A,P,B,Q四点的曲线系方程为(\sqrt{2}x+y-1)(\sqrt{2}x-y)+\lambda(x^2+\frac{y^2}{2}-1)=0. \\
化简得:(\lambda+2)x^2+(\frac{\lambda}{2}-1)y^2-\sqrt{2}x-y-\lambda=0. \\
若这四个点在圆上,则上式为圆系方程,满足\lambda+2=\frac{\lambda}{2}-1, \\
解得\lambda=-6. \\
此时圆的方程为4x^2+4y^2+\sqrt{2}x-y-6=0,D^2+E^2-4F=27>0. \\
故存在圆4x^2+4y^2+\sqrt{2}x-y-6=0使A,P,B,Q在同一圆上.
$$

例3：(2021新高考Ⅰ卷)在平面直角坐标系 $ xOy $ 中 $ , $ 已知双曲线 $ \displaystyle C:x^2-\frac{y^2}{16}=1(x\geqslant1), $ 设点 $ T $ 在直线 $ \displaystyle x=\frac{1}{2} $ 上 $ , $ 过 $ T $ 的两条直线分别交 $ C $ 于 $ A,B $ 两点和 $ P,Q $ 两点 $ , $ 且 $ |TA|\cdot|TB|=|TP|\cdot|TQ|, $ 求直线 $ AB $ 的斜率与直线 $ PQ $ 的斜率之和.
$$
由题可知\frac{|TA|}{|TQ|}=\frac{|TP|}{|TB|},所以\triangle{TAP}\sim\triangle{TBQ},易知A,P,B,Q四点共圆. \\
设T(\frac{1}{2},t),l_{AB}:y=k_1(x-\frac{1}{2})+t,l_{PQ}:y=k_2(x-\frac{1}{2})+t \\
则过点A,P,B,Q的曲线系与双曲线方程满足下式: \\
\left(y-k_1(x-\frac{1}{2})+t\right)\left(y-k_2(x-\frac{1}{2})+t\right) = \lambda \left(x^2-\frac{y^2}{16}-1\right)\\
比对xy项:k_1+k_2=0. \\
故直线AB的斜率与直线PQ的斜率之和为0.
$$

例4：已知椭圆 $ E:\displaystyle \frac{x^2}{16}+\frac{y^2}{4}=1 $ 的一个顶点为 $ A(-4,0), $ 过点 $ P(2,1) $ 作斜率为 $ k $ 的直线 $ l, $ 交椭圆 $ E $ 于 $ B,C $ 两点 $ (B,C $ 不与 $ A $ 重合 $ ), $ 若直线 $ AB,AC $ 的斜率之积为 $ \displaystyle -\frac{1}{4}, $ 求 $ k $ 的值.
$$
设直线l:kx-y-2k+1=0,l_{AB}:k_1x-y+4k_1=0,l_{AC}:k_2x-y+4k_2=0. \\
又点A处切线为x=-4,故设经过P,A,B三点的曲线系方程为: \\
(k_1x-y+4k_1)(k_2x-y+4k_2)+\lambda(x+4)(kx-y-2k+1) = 0 \\
其中x^2系数:k_1k_2+\lambda k, y^2系数:1,常数项:16k_1k_2+4\lambda(1-2k) \\
又椭圆E:x^2+4y^2-16=0 \\
比对系数可得: \\
\frac{1}{k_1k_2+\lambda k} = 4,\frac{16k_1k_2+4\lambda(1-2k)}{1} = -4,且k_1k_2=-\frac{1}{4} \\
可解得\lambda=1,k=\frac{1}{2}.
$$

#### 仿射变换

#### 定比点差

- 定比点差是点差法的特殊情况 $ , $ 同时也是直线参数方程的变体.运用定比点差能够快速证明动点过定直线和点列共线等题目 $ , $ 可以说这是圆锥曲线中最高效也不失优雅的方法.

例1：已知椭圆 $ \displaystyle C:\frac{x^2}{4}+\frac{y^2}{3}=1, $ 若过点 $ P(4,0) $ 的直线 $ l $ 与椭圆交于 $ A,B, $ 点 $ Q $ 在直线 $ l $ 上(异于 $ P $ 点) $ , $ 且 $ \displaystyle \frac{|AP|}{|PB|} = \frac{|AQ|}{|QB|}. $ 证明：点 $ Q $ 在定直线上.
$$
由题意,设\frac{|PA|}{|AQ|} = \frac{|PB|}{|BQ|}=\lambda,
则\vec{PA} = \lambda\vec{AQ}, \vec{PB} = \lambda{BQ}. \\
设点A(x_1,y_1),B(x_2,y_2),Q(x,y). \\
由\vec{PA} = \lambda\vec{AQ}可得: \\
\begin{cases}
x_1-4 = \lambda(x-x_1) \\
y_1-1 = \lambda(y-y_1) \\
\end{cases} \\
解得A(\frac{4+\lambda{x}}{1+\lambda},\frac{1+\lambda{y}}{1+\lambda}). \\
同理可得B(\frac{4-\lambda{x}}{1-\lambda},\frac{1-\lambda{y}}{1-\lambda}). \\
因为A,B两点均在椭圆C上,所以分别代入得: \\
\begin{cases}
\displaystyle \frac{1}{4}\left(\frac{4+\lambda{x}}{1+\lambda}\right)^2 + \frac{1}{3}\left(\frac{1+\lambda{y}}{1+\lambda}\right)^2 = 1 \\
\displaystyle \frac{1}{4}\left(\frac{4-\lambda{x}}{1-\lambda}\right)^2 + \frac{1}{3}\left(\frac{1-\lambda{y}}{1-\lambda}\right)^2 = 1 \\
\end{cases} \\
展开得:
\begin{cases}
\displaystyle \frac{1}{4}(4+\lambda{x})^2+\frac{1}{3}(1+\lambda{y})^2 = (1+\lambda)^2 \cdot\cdot\cdot\cdot\cdot\cdot①\\
\displaystyle \frac{1}{4}(4-\lambda{x})^2+\frac{1}{3}(1-\lambda{y})^2 = (1-\lambda)^2 \cdot\cdot\cdot\cdot\cdot\cdot②\\
\end{cases} \\
①-②得:4\lambda{x}+\frac{4}{3}\lambda{y} = 4\lambda, \\
即x+\frac{y}{3}=1.
$$
例2：已知椭圆 $ \displaystyle C:\frac{x^2}{4}+\frac{y^2}{3}=1,A,B $ 为椭圆上两点 $ , $ 且满足 $ \displaystyle k_{OA}\cdot k_OB = -\frac{3}{4}, $ 存在一点 $ P $ 满足 $ \vec{OP} = 3\vec{PA}, $ 直线 $ PB $ 交椭圆于点 $ Q. $ 求 $ \displaystyle \frac{|BP|}{|BQ|} $ 的值.
$$
由题意,设\frac{|BP|}{|BQ|} = \lambda,即\vec{BP} = \lambda\vec{BQ},设A(x_1,y_1),B(x_2,y_2),Q(x,y). \\
由\vec{BP} = \lambda\vec{BQ}可得: \\
\begin{cases}
3x_1-x_2 = \lambda(x-x_2) \\
3y_1-y_2 = \lambda(y-y_2) \\
\end{cases} \\
解得Q(\frac{3x_1+(\lambda-1)x_2}{\lambda},\frac{3y_1+(\lambda-1)y_2}{\lambda}). \\
因为点Q在椭圆C上,代入得: \\
\frac{1}{4}\left(\frac{3x_1+(\lambda-1)x_2}{\lambda}\right)^2 + \frac{1}{3}\left(\frac{3y_1+(\lambda-1)y_2}{\lambda}\right)^2=1 \\
\frac{1}{4}\left(9x_1^2+6(\lambda-1)x_1x_2+(\lambda-1)^2x_2^2\right) + \frac{1}{3}\left(9y_1^2+6(\lambda-1)y_1y_2+(\lambda-1)^2y_2^2\right) = \lambda^2 \\
又因为k_{OA}\cdot k_OB = -\frac{3}{4} = \frac{y_1}{x_1}\cdot\frac{y_2}{x_2},即y_1y_2 = -\frac{3}{4}x_1x_2. \\
所以9\left(\frac{x_1^2}{4}+\frac{y_1^2}{3}\right) + (\lambda-1)^2\left(\frac{x_2^2}{4}+\frac{y_2^2}{3}\right) = \lambda^2 \\
即9+(\lambda-1)^2 = \lambda^2 \\
解得\lambda = 5. \\
所以\frac{|BP|}{|BQ|} = 5.
$$

例3：已知椭圆 $ \displaystyle C:\frac{x^2}{8}+\frac{y^2}{4} = 1 $ 的上顶点 $ D, $ 右焦点 $ F, $ 点 $ P(4,2). $ 过点 $ P $ 作直线 $ l $ 交 $ C $ 于 $ A,B $ 两点( $ A $ 在 $ P $ 与 $ B $ 之间) $ , $ 与直线 $ DF $ 交于点 $ Q, $ 若 $ \vec{PA}=\lambda_1\vec{PB},\vec{QA}=\lambda_2\vec{BQ}, $ 求 $ \lambda_1 - \lambda_2 $ 的值.
$$
本题显然能够使用调和系列的方法实现速解,但是却难以在大部分考试中拿到过程分, \\
然而定比点差则能够拿到严谨的证明步骤分,因此本题选用定比点差法展示其严谨性. \\
设A(x_1,x_2),B(x_2,y_2) \\
由\vec{PA}=\lambda_1\vec{PB}可得: \\
\begin{cases}
x_1-\lambda_1x_2=4(1-\lambda_1)\cdot\cdot\cdot\cdot\cdot\cdot① \\
y_1-\lambda_1y_2=2(1-\lambda_1)\cdot\cdot\cdot\cdot\cdot\cdot② \\
\end{cases} \\
因为A,B均在C上,所以有:
\begin{cases}
\displaystyle \frac{x_1^2}{8}+\frac{y_1^2}{4} = 1\cdot\cdot\cdot\cdot\cdot\cdot③ \\
\displaystyle \frac{\lambda_1^2 x_2^2}{8}+\frac{\lambda_1^2 y_2^2}{4} = \lambda_1^2 \cdot\cdot\cdot\cdot\cdot\cdot④ \\
\end{cases} \\
③-④得: \\
\frac{(x_1-\lambda_1x_2)(x_1+\lambda_1x_2)}{8} + \frac{(y_1-\lambda_1y_2)(y_1+\lambda_1y_2)}{4} = 1-\lambda_1^2 \\
将①②分别代入得: \\
\frac{4(1-\lambda_1)(x_1+\lambda_1x_2)}{8} + \frac{4(1-\lambda_1)(y_1+\lambda_1y_2)}{4} = 1-\lambda_1^2 \\
化简得: \\
x_1+y_1 = 2+2\lambda_1-\lambda_1x_2-\lambda_1y_2\cdot\cdot\cdot\cdot\cdot\cdot⑤ \\
由\vec{QA}=\lambda_2\vec{BQ}可解得: \\
Q(\frac{x_1+\lambda_2x_2}{1+\lambda_2},\frac{y_1+\lambda_2y_2}{1+\lambda_2}) \\
因为Q在直线DF:x+y=2上,故代入得: \\
x_1+y_1+\lambda_2x_2+\lambda_2y_2-2-2\lambda_2=0 \\
将⑤代入得: \\
2+2\lambda_1-\lambda_1x_2-\lambda_1y_2+\lambda_2x_2+\lambda_2y_2-2-2\lambda_2=0 \\
(\lambda_1-\lambda_2)(x_1+y_2-2)=0 \\
显然,若使得上式恒成立,则须使\lambda_1-\lambda_2=0.
$$

#### 调和系列

##### 调和点列

- 调和点列的定义

  设存在直线 $ AB, $ 线段 $ AB $ 上有一点 $ M,AB $ 的延长线上有一点 $ N, $ 满足 $ \displaystyle \frac{|AM|}{|MB|} = \frac{|AN|}{|NB|}. $ 则称 $ A,M,B,N $ 成调和点列 $ , $ 其中 $ A,B $ 调和分割线段 $ MN, $ 或 $ M,N $ 调和分割线段 $ AB. $ 

##### 极点极线

- 极点极线的定义

  对于圆锥曲线 $ C, $ 其所在平面内任意一点(极点)有唯一对应的极线 $ , $ 其满足极线方程.

  对于圆锥曲线 $ C $ 的一对极点极线 $ , $ 若过极点 $ P $ 引一条直线 $ l $ 与 $ C $ 交于点 $ M,N, $ 与极线交于点 $ Q, $ 则 $ P,M,Q,N $ 构成调和点列.

- 极点极线的性质与结论：在圆锥曲线 $ C $ (此处仅给出椭圆与双曲线)中 $ , $ 若有一点 $ P(x_0,y_0), $ 则其极线方程为 $ \displaystyle \frac{x_0x}{a^2} \pm \frac{y_0y}{b^2} = 1, $ 当

  ①：点 $ P $ 在圆锥曲线 $ C $ 上时 $ , $ 该方程与圆锥曲线 $ C $ 有一个交点 $ ; $ 此时该方程表示圆锥曲线 $ C $ 在点 $ P $ 处的切线方程.

  ②：点 $ P $ 在圆锥曲线 $ C $ 外部时 $ , $ 该方程与圆锥曲线 $ C $ 有两个交点 $ ; $ 此时该方程表示点 $ P $ 与圆锥曲线 $ C $ 的切点弦方程.

  ③：点 $ P $ 在圆锥曲线 $ C $ 内部时 $ , $ 该方程与圆锥曲线 $ C $ 没有交点.特别地 $ , $ 若点 $ P $ 为圆锥曲线 $ C $ 的一个焦点 $ , $ 则该方程表示该焦点所对应的一条准线.

- 下面推导在圆锥曲线 $ \displaystyle C:\frac{x^2}{a^2} \pm \frac{y^2}{b^2} = 1 $ 中的极线方程：

$$
设存在直线AB,线段AB上有一点M,AB的延长线上有一点N,满足\frac{|AM|}{|MB|} = \frac{|AN|}{|NB|}. \\
设A(x_1,y_1),B(x_2,y_2),\vec{AM} = \lambda\vec{MB}, \vec{AN} = -\lambda\vec{NB}. \\
易知M(\frac{x_1 + \lambda x_2}{1 + \lambda}, \frac{y_1 + \lambda y_2}{1 + \lambda}), N(\frac{x_1 - \lambda x_2}{1 - \lambda}, \frac{y_1 - \lambda y_2}{1 - \lambda}). \\
对于圆锥曲线C,有 \\
\begin{cases}
\displaystyle \frac{x_1^2}{a^2} \pm \frac{y_1^2}{b^2} = 1 \cdot\cdot\cdot\cdot\cdot\cdot①\\
\displaystyle \frac{x_2^2}{a^2} \pm \frac{y_2^2}{b^2} = 1 \cdot\cdot\cdot\cdot\cdot\cdot②\\
\end{cases} \\
①-\lambda^2②得: 
\frac{x_1^2-\lambda^2x_2^2}{a^2} \pm \frac{y_1^2-\lambda^2y_2^2}{b^2} = 1-\lambda^2 \\
利用平方差公式展开得:
\frac{(x_1+\lambda x_2)(x_1-\lambda x_2)}{a^2} \pm \frac{(y_1+\lambda y_2)(y_1-\lambda y_2)}{b^2} = 1-\lambda^2 \\
通过分析点M,N坐标可知 \\
x_1+\lambda x_2 = (1 + \lambda)x_M,\space\space\space x_1-\lambda x_2 = (1 - \lambda)x_N, \\
y_1+\lambda y_2 = (1 + \lambda)y_M,\space\space\space y_1-\lambda y_2 = (1 - \lambda)y_N, \\
上述等式可化为
\frac{x_M(1+\lambda)x_N(1-\lambda)}{a^2} \pm \frac{y_M(1+\lambda)y_N(1-\lambda)}{b^2} = 1-\lambda^2 \\
即\frac{x_M x_N}{a^2} \pm \frac{y_M y_N}{b^2} = 1 \\
所以点M的极线过N,点N的极线过M. \\
所以在圆锥曲线C中,若有一点P(x_0,y_0),则其极线方程为\frac{x_0x}{a^2} \pm \frac{y_0y}{b^2} = 1.
$$

- 配极原则：若点 $ P $ 在点 $ Q $ 的极线上 $ , $ 则点 $ Q $ 也在点 $ P $ 的极线上.
- 自极三角形：若在圆锥曲线 $ C $ 上存在一内接四边形 $ ABCD, $ 设对角线 $ AC,BD $ 交于点 $ P, $ 直线 $ AB,CD $ 的延长线交于点 $ Q, $ 直线 $ AD,BC $ 的延长线交于点 $ M, $ 则称三角形 $ PQM $ 为自极三角形.在自极三角形 $ PQM $ 中 $ , $ 其任意一顶点与对边称极点极线.

例1：(2020高考数学课标Ⅰ卷理科第20题)已知 $ A,B $ 分别为椭圆 $ E:\displaystyle \frac{x^2}{9} + y^2 = 1 $ 的左、右顶点 $ ,G $ 为 $ E $ 的上顶点 $ ,\vec{AG}\cdot \vec{GB} = 8,P $ 为直线 $ x=6 $ 上的动点 $ ,PA $ 与 $ E $ 的另一交点为 $ C,PB $ 与 $ E $ 的另一交点为 $ D. $ 证明：直线CD恒过定点.
$$
由题,设P(6,t) \\
代入极线方程\frac{x_0x}{a^2} + \frac{y_0y}{b^2} = 1得: \\
\frac{2x}{3}+ty = 1 \\
令y=0,解得x = \frac{3}{2}. \\
即直线CD恒过定点\left(\frac{3}{2},0\right).
$$

例2：在平面直角坐标系中 $ , $ 椭圆 $ \displaystyle E:\frac{x^2}{4} + y^2 = 1 $ 的左右两顶点分别为 $ A,B, $ 过点 $ M(-1,0) $ 斜率为 $ k $ 的直线交椭圆 $ E $ 于 $ C,D $ 两点 $ , $ 点 $ C $ 在 $ x $ 轴上方 $ . $ 记直线 $ AD,BC $ 的斜率分别为 $ k_1,k_2, $ 求证： $ \displaystyle \frac{k_1}{k_2} $ 为定值 $ . $ 
$$
点M若为极点,则其所对应的极线方程为x=-4 \\
由题意可知AB,CD交于点M(-1,0),由椭圆内接四边形结论可知直线AD,CB交点在M的极线上 \\
设直线AD,CB交于点P(-4,t) \\
k_1 = \frac{t}{-4+2} = \frac{t}{-2} \\
k_2 = \frac{t}{-4-2} = \frac{t}{-6} \\
\frac{k_1}{k_2} = \frac{t}{-2} \cdot \frac{-6}{t} = 3 \\
故\frac{k_1}{k_2}为定值3,证毕.
$$

例3：(2020北京卷)已知椭圆 $ \displaystyle C:\frac{x^2}{8}+\frac{y^2}{2}=1 $ 过点 $ A(-2,-1), $ 且过点 $ B(-4,0) $ 的直线 $ l $ 交椭圆 $ C $ 于点 $ M,N. $ 直线 $ MA,NA $ 分别交直线 $ x=-4 $ 于点 $ P,Q. $ 求 $ \displaystyle \frac{|PB|}{|BQ|} $ 的值.
$$
易知B的极线为x=-2过点A.设该直线于MN交于点Z.\\
BZ调和分割MN,\frac{|BN|}{|BM|}=\frac{|ZN|}{|ZM|}.\\
由ZA于PQ平行,得\frac{|BN|}{|ZN|}=\frac{|BQ|}{|AZ|},\frac{|BM|}{|ZM|}=\frac{|PB|}{|AZ|}.\\
解得|PB|=|BQ|,故\frac{|PB|}{|BQ|}=1.
$$

##### 任意二次曲线的极线方程

设圆锥曲线 $ \Gamma:Ax^2+By^2+Cxy+Dx+Ey+F = 0, $ 平面上任意一点 $ P(x_0,y_0), $ 则极点 $ P $ 关于圆锥曲线 $ \Gamma $ 的极线方程为：
$$
Ax_0x+By_0y+C\frac{x_0y+y_0x}{2}+D\frac{x_0+x}{2}+E\frac{y_0+y}{2}+F = 0.
$$
对于圆锥曲线的一般方程 $ f(x,y)=0, $ 点 $ P(x_0,y_0) $ 关于 $ \Gamma $ 的极线方程 $ , $ 即在 $ f(x,y)=0 $ 中：

- 将 $ x^2, y^2 $ 替换为 $ x_0x,y_0y $ 
- 将 $ xy $ 替换为 $ \frac{x_0y+y_0x}{2} $ 
- 将 $ x,y $ 替换为 $ \frac{x_0+x}{2},\frac{y_0+y}{2} $ 
- 常数项保持不变

##### 隐函数求导推导切线方程

$$
设圆锥曲线C的方程为C:\frac{x^2}{a^2} \pm \frac{y^2}{b^2} = 1. \\
方程两边对x求导得: \\
\frac{2x}{a^2} \pm \frac{2y \cdot y'}{b^2} = 0. \\
若点P(x_0,y_0)在C上,即\frac{x_0^2}{a^2} \pm \frac{y_0^2}{b^2} = 1,有:\\
\frac{2x_0}{a^2} \pm \frac{2y_0 \cdot y'}{b^2} = 0. 其中y'即为圆锥曲线在点P处的斜率\\
y' = \mp \frac{b^2}{a^2} \cdot \frac{x_0}{y_0} \\
所以直线l的方程为: \\
l:y-y_0 = \mp \frac{a^2x_0}{b^2y_0}(x-x_0) \\
\frac{x_0x}{a^2} \pm \frac{y_0y}{b^2} = \frac{x_0^2}{a^2} \pm \frac{y_0^2}{b^2} = 1 \\
即l:\frac{x_0x}{a^2} \pm \frac{y_0y}{b^2} = 1.
$$

##### 调和线束

- 调和线束的定义

  若点 $ A,M,B,N $ 构成调和点列 $ , $ 并从四点所在直线外任意一点分别向四点作直线 $ , $ 则这四条直线构成调和线束.

- 调和线束的性质

  对于调和线束 $ l_1,l_3,l_2,l_4, $ 从其交点外引一条任意直线与 $ l_1,l_3,l_2,l_4 $ 分别交于点 $ A,M,B,N, $ 则 $ A,M,B,N $ 构成调和点列.

  **特别地，平行线交于无穷远点。**


例1：(2020北京卷)已知椭圆 $ \displaystyle C:\frac{x^2}{8}+\frac{y^2}{2}=1 $ 过点 $ A(-2,-1), $ 且过点 $ B(-4,0) $ 的直线 $ l $ 交椭圆 $ C $ 于点 $ M,N. $ 直线 $ MA,NA $ 分别交直线 $ x=-4 $ 于点 $ P,Q. $ 求 $ \displaystyle \frac{|PB|}{|BQ|} $ 的值.
$$
易知B的极线为x=-2过点A.\\
设直线x=-2交BM与点Z,显然点B,N,Z,M构成调和点列.\\
设直线AM为l_1,AZ为l_2,AN为l_3,AB为l_4,直线x=-4为l'.\\
易知l_1,l_3,l_2,l_4构成调和线束.\\
设直线l_1,l_3,l_2,l_4分别于l'交于P,Q,E_{\infty},B.\\
由调和线束性质知P,Q,E_{\infty},B构成调和点列.\\
故\frac{|PE_{\infty}|}{|QE_{\infty}|}=\frac{|BQ|}{|BP|}=1.\\
$$

例2：(2022全国乙卷)已知椭圆 $ E $ 的方程为 $ \displaystyle \frac{x^2}{3}+\frac{y^2}{4}=1, $ 且过 $ \displaystyle A(0,-2),B(\frac{3}{2},-1) $ 两点.设过点 $ P(1,-2) $ 的直线交 $ E $ 于 $ M,N $ 两点 $ , $ 过 $ M $ 的且平行于 $ x $ 轴的直线与线段 $ AB $ 交于点 $ T, $ 点 $ H $ 满足 $ \vec{MT} = \vec{TH}. $ 证明：直线 $ HN $ 过定点.
$$

$$

#### 齐次化

##### 一般齐次化

- 在作答圆锥曲线题目时 $ , $ 可以利用二次齐次化方程来简化计算 $ , $ 减少计算量.齐次化方程常用来解答关于斜率之积或斜率之和等与斜率密切相关的一系列问题.

  例1：已知直线 $ y = kx+4 $ 与椭圆 $ \displaystyle \frac{x^2}{4} + y^2 = 1 $ 交于 $ A,B $ 两点 $ ,O $ 是坐标原点 $ . $ 若 $ k_{OA}+k_{OB} = 2, $ 求该直线的方程 $ . $ 

  - 第一种齐次化联立：经典方程 $ mx+ny=1. $ 

  $$
  易知直线不过原点，不妨设直线方程为mx+ny = 1. \\
  由题可知m = -\frac{k}{4},n = \frac{1}{4} \\
  椭圆方程可化为
  \frac{x^2}{4} + y^2 = (mx+ny)^2 \\
  整理得(4m^2-1)x^2 + (4n^2-4)y^2 + 8mnxy = 0 \\
  方程两边同时除以x^2得: \\
  (4n^2-4)\left(\frac{y}{x}\right)^2 + 8mn\left(\frac{y}{x}\right) + (4m^2-1) = 0 \\
  不难发现这是关于\frac{y}{x}的方程,设直线与椭圆交于A(x_1,y_1),B(x_2,y_2) \\
  由韦达定理可得: \frac{y_1}{x_1} + \frac{y_2}{x_2} = \frac{-8mn}{4n^2-4} \\
  又k_{OA} = \frac{y_1}{x_1}, k_{OB} = \frac{y_2}{x_2} \\
  所以k_{OA}+k_{OB} = \frac{-8mn}{4n^2-4} = 2 \\
  将m = -\frac{k}{4},n = \frac{1}{4}代入得:k=-15. \\
  故所求直线方程为y = -15x + 4.
  $$
  
  - 第二种齐次化联立：不设直线 $ , $ 直接代换
  
  $$
  设点A(x_1,y_1),B(x_2,y_2) \\
  由
  \begin{cases}
  y = kx + 4 \\
  \frac{x^2}{4} + y^2 = 1 \\
  \end{cases} ,得: \\
  \frac{y^2}{4} +y^2 = \left( \frac{y-kx}{4} \right)^2 \\
  化简得:15y^2+2kxy+(4-k^2)x^2=0 \\
  将方程两边同时除以x^2,得: \\
  15\left(\frac{y}{x}\right)^2 + 2k\left(\frac{y}{x}\right) + 4-k^2=0 \\
  由韦达定理可得:\frac{y_1}{x_1} + \frac{y_2}{x_2} = \frac{-2k}{15} = 2 \\
  解得k=-15. \\
  故所求直线方程为y = -15x + 4.
  $$

##### 构造齐次化

- 在齐次化的基础上用以解决直线交点不在原点的问题.

  例1：已知椭圆 $ \displaystyle C:\frac{x^2}{2}+y^2=1 $ 的一个顶点为 $ P(1,0). $ 过点 $ P $ 作斜率为 $ k_1 $ 的直线 $ l_1 $ 交椭圆 $ C $ 于另一点 $ A, $ 过点 $ P $ 作斜率为 $ k_2(k_2\neq k_1) $ 的直线 $ l_2 $ 交椭圆 $ C $ 于另一点 $ B. $ 若 $ k_1 k_2=1. $ 求证：直线 $ AB $ 经过定点.
  $$
  设直线l_{AB}:m(x-0)+n(y-1)=1 \\
  C:\frac{1}{2}x^2+(y-1+1)^2=1 \\
  即C:\frac{1}{2}x^2+(y-1)^2+2(y-1)=0 \\
  联立
  \begin{cases}
  l_{AB}:m(x-0)+n(y-1)=1 \\
  C:\frac{1}{2}x^2+(y-1)^2+2(y-1)=0 \\
  \end{cases}
  得: \\
  \frac{1}{2}x^2+(y-1)^2+2(y-1)\left(mx+n(y-1)\right)=0 \\
  化简得:(2n+1)(y-1)^2+2mx(y-1)+\frac{1}{2}x^2=0 \\
  等式两边同时除x^2得: \\
  (2n+1)(\frac{y-1}{x})^2+2m\frac{y-1}{x}+\frac{1}{2}=0 \\
  由韦达定理可得:k_1{k_2}=\frac{\frac{1}{2}}{2n+1}=1, \\
  解得n=-\frac{1}{4}. \\
  故直线l_{AB}:mx-\frac{1}{4}(y-1)=1恒过(0,-3).
  $$

- 

##### 平移齐次化

#### 圆锥曲线的统一极坐标方程

圆锥曲线 $ \Gamma $ 的统一极坐标方程为 $ \displaystyle \Gamma : \frac{ep}{1-e\cos\theta}, $ 其中 $ e $ 为离心率 $ ,\theta $ 为极角.

#### 阿波罗尼斯圆

#### 卡西尼卵形线

- 定义

  对于平面内两点 $ A,B, $ 且 $ AB=2c $ ( $ c $ 为定值) $ , $ 平面内满足 $ MA\cdot MB=a^2 $ ( $ a $ 是定值)的点 $ M $ 的轨迹称为卡西尼卵形线.若 $ A,B $ 位于平面直角坐标系 $ x $ 轴上 $ , $ 则图像关于 $ x $ 轴和 $ y $ 轴对称 $ , $ 且关于原点中心对称.

  -  $ a<c $ 时 $ , $ 图像分为两部分 $ , $ 每一部分均为闭合曲线.
  -  $ a=c $ 时 $ , $ 图像为伯努利双扭线 $ , $ 且图像经过原点.
  -  $ c<a<\sqrt{2}c $ 时 $ , $ 图像为闭合圆滑曲线 $ , $ 且曲线中部凹陷.
  -  $ a=\sqrt{2}c $ 时 $ , $ 图像为卵形.
  -  $ a>\sqrt{2}c $ 时 $ , $ 图像为闭合圆滑曲线 $ , $ 且曲线中部凸起.

![](https://pics6.baidu.com/feed/d01373f082025aaf4a75d388d30ee96c024f1a1d.jpeg@f_auto?token=bf28e58bf429e967d1a0af482162854f)

#### 内准圆/外准圆(蒙日圆)

##### 蒙日圆

- 定义：对于任意椭圆 $ C, $ 若从 $ C $ 外一点 $ P $ 作两条关于 $ C $ 切线 $ , $ 且这两条切线相互垂直,则 $ P $ 点的轨迹所形成的圆即为 $ C $ 的蒙日圆.

- 轨迹：对于椭圆 $ \displaystyle C:\frac{x^2}{a^2}+\frac{y^2}{b^2}=1, $ 其蒙日圆的轨迹方程为 $ x^2+y^2=a^2+b^2. $ 下面给出证明.
  $$
  设椭圆\displaystyle C:\frac{x^2}{a^2}+\frac{y^2}{b^2}=1以及C外一点P(x_0,y_0) \\
  设过点P的直线l:y-y_0=k(x-x_0). \\
  l斜率不存在时容易证明P在蒙日圆上,此处省略. \\
  联立l与C的方程.若满足l是C的切线,则有 \\
  \Delta = (a^2-x_0^2)k^2+2x_0y_0k+b^2-y_0^2=0 \\
  又k_1k_2=\frac{b^2-y_0^2}{a^2-x_0^2}=-1,即得 \\
  x_0^2+y_0^2=a^2+b^2 \\
  故满足要求的点P的轨迹方程为x^2+y^2=a^2+b^2. \\
  $$

##### 内准圆

- 定义：对于任意椭圆 $ C, $ 若从原点作两条互相垂直的直线分别交 $ C $ 于点 $ A,B, $ 并过原点作直线 $ AB $ 的垂线交直线 $ AB $ 于点 $ P, $ 则 $ P $ 点的轨迹所形成的圆即为 $ C $ 的内准圆.

- 轨迹：对于 $ \displaystyle C:\frac{x^2}{a^2}+\frac{y^2}{b^2}=1, $ 其内准圆的轨迹方程为 $ \displaystyle x^2+y^2=\frac{a^2b^2}{a^2+b^2}. $ 下面给出证明.
  $$
  设椭圆C:\frac{x^2}{a^2}+\frac{y^2}{b^2}=1以及直线l:mx+ny=1 \\
  原点到l距离d=\frac{1}{\sqrt{m^2+n^2}} \\
  联立l与C得: \\
  (\frac{1}{b^2}-n^2)y^2-2mnxy+(\frac{1}{a^2}-m^2)x^2 = 0 \\
  方程两边同时除x^2得: \\
  (\frac{1}{b^2}-n^2)\left(\frac{y}{x}\right)^2-2mn\left(\frac{y}{x}\right)+(\frac{1}{a^2}-m^2) = 0 \\
  若满足l_{OA} \perp l_{OB},则有k_1k_2=\frac{\frac{1}{a^2}-m^2}{\frac{1}{b^2}-n^2}=-1,即 \\
  m^2+n^2 = \frac{1}{a^2}+\frac{1}{b^2} \\
  代入d得:d=\frac{1}{\sqrt{\frac{1}{a^2}+\frac{1}{b^2}}}=\sqrt{\frac{a^2b^2}{a^2+b^2}} \\
  易知此时d即为C的内准圆半径,故内准圆方程为x^2+y^2=\frac{a^2b^2}{a^2+b^2}.
  $$

#### 圆锥曲线的光学性质

此小结所述内容用解析法证明略为复杂 $ , $ 可参考《圆锥曲线论》中的几何法证明.

##### 椭圆的光学性质

- 在椭圆中 $ , $ 从一个焦点出发的光线经椭圆反射后 $ , $ 一定经过椭圆的另一个焦点.

  该结论可拓展到三维中.即在椭球(椭圆绕长轴旋转所称图形)中 $ , $ 从一个焦点出发的光线经椭球反射后 $ , $ 也一定经过椭球的另一个焦点.

##### 双曲线的光学性质

- 在双曲线中 $ , $ 从一个焦点出发的光线经双曲线反射后 $ , $ 反射光线的反向延长线一定经过双曲线的另一个焦点.

  该结论仍可拓展到三维中.即在双叶双曲面(双曲线绕实轴旋转所称图形)中 $ , $ 从一个焦点出发的光线经该曲面反射后 $ , $ 反射光线的反向延长线一定经过该曲面的另一个焦点.

##### 抛物线的光学性质

- 在抛物线中 $ , $ 从焦点出发的光线经抛物线反射后 $ , $ 一定与准线垂直 $ , $ 即与抛物线的对称轴平行.

  该结论仍可拓展到三维中.即在抛物面(抛物线绕对称轴旋转所称图形)中 $ , $ 从焦点出发的光线经抛物面反射后 $ , $ 一定与抛物面的顶点与焦点所在直线平行.

#### 常见定理

##### 圆幂定理

- 对于一个圆 $ O, $ 从直线外一点 $ P $ 引两条直线分别交 $ O $ 于 $ A,B;C,D $ 四点 $ , $ 则有 $ |TA|\cdot|TB|=|TC|\cdot|TD|. $ 

##### 塞瓦定理

##### 梅涅劳斯定理

##### 彭赛列闭合定理

##### 帕斯卡定理

##### 蝴蝶定理

## 统计学与概率论