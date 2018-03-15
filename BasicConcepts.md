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

### Exponential family
>&emsp;&emsp;可以表达为特定形式的概率分布（这主要为了基于一些代数特性上的方便）
&emsp;&emsp;常见的指数族分布：normal，exponential，gamma，chi-squared，beta，Dirichlet，Bernoulli，categorical，Poisson，Wishart，inverse Wishart，geometric
指数族分布是PDF可以表达为如下形式的概率分布集合：  

&emsp;&emsp;$f_x(x|\theta)=h(x)e^{\eta(\theta)T(x)-A(x)}$&emsp;
&emsp;&emsp;$\theta$是参数nature parameter，$h(x)$是underlying measure底层观测值，$T(x)$是充分统计量sufficient statistic（通常$T(x)=x$)， $A(x)$是对数正则参数log normalizer

-------




