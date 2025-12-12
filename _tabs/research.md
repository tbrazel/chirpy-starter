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




## Equivariant enumerative geometry
We study how symmetry manifests in (a) counting solutions to enumerative problems and (b) *solving* for solutions in terms of parameters. This work borders equivariant algebraic topology, Hodge theory and hyperbolic geometry, and numerical algebraic geometry.

- *Equivariant algebraic geometry*, **Adv. Math.**, 2025.

## Quadratic enumerative geometry

## Fun short results

## Homotopy theory

## Number theory



<script src="{{ '/assets/js/publications.js' | relative_url }}"></script>