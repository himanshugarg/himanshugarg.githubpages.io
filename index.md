### HG: The Second Best Time is Now

#### {{ Practice }}
  
{% for post in site.categories.practice %}
  <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
{% endfor %}
    
#### {{ Poem }}
  
{% for post in site.categories.poem %}
  <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
{% endfor %}

#### {{ Personal }}
  
{% for post in site.categories.personal %}
  <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
{% endfor %}
