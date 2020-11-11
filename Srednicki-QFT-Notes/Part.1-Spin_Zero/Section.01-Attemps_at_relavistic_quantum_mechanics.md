# 1. Attempts at relativistic quantum mechanics

$$
\newcommand{\pdfrac}[2]{\frac{\partial #1}{\partial #2}}
\newcommand{\dd}[2]{\text{d}^{#1}{#2}}
\newcommand{\dfrac}[2]{\frac{\dd{}{#1}}{\dd{}{#2}}}
\newcommand{\bra}[1]{\left\langle #1 \right|}
\newcommand{\ket}[1]{\left| #1 \right\rangle}
\newcommand{\braket}[2]{\left\langle #1 \middle| #2 \right\rangle}
\newcommand{\bracket}[3] {\left\langle #1 \middle| #2 \middle| #3 \right\rangle}
$$

### (1.5)

$$
\begin{aligned}
H & = \sqrt{\vec p^2 c^2 + m^2 c^4} = \sqrt{m^2 c^4 \left(1 + \frac{\vec p^2}{m c^2}\right)} = m c^2 \left(1+\frac{\vec p^2}{2 m^2 c^2}+\cdots\right) \\
& = m c^2 + \frac1{2m} \vec p^2 + \cdots
\end{aligned}
$$

### (1.23)

&emsp;&emsp;非相对论情形下, 有

$$
i \hbar \pdfrac{}{t}\braket{\psi, t}{\psi, t} = H \psi(\vec x, t) \overset{\dagger}{\Longleftrightarrow} - i \hbar \pdfrac{}{t} \psi^*(\vec x, t) = H \psi^*(\vec x, t)
$$

$$
\begin{aligned}
\therefore\ \dfrac{}{t}\braket{\psi, t}{\psi, t} & = \dfrac{}{t} \int{\dd{3}{\vec x} \braket{\psi, t}{\vec x} \braket{\vec x}{\psi, t}} \\
& = \int{\dd{3}{\vec x} \left[\psi(\vec x, t) \pdfrac{}{t} \psi^*(\vec x, t) + \psi^*(\vec x, t) \pdfrac{}{t} \psi(\vec x, t)\right]} \\
& = \frac1{i \hbar} \int{\dd{3}{\vec x} \left[-\psi(\vec x, t) H \psi^*(\vec x, t) + \psi^*(\vec x, t) H \psi(\vec x, t) \right]} \\
& = \frac1{i \hbar} \int{\dd{3}{\vec x} \left[\psi(\vec x, t) \frac{\hbar^2}{2m} \nabla^2 \psi^*(\vec x, t) - \psi^*(\vec x, t) \frac{\hbar^2}{2m} \nabla^2 \psi(\vec x, t) \right]} \\
& = \frac{i \hbar}{2m} \int{\dd{3}{\vec x}\ \nabla\cdot \left[\psi^*(\vec x, t)  \nabla \psi(\vec x, t) - \psi(\vec x, t) \nabla \psi^*(\vec x, t) \right]} \\
& = \frac{i \hbar}{2m} \oint_{S \rightarrow \infty}{\!\!\!\!\!\!\!\!\!\!\!\dd{}{\vec \sigma}\cdot \left[\psi^*(\vec x, t)  \nabla \psi(\vec x, t) - \psi(\vec x, t) \nabla \psi^*(\vec x, t) \right]} \\
& = 0
\end{aligned}
$$

其中最后一步利用了无穷远边界条件.