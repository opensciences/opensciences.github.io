---
title: OpenScience Documentation
layout: repopage
---

# Web Developer/Systems programmer
The web developer/systems programmer ("Develoepr") has the following general responsibilities:
 * Maintain and expand the site using the Jekyll framework
 * Work with the Curator to develop efficient processes to add datasets to the repository

The specific work that the Developer does varies widely and is largely contingent upon what Dr. Menzies (the current leader of the OpenScience project) wants to be done. Here are some examples of work that has been done in the past, on version 4 of the tera-PROMISE repository:

 * Add a search engine
 * Add Google analytics to the site
 * Reorganize the structure of certain parts of the site (for example, the people page)
 * Systematically remove dead links
 * Add a contribute section to the site
 * Modify small HTML/CSS features in the site

The website is built with the Jekyll framework; almost all of the work done on the site will have some relevancy to Jekyll, so it's important to know how it works. The Jekyll site has a good [documentation section](http://jekyllrb.com/docs/home/) if you're unfamiliar with how it works (also, you can read the next section for a basic overview of how the OpenScience site is built with Jekyll).

# How Jekyll works

The [Jekyll documentation](http://jekyllrb.com/docs/home/) provides a good, much more in depth tutorial on how it works, but here are a few key pointers that are relevant to the OpenScience site:
 * ```_config.yml``` contains some site settings like site names, authors, markdown versions (Jekyll uses markdown for much of the content), and other variables.
 * ```_includes``` is a directory containing HTML snippets that will be inserted in other pages with the Liquid templating engine (next section).
 * ```_layouts``` is a directory containing default page layouts, constructed with snippets from ```_includes``` and with statements from the Liquid templating engine.
 * ```_posts``` is a directory that contains only Jekyll posts. All description pages for the datasets housed in tera-PROMISE are Jekyll posts, written purely in [markdown](http://daringfireball.net/projects/markdown/) and [Front Matter](http://jekyllrb.com/docs/frontmatter/) (see the YAML/Front Matter section below). For each category in the tera-PROMISE repo, there's a ```_posts``` directory in the directory for that category which contains the datasets in the category. For example, the directory structure for a dataset in the [Green mining](http://openscience.us/repo/green-mining/) section is this: ```/repo/green-mining/_posts/2015-03-15-greentrace.md```

# How Liquid works

Liquid is a templating engine that allows Jekyll to create and fill in templates. [Here](http://liquidmarkup.org/) is the website; its documentation is a bit spotty but feel free to look around the GitHub site to see examples of Liquid being used. It's most common in the ```_layouts``` folder.

# How YAML and Front Matter work

On the top of each description page in ```_posts``` is a few lines of metadata preceded and followed by three dashed lines, like this:
```
---
title: splot
excerpt: "Scaling Exact Multi-objective Combinatorial Optimization by Parallelization"
layout: repo
authors: "Marcilio Mendonca, Moises Branco, Donald Cowan"
version: 4
---
```

Many of the older datasets don't have as much metadata, but the newer ones should all follow the above standard.

The metadata described in more detail:
 * ```title``` The dataset name
 * ```excerpt``` The blurb about the dataset, almost always a paper title associated with the dataset
 * ```layout``` The layout of the page; the different types are outlined below.
 * ```authors``` The authors of the dataset
 * ```version``` The current version of tera-PROMISE. This number will probably stay at 4 for a good while.

```layout``` defines the type (and layout) of page that the markdown content will be put into; the layouts come from the ```_layouts``` directory. The layouts related to the repository are ```repo```, ```repopage```, ```main```, and ```content```.
 * The ```repo``` layout is for pages in the repository that aren't dataset pages.
 * The ```repopage``` layout is for dataset pages ("description pages").
 * The ```main``` layout is for...
 * The ```content``` layout is for...




