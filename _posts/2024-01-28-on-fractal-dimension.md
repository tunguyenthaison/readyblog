---
layout: post
title: On fractal dimension of almost periodic attractor
date: 2024-01-28 04:48:00-0400
description: some notes on this subject
tags: formatting math
categories: sample-posts
related_posts: true
---

In this post, I go through some of the interesting results by Naito 
{% cite naito_fractal_1996 %}. More precisely, I want to look into this result:

{% quote naito_fractal_1996 %}

Theorem 1. Let $f(t):\mathbb{R}\to X$ be an almost periodic function, which satisfies a Hölder condition: there exists a constant $\delta: 0< \delta\leq 1$ such that

$$
    \sup_{t,s\in \mathbb{R}, t\neq s} \frac{|f(t)-f(s)|}{|t-s|} = c_0 < \infty. 
$$

{% endquote %}

The reason for this is as follows.  {% cite einstein1950meaning %}, 
A later paper claimed one of the result is indeed having a gap, while proposing
some fix. Going through it carefully maybe a good way to avoid any future mistales.
Whether or not this is a good use of time is up to debate, another version of myself
in the next couple of days may regret this.


This theme supports rendering beautiful math in inline and display modes using [MathJax 3](https://www.mathjax.org/) engine. You just need to surround your math expression with `$$`, like `$$ E = mc^2 $$`. If you leave it inside a paragraph, it will produce an inline expression, just like $$ E = mc^2 $$.

To use display mode, again surround your expression with `$$` and place it as a separate paragraph. Here is an example:

$$
\sum_{k=1}^\infty |\langle x, e_k \rangle|^2 \leq \|x\|^2
$$

You can also use `\begin{equation}...\end{equation}` instead of `$$` for display mode math.
MathJax will automatically number equations:

\begin{equation}
\label{eq:cauchy-schwarz}
\left( \sum*{k=1}^n a_k b_k \right)^2 \leq \left( \sum*{k=1}^n a*k^2 \right) \left( \sum*{k=1}^n b_k^2 \right)
\end{equation}

and by adding `\label{...}` inside the equation environment, we can now refer to the equation using `\eqref`.

Note that MathJax 3 is [a major re-write of MathJax](https://docs.mathjax.org/en/latest/upgrading/whats-new-3.0.html) that brought a significant improvement to the loading and rendering speed, which is now [on par with KaTeX](http://www.intmath.com/cg5/katex-mathjax-comparison.php).
