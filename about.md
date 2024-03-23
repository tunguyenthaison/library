---
layout: page
title: About
permalink: /about
---

## Commonly used links: 

- [Hackerrank](https://www.hackerrank.com/domains/algorithms)


## How to use `katex` with references

- How to use `\label{}` and `\eqref{}` with `katex`?
  * `https://github.com/falgon/roki-web/issues/34`
  * `https://github.com/KaTeX/KaTeX/issues/2003`
 
- Example code with `label` and `tag`

{% highlight tex %}
$$
    \begin{aligned} 
        \sin 2\theta = 2\sin \theta \cos \theta = \cfrac{2 \tan \theta}{1+\tan^2 \theta} . 
    \end{aligned} \label{1-1}\tag{1-1}
    Search by definition $\eqref{1-1}$ or $\ref{1-1}$.
$$


{% endhighlight %}

- Rendered version:

$$
\begin{aligned} 
    \sin 2\theta = 2\sin \theta \cos \theta = \cfrac{2 \tan \theta}{1+\tan^2 \theta} .
\end{aligned} \label{1-1}\tag{1-1}
$$

Search by definition $\eqref{1-1}$ or $\ref{1-1}$.

## Macros
- Type `\R` to obtain $\R$. 
- Configure in  `_layouts/default.html`. 



