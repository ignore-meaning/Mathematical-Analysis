# 数学分析

重写自《数学分析》(卓里奇)。

目标是在不降低做题效率（原有的数学工具需要得到保留）的前提下使定义更加严谨。

最新的 pdf 版见根目录下的 `Analysis.pdf` 文件

以下是一些对应章节的碎碎念

## 准备工作

### 广义实数

开头就引入正负无穷 $\pm \infty$ 显然对初学者是不友好的（毕竟认识并理解无穷是整个第三章的重要目标之一）。而且很多与实数关联的性质、二元运算、二元关系对于无穷能不能用也没有讲清楚，既没说可以，也没说不可以。实际上在后文中我不言自明地用了 “任意实数都小于正无穷，大于负无穷”，但我还没想好这一部分的知识在什么地方写，写到什么程度。

另一个值得一提的是 “邻域” 这个概念（虽然这个名词并没有出现），我这里写的 $\mathring{U}_E^\delta(a)$ 允许 $a = +\infty$，但是失去了 “$\delta$ 越小区间长度越小的性质”，我在考虑是否应当这么定义：

$$
U^\delta(+\infty) := \left(\frac{1}{\delta}, +\infty\right)
$$



### 函数

这一部分主要是实数、函数、函数集之间的运算。这一部分函数之间的运算的定义有很大的问题，举个例子，实际上 $D(f/g) \neq D(f) \cap D(g)$ 因为还要保证 $g(x) \neq 0$，但我还没想好怎么完善它。定义三也只是给出一个例子（虽然我觉得通过例子应该能让人挺明白的），距离“严谨”还差了十万八千里。

## 极限

涉及到极限时我遇到了一个无关乎数学，在于语言表述的问题。“对于...如果...则...被称为...”这种表述是否科学。例如，当我在定理里面写到 $\lim(f,a)$ 是否已经体现出 $f$ 是函数而 $a$ 是其定义域的一个极限点了，当我写 $\lim(f,a) = A$ 时是否隐含着 $\lim(f,a)$ 存在的信息了？

### 数列的极限

这一部分我写得比较满意，还值得商榷的地方是关于无穷级数的定义。

### 函数的极限

最大的创新是关于 $o(g)$ 的定义。

正常情况下小o里面应该是一个函数（暂且不考虑函数集），但是我们常用的形式反而是 $o(x^2)$。当然，这代表着一个二次函数 $f:\mathbb{R} \rightarrow \mathbb{R}, x \mapsto x^2$，但总感觉怪怪的。一个（可能更加奇怪但）可行的方法是用 $o\bigl(\mathrm{id}^2\bigr)$ 来代替 $o(x^2)$，其中 $\mathrm{id}$ 指代恒等映射。

## 连续函数

无
