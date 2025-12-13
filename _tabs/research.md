---
layout: page
icon: fas fa-flask-vial
order: 2
math: true
---

<link rel="stylesheet" href="{{ '/assets/css/publication_list_style.css' | relative_url }}">

My research is vaguely at the interface of algebraic geometry and algebraic topology. Some topics I love include: homotopy theory, enumerative algebraic geometry, 


## Preprints
{% assign preprints = site.data.publications | where_exp: "pub", "pub.status != 'published' and pub.status != 'to appear'" %}
{% include publications.html pubs=preprints %}

## Publications
{% assign pubs = site.data.publications | where_exp: "pub", "pub.status == 'published' or pub.status == 'to appear'" %}
{% include publications.html pubs=pubs %}

## Software
- [`CpMackeyFunctors.m2`](https://macaulay2.com/doc/Macaulay2/share/doc/Macaulay2/CpMackeyFunctors/html/index.html), a Macaulay2 package for doing homological algebra computations with $C_p$-Mackey functors. With D. Chan, B. Mudrak, C. Vogeli, C. Wang, M. Zeng, S. Zotine.
- [`A1BrouwerDegrees.m2`](https://macaulay2.com/doc/Macaulay2/share/doc/Macaulay2/A1BrouwerDegrees/html/index.html), a Macaulay2 package for computing local and global $\mathbb{A}^1$-Brouwer degrees, and manipulating the associated symmetric bilinear forms. With N. Borisov, F. Espino, T. Hagedorn, Z. Han, J. Lopez Garcia, J. Louwsma, G. Ong, and A. Tawfeek.



<script src="{{ '/assets/js/publications.js' | relative_url }}"></script>