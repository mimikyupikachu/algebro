---
{"dg-publish":true,"permalink":"/常用概念/根 radical/","dgPassFrontmatter":true,"created":"2024-09-13T21:20:27.641+08:00","updated":"2024-10-22T12:09:18.968+08:00"}
---

# Ideals, Varieties, and Algorithms

称理想 $I$ 是 radical, 满足: 若多项式的某次幂 $f^m$ 在理想 $I$ 中, 则 $f$ 也在 $I$ 中.

仿射簇生成的理想总是根.  $\mathbf{I}(V)$ is always a radical ideal.

# 数学辞海第二卷

环的所有本原理想之交, 等于一切左本原理想的交, 等于最大的右拟正则理想(包含一切[[常用概念/不常用概念/拟正则理想#^e4957c\|右拟正则右理想]]), 等于最大的左拟正则理想(包含一切左拟正则左理想), 等于一切模的极大右理想之交, 等于一切模的极大左理想的交, 等于 $\{ x \in R\,|\,xa\,是右拟正则\,,\,\forall a \in R \}$.

# 群与代数表示引论

有限维 $F$- 代数 $A$ 的最大幂零理想称为 $A$ 的 Jacobson 根, 记作 $\operatorname{rad}A$.
+ 是 $A$ 的所有极大理想之交.
+ 是 $A$ 的所有极大左理想之交.
+ 是 $A$ 的所有极大右理想之交.
+ 是 $A$ 的最大拟正则理想.
+ 是 $A$ 的最大拟正则左理想.
+ 是 $A$ 的最大拟正则右理想.
+  $\operatorname{rad}(A)=\underset{S}{\cap}\operatorname{ann}(S)$, $S$ 取遍单模.

# [[0rigin/有限维代数\|有限维代数]]


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/books//3-the-radical/3-1/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




根(radical)是一个理想, 关于它的商代数是半单的. 且根是具有此性质的最小的理想. 即若 $A/I$ 是半单的, 则 $I\supset \mathrm{rad\ }A$.
###### 模的根

a measure of how far it is from being semisimple 半单性的度量:  $\mathrm{rad\ }M:=\{ m \in M\ |\ \forall f:M\rightarrow S,\ f(m)=0 \}$. 如果 $M$ 是半单模, 则 $M$ 可以写成单模直和的形式. 对于非零的 $m$, 总有一个投影使得 $f(m)\neq m$. 所以半单模的根是0.

对于上述的 $f$,  $\mathrm{Ker\ }f$ 总是 $M$ 的极大子模(因为是到单模的同态). 反过来对于极大子模 $M'$, 总能找到到单模的 $M\stackrel{f}{\longrightarrow}M/M'$, 使得 $\mathrm{Ker\ }f=M'$. 所以根也是**极大子模**之交.

**定理3.1.1.1**: $M$ 是半单模当且仅当 $\mathrm{rad\ }M=0$.

**定理3.1.1.2**: 任意形如 $M/\mathrm{rad\ }M$ 的商模都是半单模.

**命题3.1.2**: 根的直和等于直和的根:  $\mathrm{rad\ }(\underset{i=1}{\overset{s}\oplus}M_i)=\underset{i=1}{\overset{s}\oplus}(\mathrm{rad\ }M_i)$.

**命题3.1.3**: 对于任意模同态 $f:M\rightarrow N$,  $f(\mathrm{rad\ }M)\subset \mathrm{rad\ }N$. 由此**诱导同态(induced homomorphism)** $\widetilde{f}:M/\mathrm{rad\ }M\rightarrow N/\mathrm{rad\ }N,\ \ m+\mathrm{rad\ }M\mapsto f(m)+\mathrm{rad\ }N$.

**引理3.1.4(Nakayama)**:  $f:M\rightarrow N$ 是 $A$- 模满同态当且仅当诱导 $A$- 模同态 $\widetilde{f}:\operatorname{top}M\rightarrow \operatorname{top}N$ 是满同态.

给出了一个验证满同态的方法: 模根(modulo the radical).

根的子模都是[[Books/环与模范畴/Ⅱ. 直和与直积/5. 直和项#^4d82dd\|多余子模]].

 $M\mathrm{rad\ }A$ 是 $M$ 的子模中, 使得对应商模是半单模的, 极小子模.

###### 代数的根

代数 $A$ 的正则模的根就是代数 $A$ 的根.

**定理3.1.6**: 若模 $M$ 是 $A$- 模, 则 $\mathrm{rad\ }M=M\mathrm{rad\ }A$. 代数的根是双边理想且关于根的商代数是半单代数.

**推论3.1.7.1**: $A$ 的半单模都是商代数 $\bar{A}=A/\mathrm{rad\ }A$ 上的模.<font color=CadetBlue>(因为$\mathrm{rad\ }M=M\mathrm{rad\ }A=0$, 所以 $\mathrm{rad\ }A$ 零化了 $M$. 所以商代数 $\bar{A}$ 可以作用在 $M$ 上.)</font> 

**推论3.1.7.2**: 单 $A$- 模的数量等于单 $\bar{A}$- 模的数量等于半单代数 $\bar{A}$ 的单分量的数量. 

**推论3.1.8**: 代数的根是一切极大理想之交.

**命题3.1.9**: <font color=Red>代数的根是**幂零理想**且包含一切幂零左理想和右理想.</font><br/> <font color=CadetBlue>p.s. [[常用概念/单与半单#^c66248\|半单代数没有非零幂零理想]]</font>

**推论3.1.10**: 代数的根就是[[Books/有限维代数/2. Semisimple algebra 半单代数/2.2 半单模和半单代数#^de668d\|强幂零元]]集.

**拟正则(quasi-regular)理想**: 对于代数 $A$ 的理想 $I$ 中的任意元素 $x$, 满足 $(1-x)$ 可逆.

**命题3.1.11**: 代数的根是拟正则理想且包含**一切**拟正则左理想和右理想.

由命题3.1.9和命题3.1.11可知, 有限维代数中, 幂零理想$\Longleftrightarrow$拟正则理想.

**推论3.1.12**: 每个[[Books/环与模范畴/Ⅳ. 经典环结构定理/15. 环的根—局部环和Artin环#^dc826a\|诣零理想]]都是拟正则理想都是幂零理想, 因此也都在根中.

**命题3.1.13**: 若代数 $A$ 的诣零理想 $I$ 满足 $A/I$ 是半单的, 则 $I=\mathrm{rad\ }A$.

**推论3.1.14**:  $\mathrm{rad\ }(A/I)=(\mathrm{rad\ }A+I)/I$. 商代数的根等于根的商代数.

</div></div>


# [[0rigin/结合代数表示论基础\|结合代数表示论基础]]


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/books//algebras-and-modules/1/#a2deb4" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



 + **代数的根(Jacobson radical)** 是: 

</div></div>


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/books//algebras-and-modules/3/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# Ⅰ 代数与模

<font size="2">[[Books/结合代数表示论基础/Ⅰ. Algebras and modules/Ⅰ.1 代数\|Ⅰ.1 代数]] </font>
<font size="2">[[Books/结合代数表示论基础/Ⅰ. Algebras and modules/Ⅰ.2 模\|Ⅰ.2 模]] </font>
## Ⅰ.3 半单模与模的根

本节中 $K$ 是代数闭域且 $A$ 是有限维 $K$- 代数


基座socle: 右 $A$- 模 $M$ 的基座 $\operatorname{soc}M$ 是由所有 $M$ 的单子模生成的模, 是半单模, 是 $M$ 的子模.

+ **[[Books/有限维代数/2. Semisimple algebra 半单代数/2.1 舒尔引理\|舒尔引理]](Schur's lemma)**: 对于非零模同态 $f:S\longrightarrow S'$
	+ 若 $S$ 是单模, $f$ 是单射;
	+ 若  $S'$ 是单模, $f$ 是满射;
	+ 若 $S$ 和 $S'$ 都是单模, $f$ 是同构.
+ **韦德伯恩-阿廷([[Books/有限维代数/2. Semisimple algebra 半单代数/2.4 Wedderburn-Artin 定理#^6e3950\|Wedderburn-Artin]])**
+ **马施克引理(Maschke's lemma)**: $G$ 是有限群, 群代数 $KG$ 是半单的$\Longleftrightarrow$  $\left\vert G\right\vert \nmid \operatorname{char}K$

**若尔当-赫尔德定理(Jordan-Hölder theorem)**: 有限维代数的模 $M$ 的任意两个**合成序列(composition series)**  $0=M_{0}\subset M_{1}\subset M_{2} \subset \cdots \subset M_{m}=M$ 和 $0=N_{0}\subset N_{1}\subset N_{2} \subset \cdots \subset N_{n}=M$ 的长度相等, 记作 $\mathscr{l}(M)=m=n$, 且**合成因子(composition factors)** 在调整顺序后同构 $M_{j+1}/M_{j}\cong N_{\sigma(j)+1}/N_{\sigma(j)}\cong S(j)$.
+  $\ell(M)=\ell(N)+\ell(M/N)$
+  $\ell(M+N)=\ell(M)+\ell(N)-\ell(M \cap N)$

<font size="2">[[Books/结合代数表示论基础/Ⅰ. Algebras and modules/Ⅰ.4 直和分解\|Ⅰ.4 直和分解]] </font>
<font size="2">[[Books/结合代数表示论基础/Ⅰ. Algebras and modules/Ⅰ.5 投射模与内射模\|Ⅰ.5 投射模与内射模]] </font>
<font size="2">[[Books/结合代数表示论基础/Ⅰ. Algebras and modules/Ⅰ.6 基本代数与模范畴的嵌入\|Ⅰ.6 基本代数与模范畴的嵌入]] </font>

</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/books//categories-functors-and-homology/3/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# Ⅹ 范畴、函子和同调

<font size="2">[[Books/结合代数表示论基础/Ⅹ. Categories, functors, and homology/Ⅹ.1 范畴\|Ⅹ.1 范畴]]</font>
<font size="2"> [[Books/结合代数表示论基础/Ⅹ. Categories, functors, and homology/Ⅹ.2 函子\|Ⅹ.2 函子]]</font>
## Ⅹ.3 范畴的根

**范畴中双边理想**: 设 $\mathcal{C}$ 是加法 $K$- 范畴, $\mathcal{C}$ 中的态射组成的类 $\mathcal{I}$ 是 $\mathcal{C}$ 中的双边理想, 如果满足下述条件:
+ 对 $\mathcal{C}$ 中每个对象 $X$, 零态射 $0_{X}:X \rightarrow X$ 都属于 $\mathcal{I}$ .
+ 若 $X \stackrel{f}{\longrightarrow}Y$ 和 $X \stackrel{g}{\longrightarrow}Y$ 都在 $\mathcal{I}$ 中, 则对任意 $\lambda,\mu \in K$, 有 $f\lambda + g\mu \in \mathcal{I}$.
+ 若 $f \in \mathcal{I}$,  $gf \in \mathrm{Hom}_\mathcal{C}$, 则 $gf \in \mathcal{I}$.
+ 若 $f \in \mathcal{I}$,  $fh \in \mathrm{Hom}_\mathcal{C}$, 则 $fh \in \mathcal{I}$.

**范畴的根**: 设 $\mathcal{C}$ 是加法 $K$- 范畴, 则 $\mathrm{rad }_{\mathcal{C}}$ 是满足下面这个等式的双边理想:
$\mathrm{rad}_{\mathcal{C}}(X,Y)=\{ h \in \mathcal{C}(X,Y);1_{X}-g\circ h 是可逆的,对 \forall g \in \mathcal{C}(X,Y) \}.$

 $f= \begin{bmatrix}\begin{smallmatrix}f_{11} &f_{12} &\cdots &f_{1n}\\f_{21} & f_{22}&\cdots &f_{2n}\\ \vdots &\vdots &\ddots &\vdots\\f_{m1}&f_{m2}&\cdots&f_{mn}\end{smallmatrix}\end{bmatrix}:\bigoplus\limits_{i=1}^{n}X_{i}\longrightarrow\bigoplus\limits_{j=1}^{m}Y_{j}$ 属于 $\mathrm{rad}_{\mathcal{C}}(\oplus^{n}_{i=1}X_{i},\oplus^{n}_{j=1}Y_{j})$ 当且仅当  $f_{ij}:X_{i}\longrightarrow Y_{j}$ 属于 $\mathrm{rad}_{\mathcal{C}}(X_{i},Y_{j})$.

 $\mathrm{rad}_{\mathcal{C}}(Z,Z)=\mathrm{rad\ }\mathrm{End }_{\mathcal{C}}(Z)$.

若 $\mathrm{End }_{\mathcal{C}}(X)$ 和 $\mathrm{End }_{\mathcal{C}}(Y)$ 是局部代数, 则 $\mathrm{rad}_{\mathcal{C}}(X,Y)$ 就是所有从 $X$ 到 $Y$ 的所有**非同构**态射. 若 $X \ncong Y$, 则 $\mathrm{rad}_{\mathcal{C}}(X,Y)=\mathrm{Hom}_{\mathcal{C}}(X,Y)$.

 $\mathrm{rad}_{A}(X,Y)$: 所有从 $X$ 到 $Y$ 之间的**不可逆**模同态组成的线性空间.  
 $\mathrm{rad}^{2}_{A}(X,Y)$: 由  $gf$ 组成. 其中 $f\in \mathrm{rad}_{A}(X,Z)$,  $g \in \mathrm{rad}_{A}(Z,Y)$. 
.
<font size="2"> [[Books/结合代数表示论基础/Ⅹ. Categories, functors, and homology/Ⅹ.4 同调代数\|Ⅹ.4 同调代数]]</font>
<font size="2">[[Books/结合代数表示论基础/Ⅹ. Categories, functors, and homology/Ⅹ.5 扩张群\|Ⅹ.5 扩张群]]</font>

</div></div>
