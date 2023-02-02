---
title: Research Timeline  (csv)
---

<section id="timeline">

<h1>Research Timeline Summary</h1>
<ul class="timeline_ul">
{% for Rstats in site.data.ResearchStatsFbs %}
  <li  class="timeline_card">
    
    <div class="timeline_head online">
      <div class="date_other" > {{ Rstats.Date }} </div>
      <div class="date_online" > {{ Rstats.Title }} </div>
    </div>
    <div class="timeline_body">
      <h2>Description</h2>
      {{ Rstats.Description }}
      
      <h2>What we learned</h2>
      {{ Rstats.Learned }}

      <h2>Themes</h2>
      {{ Rstats.Themes }}
      
      <h2>Insights</h2>
      {{ Rstats.Insights }}
      
      <h2>Recommendations</h2>
      {{ Rstats.Recommendations }}
      
      {% unless {{ Rstats.Quotes }} == "" %}
        <h2>Quotes</h2>
        {{ Rstats.Quotes }}
      {% endunless %}

    </div>
  </li>
{% endfor %}
</ul>
  
</section>
