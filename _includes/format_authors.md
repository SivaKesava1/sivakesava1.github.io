
{%- assign tag = include.tag | default: 'em' -%}
{%- capture highlighted_name -%}<{{ tag }} class='authors color-medium-accent'>{{ site.name }}</{{ tag }}>{%- endcapture -%}

{%- capture authors -%}
  {{ include.data | join: ',&nbsp;' }}
{%- endcapture -%}
{%- capture result -%}
  {%- include text_process.md data=authors -%}
{%- endcapture -%}
<!-- {{ authors}} -->
{{- result | replace: site.name, highlighted_name -}}