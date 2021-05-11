---
layout: post
title:  "How to add a blog post"
date:   2021-05-09
---

# Welcome!

The source for this blog may be found [here][blog-source].

Feel free to suggest a blog post on any topic you like. It could be a summary of a paper (your's or other's) with code, tools or techniques that you use that others might find useful, or a piece of outreach writing. Any length is absolutely fine.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.markdown` and includes the necessary front matter.

You'll find this post in the `_posts` directory. Download or copy the raw source of this post to get an idea about how it works and use it as a template for writing your own.

Once done, you can initialise a pull request to merge your changes, or simply send your post to **DC**.

To include an image in your post:

![QUBEKit logo](/assets/QuBeKit.png)

or [link to it in the text](/assets/QuBeKit.png).

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def _monopole_esp_one_charge(charge: float, dist: float) -> float:
    """
    Calculate the esp from a monopole at a given distance
    :param charge: charge at atom centre
    :param dist: distance from sample_coords to atom_coords
        (provided as argument to prevent repeated calculation)
    :return: monopole esp value
    """
    return (charge * ELECTRON_CHARGE * ELECTRON_CHARGE) / (
        4 * PI * VACUUM_PERMITTIVITY * dist
    )
{% endhighlight %}

## How to find out more

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[blog-source]: https://github.com/cole-group/cole-group.github.io
[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
