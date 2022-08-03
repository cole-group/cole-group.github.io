---
layout: post
title:  "How to add a blog post"
date:   2021-05-09
---

# Welcome!

The source for this blog may be found [here][blog-source].

Feel free to suggest a blog post on any topic you like. It could be a summary of a paper with code, computational tools or techniques that others might find useful, or a piece of outreach writing. Any length is absolutely fine. Remember to link to the original paper or software if you're building on the work of others.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.markdown` and includes the necessary front matter (see the first 5 lines of the source for this post).

You'll find this post in the `_posts` directory. Download or copy the raw source of this post to get an idea about how it works and use it as a template for writing your own.

Once done, you can initialise a pull request to merge your changes, or simply send your post to **DC**.

To include an image in your post:

![QUBEKit logo](/assets/QuBeKit.png)

or [link to it in the text](/assets/QuBeKit.png).

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
from qubekit.charges import DDECCharges, ExtractChargeData
from qubekit.molecules import Ligand
from qubekit.nonbonded import VirtualSites
from qubekit.parametrisation import OpenFF

# Load the molecule into QUBEKit from file.
molecule = Ligand.from_file("methylisocyanate.pdb") # Generate basic parameters using OpenFF.
OpenFF().run(molecule)

# Extract charge data and save to be used in the virtual sites fit.
ddec_file_path = "ChargeMol"
ddec_version = 6

ExtractChargeData.extract_charge_data_chargemol(
    molecule, ddec_file_path, ddec_version
)

# Apply symmetry to the reference data (optional).
DDECCharges.apply_symmetrisation(molecule) # Fit virtual sites to the molecule.
VirtualSites().run(molecule)

# Write the force field parameters to file.
molecule.write_parameters("methylisocyanate.xml")
{% endhighlight %}

## How to find out more

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[blog-source]: https://github.com/cole-group/cole-group.github.io
[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
