To automatically generate a proceeding of conference papers in Overleaf, you can use the "combine" package. Here are the general steps:
- Create a new Overleaf project and add a main.tex file.
- In the main.tex file, include the "combine" package with the command: \usepackage{combine}.
- Create a subfolder for each paper that you want to include in the proceeding. For example, you can create a folder for paper1 and another folder for paper2.
- In each subfolder, create a new .tex file for the corresponding paper. For example, you can create paper1.tex in the paper1 folder and paper2.tex in the paper2 folder.
- In the main.tex file, use the command \begin{papers} to indicate the beginning of the paper list.
- For each paper, use the command \collected{filename} to include the paper in the proceeding. For example, if you have a paper1.tex file in the paper1 folder, you can use the command \collected{paper1/paper1} to include the paper.
- Use the command \end{papers} to indicate the end of the paper list
Here is an example code for the main.tex file:


\documentclass{article}

\usepackage{combine}

\begin{document}

\title{Proceeding of Conference Papers}

\author{Your Name}

\maketitle

\begin{papers}

\collected{paper1/paper1}
\collected{paper2/paper2}

\end{papers}

\end{document}
