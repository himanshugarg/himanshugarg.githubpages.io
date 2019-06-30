<h1><a href="https://himanshugarg.github.io/">#HG: The Second Best Time is Now</a></h1>  
{% for cat in site.categories %}
  <h4>{{ cat }}</h4>
  
    {% for post in site.categories[cat] %}
      <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
    {% endfor %}
    
{% endfor %}
