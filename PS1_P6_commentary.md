---
title: Some commentary on Problem 6 in Problem Set 1
subtitle: Optional Material
header-includes: |
	\usepackage{amsmath}
	\usepackage{mathtools}
	\DeclarePairedDelimiter\floor{\lfloor}{\rfloor}
---

Before we show why the technique you used earlier works, let us introduce first the *floor function*. The floor function ($\floor*{x}$) simply *rounds down* a number, in other words, it give the lowest integers greater than the integer given to it. For example $\floor*{3.5} = 3$ and $\floor*{-4.1} = -4$.

Let us define numbers $p_1$, $p_2$, and $n$, which are all integers. We can express $p_1$ and $p_2$ as the following:
\begin{gather}
p_1 = nk + a \\
p_2 = nl + b
\end{gather}
Where $k$ and $l$ are integers, and $a$ and $b$ are nonnegative integers less than $n$. Basically, we can express them as n times something plus the remainder from dividing it by n. For example, 62 can be expressed as $3 \times 20 + 2$ and -161 can be expressed as $3 \times -54 + 1$. Note that the remainder will never exceed 3, otherwise, $k$ or $l$ will be added with the remainder divided by 3.

What we are trying to show now is:
\begin{equation}
\floor*{\frac{p_1}{n}} - \floor*{\frac{p_2}{n}} = \floor*{\frac{p_1 - p_2}{n}}
\end{equation}

Substitute equations 1 and 2 into equation 3:
\begin{equation}
\floor*{\frac{nk + a}{n}} - \floor*{\frac{nl + a}{n}} = \floor*{\frac{nk - nl + a - b}{n}}
\end{equation}

Let us simplify first the left hand side of the equation
\begin{equation*}
\floor*{\frac{nk + a}{n}} - \floor*{\frac{nl + b}{n}} = \floor*{k + \frac{a}{n}} - \floor*{l + \frac{b}{n}}
\end{equation*}

Since $a$ and $b$ are less than n, $\frac{a}{n}$ and $\frac{b}{n}$ are fractional, therefore they are 0 in the floor function. This leaves us with
\begin{equation*} k - l \end{equation*}
for the left side.

Now we work on the right side of the equation:
\begin{equation*}
\floor*{\frac{nk - nl + a - b}{n}} = \floor*{k - l + \frac{a - b}{n}}
\end{equation*}
To show that the left and right sides are equal, we must show that $\frac{a - b}{n}$ is fractional, in other words, show that $\lvert a - b \rvert$ is less than $n$. The maximum value of $a$ or $b$ is $n - 1$ and the minimum the value is 0. Therefore $1 - n \leq a - b \leq n - 1$, the absolute value of $a-b$ is less than n. Therefore we have
\begin{equation*}
\floor*{k - l + \frac{a - b}{n}} = \floor*{k - l} = k - l
\end{equation*}

Therefore,
\begin{equation*}\floor*{\frac{p_1}{n}} - \floor*{\frac{p_2}{n}} = \floor*{\frac{p_1 - p_2}{n}}\end{equation*}