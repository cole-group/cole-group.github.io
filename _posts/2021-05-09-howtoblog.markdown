---
layout: post
title:  "How to add a blog post"
date:   2021-05-09
---

# Welcome!

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.markdown` and includes the necessary front matter.

You'll find this post in the `_posts` directory. Download or copy the raw source of this post to get an idea about how it works and use it as a template for writing your own.

Once done, you can initialise a pull request to merge your changes, or simply send your post to **DC**.

Include an image in the text:

![QUBEKit logo](/assets/QuBeKit.png)

or [link to it in the text](/assets/QuBeKit.png).

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def lj(r):
    """returns LJ potential for given r"""
    u_r = (sigma/r)**12 - (sigma/r)**6
    u_r = 4 * eps * u_r
    return u_r
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
