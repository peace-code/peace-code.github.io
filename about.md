---
layout: page
title: 소개
---
<h2>피스코드 Peacecode</h2>
<p class="message">
  안녕하세요! 우리는 피스코드에요! 놀랍게도 세계 평화를 위해 코드를 쓰고 서비스를 만들고 있어요!
  가장 중요한 원칙은 서로의 의견을 경청하고 존중하면서 키보드와 마우스를 잡고 만들어내는 겁니다!
</p>

<ul>
  {% for repo in site.github.public_repositories %}
  <li>
    <h2><a target="_blank" href="{{ repo.html_url }}">{{ repo.name }}</a></h2>
    <p>{{ repo.description}}</p>
  </li>
  {% endfor %}
</ul>

<p class="message">
  <address>
	<strong>이메일</strong><br>
	<em>contact@peacecode.org</em>
  </address>

  {% include contact_static.html %}
  
</p>