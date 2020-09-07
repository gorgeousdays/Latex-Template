### LATEX的一些小功能

***

#### 1.无序列表与有序列表

##### 1.1 无序列表

```latex
\begin{itemize}
  \item one
  \item two
  \item ...
\end{itemize}
```

##### 1.2 有序列表

```latex
% \begin{enumerate}[i)] 通过添加参数可以控制有序列表的序列 
\begin{enumerate}
  \item one
  \item two
  \item ...
\end{enumerate}
%或者用
\begin{description}
  \item[item a] one
  \item[item b] two
  \item[item c] ...
\end{description}
```

#### 2.杂项

```latex
\textbf{加粗} 

\textit{斜体 Italics}

生成脚注\footnote{脚注可以补充说明一些东西}

\newpage  %  强制分页

\par  %  分段 或用两个回车 

\newline  %  换行 或者用 \\

\mbox{在数学环境下中输入中文}  %实现在公式中输入中文
```

#### 3.定理、证明等环境

```latex
\begin{theorem}
  这是一个定理。
  \label{thm:example}
\end{theorem}
由\cref{thm:example}我们知道了定理环境的使用。


\begin{lemma}
  这是一个引理。
  \label{lem:example}
\end{lemma}
由\cref{lem:example}我们知道了引理环境的使用。


\begin{corollary}
  这是一个推论。
  \label{cor:example}
\end{corollary}
由\cref{cor:example}我们知道了推论环境的使用。


\begin{assumption}
  这是一个假设。
  \label{asu:example}
\end{assumption}
由\cref{asu:example}我们知道了假设环境的使用。


\begin{conjecture}
  这是一个猜想。
  \label{con:example}
\end{conjecture}
由\cref{con:example}我们知道了猜想环境的使用。


\begin{axiom}
  这是一个公理。
  \label{axi:example}
\end{axiom}
由\cref{axi:example}我们知道了公理环境的使用。


\begin{principle}
  这是一个定律。
  \label{pri:example}
\end{principle}
由\cref{pri:example}我们知道了定律环境的使用。


\begin{problem}
  这是一个问题。
  \label{pro:example}
\end{problem}
由\cref{pro:example}我们知道了问题环境的使用。


\begin{example}
  这是一个例子。
  \label{exa:example}
\end{example}
由\cref{exa:example}我们知道了例子环境的使用。


\begin{proof}
  这是一个证明。
  \label{prf:example}
\end{proof}
由\cref{prf:example}我们知道了证明环境的使用。


\begin{solution}
  这是一个解。
  \label{sol:example}
\end{solution}
由\cref{sol:example}我们知道了解环境的使用。
```

