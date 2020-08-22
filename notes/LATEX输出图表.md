### LATEX输出图表

***

#### 1.输出图片

```latex
%单张图片的输出

\begin{figure}[H]  %  H代图片就在当前位置 在某些情况下由于一页已经排不下，图片会自动调到其他地方，加上该参数可以避免
\centering  %  表示图片居中
\includegraphics[width=5in]{1.png}  % 图片宽度 可以用height参数控制高度  1.png表示图片位置，将图片至于figures文件夹下
\caption{问题二流程图}  %图片名称
\end{figure}

%多张图片的输出(两张图片并排)
\begin{figure}[H]
    \begin{minipage}[t]{0.5\linewidth}
        \centering
        \includegraphics[width=3in]{4.png}
        \label{fig:side:a} %控制图片位置
         % \caption{fig2}为两张图分别加标题图片
    \end{minipage}%
    \begin{minipage}[t]{0.5\linewidth}
        \centering
        \includegraphics[width=3in]{5.png}
        \label{fig:side:b}
        % \caption{fig2}为两张图分别加标题图片
    \end{minipage}%
    \caption{$\theta$角与$A_i$角关系示意图} %两张图片共享一个题目
\end{figure}

```

#### 2.输出表格

```latex
% array用法  \hline表示水平线，而竖线可以使用|来表示

\begin{array}{|c|c|} %表示表格的宽度为2个字符
        \hline 
        0 & 1 \\\\\hline
        1 & 0 \\\\\hline
\end{array}

% \quad和\hspace{}都是表示空格，但是空的个数不同

\begin{array}{cc}
        (A)\quad 4 & \hspace{4cm}(B)\quad 3\\\\
        (B)\quad 2 & \hspace{4cm}(D)\quad 1
\end{array}

%table用法

\begin{table}[htbp]
	\centering  % 显示位置为中间
	\caption{standard table}  % 表格标题
	\label{table1}  % 用于索引表格的标签
	%字母的个数对应列数，|代表分割线
	% l代表左对齐，c代表居中，r代表右对齐
	\begin{tabular}{cccc}  
		\hline  % 表格的横线
		& & & \\[-6pt]  %可以避免文字偏上 调整文字与上边界的距离
		1&2&3&4 \\  % 表格中的内容，用&分开，\\表示下一行
		\hline
		& & & \\[-6pt]  %可以避免文字偏上 
		0.1&0.2&0.3&0.4 \\
		\hline
	\end{tabular}
\end{table}


%输出三线表格
\begin{table}[!htbp]
  \caption[标签名]{中文标题}
  \begin{tabular}{cc...c}
    \toprule[1.5pt]
    表头第1个格 & 表头第2个格 & ... & 表头第n个格 \\
    \midrule[1pt]
    表中数据(1,1) & 表中数据(1,2) & ... & 表中数据(1,n)\\
    表中数据(2,1) & 表中数据(2,2) & ... & 表中数据(2,n)\\
    ...................................................\\
    表中数据(m,1) & 表中数据(m,2) & ... & 表中数据(m,n)\\
    \bottomrule[1.5pt]
  \end{tabular}
\end{table}
```

