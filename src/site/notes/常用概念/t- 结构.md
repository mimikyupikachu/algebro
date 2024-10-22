---
{"dg-publish":true,"permalink":"/常用概念/t- 结构/","dgPassFrontmatter":true,"created":"2024-10-21T08:00:44.856+08:00","updated":"2024-10-22T12:07:47.995+08:00"}
---

 $t$- 结构: 三角范畴 $\mathcal{D}$ 上的 $t$- 结构是指 $(\mathcal{D}^{\leqslant0},\mathcal{D}^{\geqslant0})$. 满足如下条件:
$\qquad$ 🄋  $\mathcal{D}^{\leqslant0}$ 和 $\mathcal{D}^{\geqslant0}$ 是 $\mathcal{D}$ 的同构封闭的满子范畴,  $\mathcal{D}^{\leqslant n}:=T^{-n}\mathcal{D}^{\leqslant0}$,  $\mathcal{D}^{\geqslant n}:=T^{-n}\mathcal{D}^{\geqslant0}$;
$\qquad$ ①  $\operatorname{Hom}_\mathcal{D}(\mathcal{D}^{\leqslant0},\mathcal{D}^{\geqslant 1})=0$.
$\qquad$ ②  $\mathcal{D}^{\leqslant0}\subseteq \mathcal{D}^{\leqslant1}$, 即 $\mathcal{D}^{\leqslant0}$ 对 $T$ 封闭; $\mathcal{D}^{\geqslant1}\subseteq \mathcal{D}^{\geqslant0}$, 即 $\mathcal{D}^{\geqslant0}$ 对 $T^{-1}$ 封闭.
$\qquad$ ③ 对 $\forall X \in \mathcal{D}$, 存在好三角 $A \rightarrow X \rightarrow B \rightarrow A[1]$. 其中 $A \in \mathcal{D}^{\leqslant0}$,  $B \in \mathcal{D}^{\geqslant1}$.

 $t$- 结构的心 the heart of the t-structure.  $\mathcal{H}:=\mathcal{D}^{\leqslant0} \cap \mathcal{D}^{\geqslant0}$. 是一个阿贝尔范畴. 