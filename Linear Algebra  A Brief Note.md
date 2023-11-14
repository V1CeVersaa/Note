# Linear Algebra : A Brief Note

***Subspaces***

A subset $U$ of $V$ is called a subspace of $V$ if and only if $U$ is a linear space, which has the same additive identity, addition, and scalar multiplication as on $V$.We only have to make sure that:

- Additive identity: $0\in U$;
- Closeness under addition: $u,v\in U \iff u+v\in U$
- Closeness under scalar multiplication: $a\in\mathbf{F},u\in U\iff au\in U$

**由于$U,V$公用相同的运算：向量加法和标量乘法，所以运算中的性质自然而然“遗传到”子空间$U$之中，所以加法的交换律、结合律与标量乘法的结合律与分配律也被“遗传”下去，自然不用验证。**

***Sums and direct sums of subspaces***

Suppose $V_1,\dots,V_m$ are subspaces of $V$. The sum of $V_1,\dots V_m$ denoted by $V_1+\dots+V_m$ is the set of all possible sums of elements of $V_1,\dots ,V_m$. More precisely,  $V_1+\dots +V_m = \left\{ v_1+v_2+\dots +v_m: v_1\in V_1,\dots v_m\in V_m\right\}$, besides, $V_1,\dots ,V_m$ is the *smallest* subspace of $V$ containing $V_1,\dots ,V_m$.

Moreover, if each element of $V_1+\dots+V_m$ can be written in only one way as a sum $v_1+\dots+v_m$ , where each $v_k\in V_k$ , $V_1+\dots+V_m$ is called a *direct sum*. We use the notation $V_1\oplus \cdots \oplus V_m$ to imply $V_1+\dots+V_m$ is a direct sum.

**值得注意的是，$V_1\oplus V_2=V_1 \oplus V_3$ 并不能表明$V_2 = V_3$，亦即和与直和并不满足消去律，反过来想，直和运算并不存在唯一的逆元，这就无法支撑消去律**

我们还有另外一种方式来定义直和：对于子空间$V_1,V_2$ ，如果$V_1\cap V_2 = \{0\}$,  则$V_1+V_2$ 是直和。对于多个线性子空间直和的情况，这种定义也有下面的推广：$\displaystyle W_1 = W_1\oplus W_2\oplus\cdots\oplus W_n$$\iff W_1\cap\sum_{j\neq i}W_j=\{0\}$并且有以下等价命题：

-  $W_1+W_2$是直和，亦即$W_1\cap W_2 = {0}$；
-  $W_1+W_2$内的每个向量$\alpha$的分解式$\alpha = \alpha_1+\alpha_2 $,$(\alpha_1\in W_1,\alpha_2\in W_2)$唯一；
-  零向量的分解式 $\mathbf{0}=\alpha_1+\alpha_2$,$(\alpha_1\in W_1,\alpha_2\in W_2)$当且仅当$\alpha_1=\alpha_2= 0$ 时成立；
-  $\dim(W_1+W_2)=\dim W_1+\dim W_2$；

*Linear Algebra Done Right* 中给出了等价命题（3）的推广形式：

Suppose $𝑉_1,\cdots,𝑉_𝑚$ are subspaces of $𝑉$. Then $𝑉_1+\cdots+𝑉_𝑚$ is a direct sum if
and only if the only way to write $0$ as a sum $𝑣_1+\cdots+𝑣_𝑚$, where each $𝑣_𝑘\in  𝑉_𝑘$ , is by taking each $𝑣_𝑘$ equal to $0$.

***Linear combinations and span***

A linear combination of list $v_1,\dots,v_m$ of vectors in $V$ is a vector of the form $a_1v_1+\cdots+a_mv_m$ , where $a_1,\dots,a_m\in\mathbf{F}$.

The set of all linear combintions of a list of vectors $v_1,\dots,v_m$ in $V$ is called the *span* of $v_1,\dots,v_m$ , denoted by $span\langle v_1,\dots,v_m\rangle$. In other words, $span\langle v_1,\dots,v_m\rangle=\{a_1v_1+\cdots+a_mv_m:a_1,\dots,a_m\in\mathbf{F}\}$

The span of empty list $\langle\ \rangle$ is defined to be $\{0\}$.

If $span\langle v_1,\dots,v_m\rangle=V$, we say the list *$v_1,\dots,v_m$ spans $V$*.

The span of a list of vectors in $V$ is the smallest subspace containing all the vectors in the list.

A vector space is called a ***finite-dimensional vector space*** if and only if some list of vectors in it spans the space. On the contary, if a vector space is not finite-dimensional, then it is called ***infinite-dimensional***.

Defintion of polynomial 

***Linear dependence***

If 

In a finite-dimensional vector space, the length of every linearly independent list of vectors is **less than or equal to** the length of every spanning list of vectors.

Every subspace of a finite-dimensional vector space is finite-dimensional.

***Bases***

A ***basis*** of $V$ is a list of vectors in $V$ that is linear independent and spans $V$. 

A list $v_1,\dots,v_m$ of vectors in $V$ is a basis of $V$ if and only if every $v\in V$ can be written **uniquely** in the form $v = a_1v_1+\cdots+a_mv_m$, where $a_1,\dots,a_m\in\mathbf{F}$.

Every *spanning list* in a vector space can be reduced to a basis of the vector space.

Every linear independent list of vectors in a finite-dimensional space can be extended to a basis of the vector space.

Suppose $V$ is finite-dimensional and $U$ is a subspace of $V$ . Then there is a subspace $W$ of $V$ such that $V = U\oplus W$. In short, every subspace of $V$ is part of a direct sum equal to $V$. (We can analyse the basis of $U$ and $W$.)

***Dimension***

Any two bases of a finite-dimensional vector space have the same length.

The ***dimension*** of a finite-dimensional vector space is the length of any basis of the vector space. The dimension of a finite-dimensional vector space $V$ is denoted by ***$\dim V$***.

If $V$ is finite-dimensional and $U$ is a subspace of $V$, then $\dim U\leq\dim V$.



  



