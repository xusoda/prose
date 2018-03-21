# Mathematics
-----
### Affine Space
>&emsp;&emsp;一种欧式空间的推广,即没有原点的向量空间

### Affine Transformation 
>&emsp;&emsp;also **affine map** or **affinity**  
&emsp;&emsp;一个向量空间进行一次线性变换并进行一次平移，变换为另一个向量空间  
&emsp;&emsp;如：$ \vec a = A\vec b + \vec c$ 即为一个仿射变换，$\vec b$ 通过矩阵“$A$”进行了一次线性变换，并通过$\vec c$进行了平移

### Affine Function
>&emsp;&emsp;在一个$\mathbb{R}^n$到$\mathbb{R}^m$仿射变换中，A为m*n的矩阵，b为m维向量，当m=1时，此变换为一个仿射函数

----------

### Exponential Family
>&emsp;&emsp;可以表达为特定形式的概率分布（这主要为了基于一些代数特性上的方便）  
&emsp;&emsp;常见的指数族分布：normal，exponential，gamma，chi-squared，beta，Dirichlet，Bernoulli，categorical，Poisson，Wishart，inverse Wishart，geometric  
&emsp;&emsp;指数族分布是PDF可以表达为如下形式的概率分布集合：  
&emsp;&emsp;$f_x(x|\theta)=h(x)e^{\eta(\theta)T(x)-A(x)}$  
&emsp;&emsp;$\theta$是参数Nature Parameter，$h(x)$是underlying measure底层观测值，$T(x)$是充分统计量Sufficient Statistic（通常$T(x)=x$)， $A(x)$是归一化常量Normalization Constant

-------

### MLE x MAP
>$X$为iid数据的一组抽样$X=(x_1,x_2...x_n)$:  
**MLE**:  
&emsp;$\hat\theta_{mle} = argmaxP(X;\theta)$  
&emsp;&emsp;&emsp;&emsp;$=argmin-\sum_{i=i}^{n}logP(x_i;\theta)$  
**MAP**:  
&emsp;$\hat\theta_{map}=argmaxP(\theta|X)$  
&emsp;&emsp;&emsp;&emsp; $=argmaxP(X|\theta)P(\theta)/P(X)$  
&emsp;&emsp;&emsp;&emsp; $=argmin-\sum_{i=i}^{n}logP(x_i;\theta)-logP(\theta)$  
&emsp;**当$\theta \sim N(0,\sigma^2): $**  
&emsp;$P(\theta)=\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{\theta^2}{2\sigma^2}}$  
&emsp;$-logP(\theta)=-log\frac{1}{\sqrt{2\pi}\sigma} +\frac{\theta^2}{2\sigma^2}$  
&emsp;其形式等价于MLE with L2 Regularization  
&emsp;MLE做的是经验风险最小化（Empricial Risk Minimization）。而MAP则是将模型复杂度作为先验概率的结构风险最小化（Structural Risk Minimization）  
>>结构风险=经验风险+置信风险  
经验风险可以由对已知样本的误差来表示，而置信风险则与已知样本数量成反比（样本越多，置信风险越小）、与目标函数VC Dimension成正比（目标函数可能性越多，复杂，推广能力越差，风险越大）

---------
### Analytical Solution && Numerical Solution
>Analytical Solution(closed-form solution):  
&emsp;use general symbolic manipulations
Numerical Solution:  
&emsp;use numerical approximation

-----
### 频率学派 x 贝叶斯
>频率学派通过总体信息和样本信息进行推断，贝叶斯通过总体信息，样本信息，以及先验信息推断。  
频率学派认为待估参数虽然是未知的，但是为常数。贝叶斯学派认为待估参数是变化的随机变量（它的分布为先验分布）

-----------
