# 一种解决TSP问题的遗传算法

我们的团队有三人，其分工如下：

* 张强（1911082231）：进行了理论研究，完成了实验Python代码实现和实验报告的编写
* 邱起璐（1911082062）：进行了理论研究并进行汇报
* 朱峰（1912082254）：进行了理论研究并制作ppt

## 1.前言

### 1.1遗传算法

​		自从1975年Holland提出遗传算法（GA）到现在，遗传算法已经有很多年的发展历史。进化算法最初是借鉴了进化生物学中的一些现象而发展起来的，这些现象包括遗传、突变、自然选择以及杂交等。这项技术在计算机自动设计 （CAD, Computer-Automated Design），工业工程与运作管理，物流系统设计，生产调度和制造系统控制[1]等方面有着非常多的应用。

### 1.2 旅行商（TSP）问题

给定一系列城市和每对城市之间的距离，求解访问每一座城市一次并回到起始城市的最短回路。它是组合优化中的一个NP困难问题，在运筹学和理论计算机科学中非常重要。问题在1930年首次被形式化，并且是在最优化中研究最深入的问题之一。许多优化方法都用它作为一个基准。尽管问题在计算上很困难，但已经有了大量的启发式和精确算法。本文则采用一种启发式的遗传算法来解决此问题

## 2.本文算法流程

* 1) 根据编码规则初始化N个个体的种群。
* 2) 若满足停止条件则停止，否则继续执行。
* 3) 对当前种群进行统计分析，比如记录其最优个体、平均适应度等等。
* 4) 独立地从当前种群中选取N个母体。
* 5) 独立地对这N个母体进行交叉操作。
* 6) 独立地对这N个交叉后的个体进行变异。
* 7) 将父代种群和交叉变异得到的种群进行合并，得到规模为2N的种群。
* 8) 从合并的种群中根据选择算法选择出N个个体，得到新一代种群。
* 9) 回到第2步。

## 3.提出的交叉操作

### 3.2对论文提出的交叉操作的质疑

在复现的过程中，我尝试了父染色体P1=[4 1 2 3 0],P2=[3 4 0 1 2]，发现算法对这个例子是有缺陷的



## 4.实验分析





## 5.参考

[1]. Wikipedia https://zh.wikipedia.org/wiki/遗传算法

[2]. Wikipedia https://zh.wikipedia.org/wiki/旅行推销员问题

[3].https://github.com/mehdirazarajani/Genetic-Algorithm-for-Traveling-Salesman-Problem-with-Modified-Cycle-Crossover-Operator-Report 

[4].https://towardsdatascience.com/evolution-of-a-salesman-a-complete-genetic-algorithm-tutorial-for-python-6fe5d2b3ca35
