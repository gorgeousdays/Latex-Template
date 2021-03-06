### LATEX基础

***

#### 1.LATEX相关文件扩展名与描述

| 扩展名 | 描述                                                         |
| ------ | :----------------------------------------------------------- |
| `.tex` | TeX 源文档                                                   |
| `.sty` | LaTeX 样式文件，使用 `\usepackage` 命令导入                  |
| `.dtx` | Documented TeX。LaTeX `sty` 文档的分发形式                   |
| `.ins` | `.dtx` 的安装文件，`latex foo.ins` 会生成所需的 sty 文档和帮助手册 |
| `.cls` | 类文档，使用 `\documentclass` 命令导入                       |
| `.fd`  | 字体描述文档                                                 |
| `.dvi` | 设备无关文件 `latex` 编译产生                                |
| `.pdf` | pdf 文档                                                     |
| `.log` | 编译日志                                                     |
| `.toc` | 存放章节名称，在下一次编译时读入以产生目录                   |
| `.lof` | 类似于 `.toc` 产生插图目录                                   |
| `.lot` | 产生表格目录                                                 |
| `.aux` | 存放各种标签引用信息，下次编译时读入以产生交叉参考           |
| `.idx` | 存放索引词，用 `makeindex` 处理                              |
| `.ind` | 处理过的 `.idx `文档，下次编译时读入以产生索引               |
| `.ilg` | `makeindex` 的日志                                           |