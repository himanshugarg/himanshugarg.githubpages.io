<h1><a href="https://himanshugarg.github.io/">#HG: The Second Best Time is Now</a></h1>  

  <h4>{{ Practice }}</h4>
  
    {% for post in site.categories.practice %}
      <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
    {% endfor %}
    

  <h4>{{ Poem }}</h4>
  
    {% for post in site.categories.poem %}
      <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
    {% endfor %}
    
    
  <h4>{{ Personal }}</h4>
  
    {% for post in site.categories.personal %}
      <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
    {% endfor %}
