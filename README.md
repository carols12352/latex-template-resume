(English|[简体中文](./README_cn.md)）
# LaTeX Resume

This is a simple, elegant one-file LaTeX resume template that requires no external files or packages beyond standard ones.

You can compile this file directly using Overleaf or any LaTeX editor (e.g., TeXShop, TeXworks).


## Basic Structure

The resume is structured as follows:

- **Header** – Name and contact info
- **Education**
- **Skills**
- **Experience**
- **Projects**
- **Leadership**


## How to Use

1. **Change Your Name and Contact Info**

In the LaTeX source, look for:

```latex
\name{Riley Johnson}
\contact{rileyjohnson@yahoo.com}{+1-384-623-6034}{rileyjohnson}{https://www.linkedin.com/in/rileyjohnson/}
```

Replace with your name, email, phone number, GitHub username, and LinkedIn link.


2. **Update Each Section**

Just follow the structure and replace the placeholders:

```latex
\section*{Education}
\textbf{University Name}, City \\
Degree (Year--Year) \\
Relevant Courses: ...
```

Use similar patterns for experience, projects, and leadership.


## Customization Guide

### 1. Change Font Size or Style

* Modify this line in `\documentclass`:

```latex
\documentclass[10pt,a4paper]{article}
```

* Change `10pt` to `11pt` or `12pt` for larger font.

### 2. Adjust Line Spacing

* Edit this value:

```latex
\setstretch{0.92}
```

* Try values like `1.0`, `1.1` for more breathing room.

### 3. Add More Space Between Sections

* Increase spacing in this block:

```latex
\titlespacing\section{0pt}{6pt plus 2pt minus 1pt}{4pt plus 1pt minus 1pt}
```

* Format: `\titlespacing{<command>}{<left>}{<before>}{<after>}`

### 4. Add Bullet Points or Sub-items

Use the `itemize` environment for skill lists or task lists:

```latex
\begin{itemize}[leftmargin=1.5em, itemsep=0pt]
    \item ...
    \item ...
\end{itemize}
```

You can change `leftmargin` or `itemsep` to adjust layout.


## FontAwesome Icons

This template uses the `fontawesome` package for:

* Email: `\faEnvelope`
* Phone: `\faPhone`
* GitHub: `\faGithub`
* LinkedIn: `\faLinkedinSquare`

If you're not using these links, you can remove that whole block.


## Tips

* You can copy-paste the `\section*{}` blocks to add more custom sections (e.g., Certifications, Awards).
* Use `\textit{}` to italicize technologies or secondary info.
* Use `\smallgap` to reduce space between elements in the same section.


## Requirements

* LaTeX packages: `fontawesome`, `titlesec`, `enumitem`, `parskip`, `setspace`
* Recommended compiler: `pdflatex`, or use [Overleaf](https://www.overleaf.com/)


## License

GNU GPL3 License – Free to use, modify, and distribute.
