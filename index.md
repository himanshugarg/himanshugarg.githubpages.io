<h4> Practice </h4>
  
{% for post in site.categories.practice %}
  <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
{% endfor %}
    
<h4> Poems </h4>
  
{% for post in site.categories.poem %}
  <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
{% endfor %}

<h4> Fiction </h4>
  
{% for post in site.categories.fiction %}
  <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
{% endfor %}

<h4> Personal </h4>
  
{% for post in site.categories.personal %}
  <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
{% endfor %}
