---
layout: post
title:  "SOCIAL"
date:   2014-07-21 08:00:00
isStaticPost: true
---

Curta, siga, conecte-se conosco!

<div class="row">
  <div class="col-md-12 col-xs-12">
    <ul class="social-links" style="padding-left: 0">
      {% for social in site.socialLinks %}
      <li>
        <a href="{% if social.permalink != null %} {{ social.permalink | prepend: site.baseurl }} {% else %} {{ social.link }} {% endif %}" target="_blank">
          <svg class="icon icon-{{ social.icon }}" viewBox="0 0 30 32">
            <use xlink:href="{{ site.baseurl }}/img/sprites/sprites.svg#icon-{{ social.icon }}"></use>
          </svg>
        </a>
      </li>
      {% endfor %}
    </ul>
  </div>
</div>