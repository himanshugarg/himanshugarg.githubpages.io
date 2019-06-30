<h1><a href="https://himanshugarg.github.io/">#HG: The Second Best Time is Now</a></h1>  
{% for post in site.posts %}
  <h5>    <a href="{{ post.url }}">{{ post.title }}</a> </h5>
{% endfor %}
{% for cat in page.categories %}
  <h4>{{ cat }}</h4>
    {% for post in site.categories[cat] %}
      <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
    {% endfor %}
{% endfor %}
