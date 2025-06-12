---
layout: default
---

# 📰 最新文章

{% for post in site.posts %}
  <div style="margin-bottom: 20px; padding: 15px; border-left: 3px solid #159957; background: #f6f8fa;">
    <h3><a href="{{ post.url | relative_url }}" style="text-decoration: none;">{{ post.title }}</a></h3>
    <p style="color: #666; font-size: 14px;">{{ post.date | date: "%Y年%m月%d日" }}</p>
    {% if post.excerpt %}
      <p>{{ post.excerpt }}</p>
    {% endif %}
  </div>
{% endfor %}
