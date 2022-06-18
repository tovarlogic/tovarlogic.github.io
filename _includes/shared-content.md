{% if page.definitions %}
## Definiciones
	{% for def-category in page.definitions %}
### {{def-category | capitalize }}
		{% for definition in site.data._shared-content.definitions[def-category] %}
- {{ definition.key }}
: {{ definition.value }}
		{% endfor %}
	{% endfor %}
{% endif %}

{% if page.acronyms %}
	{% for acr-category in page.acronyms %}
		{% for acronym in site.data._shared-content.acronyms[acr-category] %}
*[{{ acronym.key }}]: {{ acronym.value }}
		{% endfor %}
	{% endfor %}
{% endif %}