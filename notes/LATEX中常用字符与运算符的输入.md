### LATEX中常用字符与运算符的输入

***

#### 1.保留字符

```latex
% # $ % ^ & _ { } ~ \
% 对于上述保留字符 采用转义字符“\”来实现输出 
```

***

#### 2.希腊字母

| 希腊字母小写、大写 | LaTeX形式       | 希腊字母小写、大写 | LaTeX形式         |
| ------------------ | --------------- | ------------------ | ----------------- |
| α   ***A***        | \alpha A        | μ  ***N***         | \mu N             |
| β  ***B***         | \beta B         | ξ  Ξ               | \xi \Xi           |
| γ  Γ               | \gamma \Gamma   | **o** ***O***      | o O               |
| δ  Δ               | \delta \ Delta  | π  Π               | \pi  \Pi          |
| ϵ  ε  ***E***      | \epsilon E      | ρ  ϱ  ***P***      | \rho P            |
| ζ  ***Z***         | \zeta Z         | σ  Σ               | \sigma \Sigma     |
| η  ***H***         | \eta H          | τ  ***T***         | \tau T            |
| θ  ϑ  Θ            | \theta \Theta   | υ  Υ               | \upsilon \Upsilon |
| ι  ***I***         | \iota I         | ϕ  φ  Φ            | \phi \Phi         |
| κ  ***K***         | \kappa K        | χ   ***X***        | \chi X            |
| λ  Λ               | \lambda \Lambda | ψ  Ψ               | \psi \Psi         |
| μ  ***M***         | \mu M           | ω  Ω               | \omega  \Omega    |

#### 3.集合相关

```latex
\mathbb{R} %特殊集合符号R 还有\mathbb{z}和\mathbb{N}

\subset  %真包含⊂  \supset表示反方向⊃

\subseteq  %包含 ⊆

\in  %属于∈  %\notin表示不属于

\cap  %交集  ∩

\cup  %并集  ∪

\mid  % |

\neg  %集合中非  ¬
```

#### 4.二元运算符

```  latex
\ge %  ≥

\le %  ≤

\equiv %  ≡

\approx  %  ≈

\cdot  %  ⋅

\pm  %  ±

\div  %  ÷

\frac{}{} %分数运算
```

#### 5.大尺寸运算符

```latex
%\sum求和符合  \prod求积符号
\begin{equation}
    p = \sum_{n=1}^Na_n 
\end{equation}

%\int表示积分符号
$ \int_{1}^{\infty} $ %\infty表示无穷
$ \int_{E} fdx $

%\lim表示极限符号
$ \lim_{n\to 0} $
$ \lim\limits_{n\to \infty}\int_{E}f_n dx \geq \int_{E}gdx $
```

#### 6.其它符号

```latex
%箭头符号
\leftarrow  %  往左箭头 或者用\gets
\rightarrow  %  往右箭头 或者用\to
\longleftarrow  %  往右加长箭头

%下列点的输出可用于矩阵
\dots  %  三点横向排列 或者用\cdots
\vdots  %  三点竖向排列
\ddtos  %  三点斜向排列

%下列符号用于证明
\forall  %	任意∀
\exists  %	存在∃

%导数相关
\partial x  %  偏导符号
\mathrm{d} x  %  求导符号
x^{’}  %  撇形式的求导符号
\dot x  %  点形式的求导符号 \ddot表示2个点 \dddot表示三个点 几个d就是几个点
\nabla f  %  全微分算子
```

