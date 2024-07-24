---
layout: post
title: "Convergence to the mean value"
author: 
GG: 
link: 
categories: [content]
---

Some basic properties of almost periodic functions.
<!--more-->


<!-- {: .message } -->
<p class="message">

Let $f\in \mathrm{AP}(\mathbb{R})$, $\varepsilon>0$ and $l_\varepsilon(f)$ be the length of the inclusion interval. 
Then $\sup_{\mathbb{R}} |f| \leq \sup_{[0,l_\varepsilon]}  |f| + \varepsilon$ and furthermore, for $T>0$ we have 

$$
\begin{equation}\label{eq:thm::ap:uap-ergodic-estimate-eps-l-eps-rate}
    \left|\frac{1}{T}\int_0^T f(x)\;dx - M(f)\right|   \leq  \varepsilon + 2\left(\sup_{x\in \mathbb{R}} |f(x)|\right) \frac{ l_\varepsilon(f)}{T}.
\end{equation}
$$

</p>

--- 




Let $n\in \mathbb{N}$, we write 

$$
\begin{equation}\label{2}
     \frac{1}{nT}\int_0^{nT} f(x)\;dx 
     = \sum_{k=0}^{k=n-1} \frac{1}{nT} \int_{kT}^{(k+1)T} f(x)\;dx \tag{2}
\end{equation}
$$

Let $l_\varepsilon$ be the length of the inclusion interval of $E(\varepsilon,f)$ and $\tau_k \in E(\varepsilon,f)\cap [kT,kT+l_\varepsilon]$ be a $\varepsilon$-period. Since $kT \leq \tau_k \leq kT + l_\varepsilon$, we have

$$
\begin{align*}
     \int_{kT}^{(k+1)T} f(x)\;dx &= \int_{kT -\tau_k}^{(k+1)T - \tau_k} f(x+\tau_k)\;dx\\
     &\qquad = \int_0^T f(x)\;dx + \int_0^T \Big(f(x+\tau_k) - f(x)\Big)\;dx  \\
     &\qquad + \int_{kT- \tau_k}^0 f(x+\tau_k)\;dx + \int_{T}^{(k+1)T - \tau_k} f(x+\tau_k)\;dx.
\end{align*}
$$

 In other words, we have

$$
\begin{align*}
     &\int_{kT}^{(k+1)T} f(x)\;dx - \int_{0}^{T} f(x)\;dx 
     = \int_0^T \Big(f(x+\tau_k) - f(x)\Big)\;dx  \nonumber \\
     &\qquad\qquad\qquad + \int_{kT- \tau_k}^0 f(x+\tau_k)\;dx -\int_{(k+1)T - \tau_k}^T f(x+\tau_k)\;dx.
\end{align*}
$$

Therefore

$$
\begin{equation}\label{3}
     \left|\int_{kT}^{(k+1)T} f(x)\;dx - \int_0^T f(x)\;dx\right| \leq \varepsilon T + 2 \Vert f\Vert _{L^\infty(\mathbb{R})}l_\varepsilon.
     \tag{3}
\end{equation}
$$

 From $\eqref{2}$ and $\eqref{3}$ we have

$$
\begin{equation}\label{4}
     \left|\frac{1}{nT}\int_{0}^{nT} f(x)\;dx - \frac{1}{T}\int_0^T f(x)\;dx\right| \leq \varepsilon + 2 \Vert f\Vert _{L^\infty(\mathbb{R})}\frac{l_\varepsilon}{T}. \tag{4}
\end{equation}
$$

Let $n\to \infty$ in $\eqref{4}$ we obtain the conclusion, since 

$$\lim_{n\to \infty}\frac{1}{nT}\int_{0}^{nT} f(x)\;dx = M(f)$$ 

exists by assumption $f\in \mathrm{AP}(\mathbb{R})$.


We will revisit this in the future.