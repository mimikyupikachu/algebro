---
{"dg-publish":true,"permalink":"/Books/范畴论中若干基本概念和结论/7 可表函子和 Yoneda 引理/","dgPassFrontmatter":true,"created":"2024-07-06T09:51:11.606+08:00","updated":"2024-07-08T18:15:52.053+08:00"}
---

**可表函子(representable functor)**: 共变函子 $F:\mathcal{C}\rightarrow \mathrm{Set}$ 满足存在对象 $X \in \mathcal{C}$ 使得 $F\cong \mathrm{Hom}_{\mathcal{C}}(X,-)$, 此时称 $X$ 为函子 $F$ 的一个代表. 或反变函子 $G:\mathcal{C}\rightarrow \mathrm{Set}$ 满足存在对象 $Y \in \mathcal{C}$ 使得 $G\cong \mathrm{Hom}_{\mathcal{C}}(-.Y)$, 此时称 $Y$ 为函子 $G$ 的一个代表.

记 $h^{X}:=\mathrm{Hom}_{\mathcal{C}}(X,-),\quad h_{X}:=\mathrm{Hom}_{\mathcal{C}}(-,X)$.

记 $[h^{X},T]=\mathrm{Nat}(h^{X},T),\quad [h_{X},S]=\mathrm{Nat}(h_{X},S)$.

可表函子在同构意义下唯一.

**米田引理(Yoneda lemma)**: 
$\qquad$ 共变函子 $T:\mathcal{C}\rightarrow \mathrm{Set}$, 有双射 $[h^{X},T]\rightarrow TX,\quad \eta\mapsto\eta_{X}(\mathrm{Id}_{X})$;
$\qquad$ 反变函子 $S:\mathcal{C}\rightarrow \mathrm{Set}$, 有双射 $[h_{X},S]\rightarrow SX,\quad \eta\mapsto\eta_{X}(\mathrm{Id}_{X})$;