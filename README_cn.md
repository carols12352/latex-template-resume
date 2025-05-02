# LaTeX 简历模板

这是一个简洁优雅的 LaTeX 简历模板，仅使用标准的 LaTeX 宏包，无需额外文件或复杂结构。

你可以直接在 Overleaf 或任何 LaTeX 编辑器（如 TeXShop、TeXworks）中编译本文件。

---

## 基本结构

简历包含以下部分：

* 个人信息（姓名和联系方式）
* 教育背景
* 技能
* 工作或实习经历
* 项目经历
* 领导力与课外活动

---

## 使用方法

### 1. 修改姓名与联系方式

在 LaTeX 源文件中找到以下内容：

```latex
\name{Riley Johnson}
\contact{rileyjohnson@yahoo.com}{+1-384-623-6034}{rileyjohnson}{https://www.linkedin.com/in/rileyjohnson/}
```

将其替换为你的姓名、电子邮箱、联系电话、GitHub 用户名和 LinkedIn 链接。

---

### 2. 修改各模块内容

按照既有结构填写即可。例如：

```latex
\section*{Education}
\textbf{University Name}, City \\
Degree (Year--Year) \\
Relevant Courses: ...
```

其他部分（如工作经历、项目等）与此类似。

---

## 自定义指南

### 1. 修改字体大小

编辑文档开头的这行代码：

```latex
\documentclass[10pt,a4paper]{article}
```

将 `10pt` 改为 `11pt` 或 `12pt` 即可调整整体字体大小。

---

### 2. 修改行距

调整这行代码的数值：

```latex
\setstretch{0.92}
```

建议改为 `1.0` 或 `1.1`，让排版更松一些。

---

### 3. 控制段落间距

修改如下命令的参数：

```latex
\titlespacing\section{0pt}{6pt plus 2pt minus 1pt}{4pt plus 1pt minus 1pt}
```

参数含义依次为：左边距、段前间距、段后间距。数值越大，间距越宽。

---

### 4. 添加项目符号或子项内容

使用 `itemize` 环境，例如：

```latex
\begin{itemize}[leftmargin=1.5em, itemsep=0pt]
    \item 熟练使用 Python 进行数据分析
    \item 熟悉 Git 和版本控制
\end{itemize}
```

你可以修改 `leftmargin` 调整缩进，修改 `itemsep` 控制条目间距。

---

## 图标说明（fontawesome）

模板使用 `fontawesome` 宏包提供以下图标命令：

* 邮箱：`\faEnvelope`
* 电话：`\faPhone`
* GitHub：`\faGithub`
* LinkedIn：`\faLinkedinSquare`

如果不使用这些链接图标，可将 `\contact{}` 命令块删除或简化。

---

## 编写建议

* 可复制 `\section*{}` 块增加更多内容模块，例如证书、获奖、出版物等。
* 用 `\textit{}` 命令将技术名词或工具名变为斜体。
* 使用 `\smallgap` 命令压缩条目间垂直间距。
* 如何使用 `\smallgap`

  ```latex
  \section*{Projects}
  \smallgap
  \textbf{Hello world!} - hahahaha
  ```

---

## 环境要求

* 所需 LaTeX 宏包：`fontawesome`、`titlesec`、`enumitem`、`parskip`、`setspace`
* 推荐编译方式：使用 `pdflatex`，或在 Overleaf 在线编译

---

## 协议声明

本模板采用 GNU GPL3 开源协议。你可以自由使用、修改和分发。
