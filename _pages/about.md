---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hey there,

I am a final year dual degree (B.Tech + M.Tech) student in the Electrical Engineering (EE) Department, Indian Institue of Technology Bombay (IITB), Mumbai, India. I am working under the guidance of Prof. Subhasis Chaudhuri on some theoretical/mathematical aspects of deep learning for my master's thesis. Currently my focus is on large scale (non-convex) optimisation in deep learning using probabilistic techniques.

My primary interests lie in the theoretical understanding of deep learning with respect to its representational power, non-convex optimisation as well as deep learning for computer vision (specifically unsupervised or semi-supervised).

-A data-driven personal website
-======
-The academicpages template is based on structured data in the [YAML metadata language](http://docs.ansible.com/ansible/YAMLSyntax.html), which is stored various markdown (.md) and .yml files in your own public Github repository. The free [Github pages](https://pages.github.com/) service creates static HTML pages for the entire site based on these files. The HTML pages are automatically rebuilt every time the repository is updated. Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. 
-
-This approach is also useful because it makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, telling GitHub Pages how to transform that content & metadata into HTML pages. You can modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files with the content & metadata your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over-- just be sure to save the markdown files!
-
-Getting started
-======
-1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
-1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button on the top right.  
-1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be under "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
-1. Set site-wide configuration and create content & metadata
-1. Check status by going to the repository settings, in the "GitHub pages" section
-
-Site-wide configuration
-------
-The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 
-
-Create content & metadata
-------
-For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).
-
-Example: editing a markdown file for a talk
-![Editing a markdown file for a talk](/images/editing-talk.png "Editing a markdown file for a talk")
-
-For more info
-------
-More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
