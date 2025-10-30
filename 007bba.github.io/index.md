---
layout: default
title: 首页
---

# 欢迎来到我的技术博客

这里是我分享技术心得和学习笔记的地方。

## 最新文章

<ul class="post-list">
  {% for post in site.posts limit:5 %}
    <li>
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <span class="post-date">{{ post.date | date: "%Y年%m月%d日" }}</span>
      <p>{{ post.excerpt | strip_html | truncate: 150 }}</p>
    </li>
  {% endfor %}
</ul>

<p><a href="{{ '/posts' | relative_url }}">查看所有文章 →</a></p>

## 关于我

我是廖家龙，一名 Java 工程师，专注于后端开发和系统架构。

- 💼 技术栈：Java, Spring Boot, MySQL, Redis
- 📚 正在学习：微服务架构、云原生技术
- 📧 联系我：2091772139@qq.com