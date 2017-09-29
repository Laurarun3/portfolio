---
title:  "Home"
---

{% include header.md %}

<div class="container-grid container-grid--boxed container-grid--homepage">
    <header>
        Menu
    </header>
    <section>
        <div class="container-grid container-grid--items2">
            {% for post in site.posts %}
            <div class="item">
                <a href="{{ post.url }}">{{ post.title }} &mdash; {{ post.date | date: "%d-%m-%Y" }}</a>
                <p>{{ post.content }}</p>
            </div>
            {% endfor %}
        </div>
    </section>
    {% include footer.md %}
</div>
