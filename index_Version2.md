---
layout: home
title: "Welcome to WatchWala"
hero_image: "/assets/images/banner.jpg" # Change to your banner image path
---

<div class="hero">
  <img src="{{ page.hero_image }}" alt="WatchWala Banner" class="hero-img"/>
  <div class="hero-text">
    <h1>Welcome to <span style="color:#3949ab;">WatchWala</span></h1>
    <p>Discover elegant watches at the best prices.<br>
    Shop now for exclusive offers!</p>
    <a class="cta-button" href="/products/">Browse Products</a>
  </div>
</div>

<h2 style="text-align:center;margin-top:40px;">Featured Watches</h2>
<div class="product-list">
  {% for product in site.products limit:3 %}
    <div class="product-card">
      <a href="{{ product.url }}">
        <img src="{{ product.image }}" alt="{{ product.title }}" />
        <h3>{{ product.title }}</h3>
        <p>Price: {{ product.price }}</p>
      </a>
    </div>
  {% endfor %}
</div>

---

<div style="text-align:center;margin:40px 0;">
  <a href="/about/" class="about-link">About Us</a>
</div>
