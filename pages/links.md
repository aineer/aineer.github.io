---
layout: mypost
title: 友情鏈接
---

欢迎各位朋友与我建立友情鏈接，本站的友链信息如下:

```
名稱：{{ site.title }}
描述：{{ site.description }}
地址：{{ site.domainUrl }}{{ site.baseurl }}
頭像：{{ site.domainUrl }}{{ site.baseurl }}/static/img/logo.jpg
```

<ul>
  {%- for link in site.links %}
  <li>
    <p>{{ link.title }}<br> </p>
    <p>-> <a href="{{ link.url }}" title="{{ link.desc }}" target="_blank" >{{ link.url }}</a></p>
    <p>描述：{{ link.desc }}</p>
  </li>
  {%- endfor %}
</ul>
