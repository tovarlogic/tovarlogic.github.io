---
title: "Notas breves"
breadcrumb_name: Notas
type: note
permalink: /notas/
excerpt: "Sección donde recojo brevemente pensamientos que quiero recordar para más adelante desarrollarlos en un artículo."
last_modified_at: 2021-05-13
---

Mediante este `Libro de Notas` pretendo ir recogiendo todos los pensamientos que merecen ser recordados para más adelante reflexionar sobre ellos y desarrollar ideas. 

## Libro de notas

| Sección 							| Descripción 														|
| - 								| - 																|
| [Diario](diario/) 				| Cajón desastre. Notas diarias que tendré que ampliar y organizar. |
| [sobre lo público](publico/) 		| Sección sobre ideas de política y gestión de lo público. 			|
| [sobre economía](publico/) 		| Sección sobre ideas y nociones económicas. 						|

| Apartado                              | Descripción                                              |
| ------------------------------------- | -------------------------------------------------------- |
| [Riesgos para la humanidad](riesgos/) | Apartado centrado en los probables riesgos que no vemos. |
| [Sociedad zombie](sociedad-zombie/)   |                                                          |
| [Nociones económicas](economia/)      |                                                          |
| [Sobre lo política](publico/#política)      |                                                          |

<ul>
  {% assign items = site.docs | where "doc_type", page.type %}
  {% assign items_sorted = items | sort: 'last_modified_at' %}
  {% for item in items_sorted %}
    <li>
      <h2><a href="{{ doc.url }}">
      		{{ item.last_modified_at }} - {{ item.title }}
      	  </a>
      </h2>
    </li>
  {% endfor %}
</ul>