---
title: Config Hexo
date: 2021-03-14 15:26:40
categories: Tech
tags:
  - Static Site
  - Hexo
  - MathJax
---

<script>
MathJax = {
  tex: {
    inlineMath: [['$', '$'], ['\\(', '\\)']]
  },
  svg: {
    fontCache: 'global'
  }
};
</script>
<script type="text/javascript" id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-svg.js">
</script>

## Alternative Themes

[`theme: next`](https://github.com/next-theme/hexo-theme-next)

[`theme: Wikitten`](https://github.com/zthxxx/hexo-theme-Wikitten)

Pay attention: `theme: Name` in `_config.yml` must be identical to `themes/Name`

## MathJax / KaTeX

[Config MathJax using in-line script](https://docs.mathjax.org/en/latest/web/configuration.html#configuration-using-an-in-line-script)

```
<script>
MathJax = {
  tex: {
    inlineMath: [['$', '$'], ['\\(', '\\)']]
  },
  svg: {
    fontCache: 'global'
  }
};
</script>
<script type="text/javascript" id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-svg.js">
</script>
```

Test $\TeX$

$$
i\hbar\frac{\partial}{\partial t}\psi=-\frac{\hbar^2}{2m}\nabla^2\psi+V\psi
$$

## Search (Local)

TODO
