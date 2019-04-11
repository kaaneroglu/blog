---
layout: post
title: Hello world!
date: '2019-04-10 21:50:10 -0600'
categories: jekyll update
published: true
---
Just wanted to say `hello world` :)

Python code snippet test:

{% highlight python %}
# Route for READ all cuisines
@app.route('/')
@app.route('/cuisines', methods=['GET'])
def showCuisines():
    cuisines= session.query(Cuisine).all()
    return render_template('index.html', title='Restaurant Catalog', cuisines=cuisines)
{% endhighlight %}

