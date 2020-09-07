### LATEX实现表格内单元格换行

***



```latex
\documentclass{article}
\usepackage{makecell}
\begin{document}
\section{One}
\begin{center}
\begin{tabular}{|c|>{\makecell*[c]}c|}
  \hline
  \makecell[tl]{Left aligned \\ cell text} & 1--2 \\
  \hline
  \makecell*[r]{Right Aligned \\ cell text} & 3--4 \\
  \hline
  \makecell[{}{p{3cm}}]{This is a \\ vertical alignment} & 5--6 \\
  \hline
  \makecell[c{>{\parindent 2em}p{3cm}}]{V \&{} H alignments} & 7--8 \\
  \hline
\end{tabular}
\end{center}
\end{document}
%推荐参数 makecell[c]{xxx\\xxx}&xxx \\ \hline   实现居中以及换行操作
```

