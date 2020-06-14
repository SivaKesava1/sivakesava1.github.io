
<h3 class="updates-small-caps"><i style="font-size:0.9em;" class="fa fa-fw fa-user-clock"></i> Updates</h3>

<div class='events'>
{%- assign sorted_updates = site.updates | sort: 'date' | reverse -%}
{%- for event in sorted_updates -%}
    {%- assign event_photo = site.baseurl | append: '/assets/images/' | append: event.photo -%}
    {%- assign highlight = event.highlight | default: site.default_highlight[event.type] -%}
    <div class='pure-g event type-{{- event.type -}}'>
        <div class='pure-u-1-8 pure-u-sm-1-12 event-date'>
            {%- if event.end_date != null -%}
                {{- event.end_date | date: "%b" -}}<i>{{event.end_date | date: "%y"}}</i><br><b>&vellip;</b><br>
            {%- endif -%}
            {{- event.date | date: "%b" -}}<i>{{- event.date | date: "%y" -}}</i>
        </div>
        <div class='pure-u-1-12 event-icon color-faded {% if highlight -%} color-{{- highlight -}} {%- endif %}'>
          <i class='fas fa-fw fa-{{ event.icon | default: site.default_icon[event.type] }}'></i>
        </div>
        <div class='pure-u-19-24 pure-u-sm-5-6 event-description'>
            {% if event.photo != null -%}
                <div class='visible-at-medium float-right-medium' style='height:100%'>
                <a class='photo-box' href='{{event_photo}}'><img src='{{event_photo}}'/></a>
                </div>
            {%- endif %}
            <span class='heading'>{%- include text_process.md data=event.headline -%}</span>
            {% if event.location != null -%}<div class='event-location'>(&hairsp;{{- event.location -}}&hairsp;)</div>{%- endif %}
            <p>
            {% include text_process.md data=event.content %}
            {% if event.photo != null -%}
            <br>
            <a class='hidden-at-medium' href='{{event_photo}}'><img src='{{event_photo}}'/></a>
            {%- endif %}
        </p>
        </div>
    </div>
   
{%- endfor %}
</div>