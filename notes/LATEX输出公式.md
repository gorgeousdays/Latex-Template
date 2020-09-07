### LATEX输出公式

***

#### 1.无编号公式

##### 1.1 行内公式

```latex
随机变量$X$的分布函数为$F(x)$，求出它的对应的密度函数$f(x)$
```

##### 1.2 行间公式

```latex
我们熟知的勾股定理是：$$a^2 + b^2 = c^2$$
```

#### 2.有编号公式

##### 2.1 手动编号

```latex
$$a^2 + b^2 = c^2 \tag{1.1}$$
$$a^2 + b^2 = c^2 \tag{no.1}$$
```

##### 2.2自动编号

```latex
\begin{equation}
    a^2 + b^2 = c^2
\end{equation}
```

##### 2.3 等式对齐

```latex
%  使用align参数
\begin{align}
    x +  y = 1\\\\
    2x + y \neq 1\\\\
    3x +4y \leq 2\\\\
    4x \geq y
\end{align}
```

##### 2.4 分开输入

```latex
\begin{equation}
    \begin{split}  %  使用split参数 当公式太长 可以分段输出
        (x + y)(x + 4y) & = x^2 + 4xy + xy + 4y^2\\\\
                & = x^2 +5xy + 4y^2
    \end{split}
\end{equation}
```

##### 2.5 分类输入

```latex
\begin{equation}
    a_{i1}A_{j1} + a_{i2}A_{j2} + \cdots + a_{in}A_{jn} = 
    \begin{cases}  %  cases参数可用于输出分段函数，即大括号公式
        \begin{vmatrix}A\end{vmatrix}，& i =j\\\\
        0, & i \neq j
    \end{cases}
\end{equation}
%  使用cases参数时只会对括号公式进行一次编号，但如果每个情况的公式都要有编号，可以使用numcases参数，但是要在专门的latex套件中调用cases宏包
```

##### 2.6 矩阵的输入

```latex
%  无外边框
\begin{array}{ccc}
    1 & 0 & 0\\\\
    0 & 1 & 0\\\\
    0 & 0 & 1\\\\
\end{array}  
%  有外边框[ ]
$$
\left[
    \begin{array}{ccc}
        1 & 0 & 0\\\\
        0 & 1 & 0\\\\
        0 & 0 & 1\\\\
    \end{array}
\right]
$$ 
%  简化写法
%  带()的矩阵
\begin{pmatrix}
    1 & 0 & 0\\\\
    0 & 1 & 0\\\\
    0 & 0 & 1\\\\
\end{pmatrix}

%  带[]的矩阵
\begin{bmatrix}
    1 & 0 & 0\\\\
    0 & 1 & 0\\\\
    0 & 0 & 1\\\\
\end{bmatrix}

%  带||,即行列式
\begin{vmatrix}
    1 & 0 & 0\\\\
    0 & 1 & 0\\\\
    0 & 0 & 1\\\\
\end{vmatrix}
```

##### 2.7公式内换行

```latex
\begin{equation}
\begin{split} %通过split标签实现公式内换行  
&\mbox{目标函数:}Q=x+y\\  %通过&实现对齐，两处&处将自动对齐
s.t.&\begin{cases
373x\le3000\\
201y\le1500\\
74973xy\le4500000\\
\end{cases}
\end{split}
\end{equation}
```