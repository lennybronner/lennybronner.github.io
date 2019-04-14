---
layout: page
title: projects
permalink: /projects/
order: 2
---

<div>
  {%- if site.posts.size > 0 -%}
    <ul class="post-list">
      {%- for post in site.posts-%}
      <li>
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}

        <div style='display: block; margin: 0; white-space: nowrap; line-height: 0px;'>

          <div style='display: inline-block; width: 30%;'>
          <img style='diplay: block; width: 100%; height: auto; line-height: normal; vertical-align: middle;' src="/assets/images/{{ post.pic_folder }}/preview.png"/>
          </div>
          
          <div style='display: inline-block; padding-left: 10px; width: 70%; white-space:normal; line-height: normal; vertical-align: middle;'>
          <h3>
            <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
            </a>
            <span class="post-meta">{{ post.date | date: date_format }}</span>
            
            {%- if site.show_excerpts -%}
            <p class="small">{{ post.excerpt | strip_html | strip_newlines | truncate: 156 }}  </p>
            {%- endif -%}
          </h3>
          </div>

        </div>
      </li>
      {%- endfor -%}
    </ul>

  {%- endif -%}

</div>