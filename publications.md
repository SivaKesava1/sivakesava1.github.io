---
layout: default
title: Publications
---
<main id="main" class="site-main">    
    <h1 class="title-small-caps"> <i class="fa fa-fw fa-copy"></i>{{ page.title }}</h1>
    {% assign xprojects = site.projects  | sort: 'sorter' | reverse%}
    {% for project in xprojects %}
    {% if project.sorter == 1 -%}
     <hr>
    {% endif %}
        <div class='paper-table flex-container'>
            <div  class='paper-left'>
                <span style='letter-spacing: 0.025em;' class='target'>
                {%- capture target -%}
                    {{- project.target.short }} =qq= {{ project.year | slice: 2,2 -}}
                {%- endcapture -%}
                {%- include text_process.md data=target -%}
                </span><br>
                <div class='icons'>(
                {%- if project.to_appear -%}
                <em style='letter-spacing: 0.25px;'>... To Appear ...</em>
                {%- elsif project.DOI or project.links.PDF or project.links.Slides %}
                    <a href='{{ project.url }}#bibtex-citation'><i class='fas fa-fw fa-sm fa-quote-left'></i></a>
                    {% if project.links.PDF -%}
                    <a href='{% include text_process.md data=project.links.PDF %}'><i class='far fa-sm fa-file-pdf'></i></a>
                    {%- endif %}
                    {% if project.links.Slides -%}
                    <a href='{% include text_process.md data=project.links.Slides %}'><i class='fas fa-sm fa-fw fa-desktop'></i></a>
                    {%- endif %}
                {% endif %})</div>
            </div>
            <div class='paper-right'>
                <div>
                <a class='title highlighted' href='{{ project.url }}'>{% include text_process.md data=project.title %}</a><br>
                <div class='authors'>{% include format_authors.md data=project.authors %}</div>
                 {%- if project.awards %}
                    <div class='awards color-accent'>
                    {%- for award in project.awards -%}
                        &loang;&hairsp;<i class='fas fa-fw fa-sm fa-{{ award.icon }}'></i>&nbsp; {% include text_process.md data=award.desc %}&hairsp;&roang; &nbsp;
                    {%- endfor -%}
                    </div>
                {% endif -%}
                </div>
            </div>
        </div>
    {% endfor %}
</main><!-- .site-main -->