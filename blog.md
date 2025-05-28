---
layout: default
title: Blog - Real-Life Parenting Stories & Tips from a Dad of Eight
description: Dive into the latest blog posts from Dad in Command, sharing honest stories, budgeting tips, fun trip ideas, and insights from a chaotic home life with eight children.
image: /assets/social-share-blog.jpg # Optional: Path to a social sharing image for your blog listing page
---

<section class="blog-post">
  <h2>Latest Blog Posts</h2>
  {% for post in site.posts %}
    <article>
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      <a href="{{ post.url | relative_url }}" class="read-more">Read More &rarr;</a>
    </article>
  {% endfor %}
</section>

<style>
  /* Basic style for read more link if not already in style.css */
  .read-more {
    display: inline-block;
    margin-top: 0.5rem;
    font-size: 0.9em;
  }
</style>
