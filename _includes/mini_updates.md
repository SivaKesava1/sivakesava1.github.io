
<div>
<h4 class="updates-small-caps"> <i class='far fa-fw fa-sm fa-clock'></i> Recent Updates <em> &middot; &middot; &middot;</em> (<a href="/updates"> Details </a>)</h4>
</div>

<div class='mini-events'>
    <div class='flex-container'>
    {%- assign sorted_updates = site.updates | sort: 'date' | reverse -%}
    {%- for event in sorted_updates limit: 5 -%}
        {%- assign eventdate = event.date | date: '%s' -%}
        {%- assign highlight = event.highlight | default: site.default_highlight[event.type] -%}
        <!-- <div class='flex-container'> -->
        <div class='event-date flex-test flex-date'>
        {%- if event.end_date == null -%}
            {{- event.date | date: "%b" -}}<i>{{- event.date | date: "%y" -}}</i>
        {%- else -%}
            {%- assign year = event.date | date: "%y" -%}
            {%- assign end_year = event.end_date | date: "%y" -%}
            <div class='multimonth'>{{- event.end_date | date: "%b" -}}<i>{{- end_year -}}</i><br><b>&#8942;</b><br>
            {{- event.date | date: "%b" -}}<i>{{- year -}}</i>
            </div>
        {% endif %}
        </div>
        <div class='event-icon flex-test flex-icon color-more-faded {% if highlight %} color-{{ highlight }} {% endif %}'>
            <i class='fas fa-fw fa-{{ event.icon | default: site.default_icon[event.type] }}'></i>
        </div>
        <div class='event-description flex-test flex-description'>
          {% include text_process.md data=event.headline %}
          {% if event.location != null -%}
            <div class='event-location'>(&hairsp;{{event.location}}&hairsp;)</div>
          {%- endif %}
        </div>
        <!-- </div> -->
    {% endfor %}
    </div>
</div>