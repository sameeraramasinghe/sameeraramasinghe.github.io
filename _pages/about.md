---
permalink: /
title: "Bio"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a post doctoral researcher at Australian Institute for Machine Learning (AIML). Before that, I was a Computer Science PhD student at The Australian National University, supervised by Dr. Salman Khan, Prof. Nick Barnes and Prof. Stephen Gould. My research focuses on incorporating inductive biases into deep neural networks towards better performance.

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

# News

* [October '21] Our paper "Rethinking Conditional GAN Training" got accepted to NeurIPS 2021 [(Arxiv)](https://arxiv.org/abs/2011.13055).
* [May '21] Our paper "Synthesized Feature based Few-Shot Class-Incremental Learning on a Mixture of Subspaces" got accepted to ICCV 2021 [(Link)](https://openaccess.thecvf.com/content/ICCV2021/papers/Cheraghian_Synthesized_Feature_Based_Few-Shot_Class-Incremental_Learning_on_a_Mixture_of_ICCV_2021_paper.pdf).
* [April '21] Joined AIML as a postdocoral researcher.
* [January '21] Our paper "Conditional Generative Modeling via Learning the Latent Space" got accepted to ICLR 2021 [(Arxiv)](https://arxiv.org/abs/2010.03132).
* [July '20] I was featured in the newsletter (Vol. 42 #3) of the International Association for Pattern Recognition (IAPR) in recognition for my latest contributions [Link](https://iapr.org/docs/newsletter-2020-03.pdf).
* [July '20] Our paper "Spectral-GANs for high-resolution 3D point cloud generation" got accepted to IROS 2020 [Link](https://ieeexplore.ieee.org/iel7/9340668/9340635/09341265.pdf). 
* [Feb '20] Our paper "Blended convolution and synthesis for efficient discrimination of 3d shapes" got accepted to WACV 2020 [Link](http://openaccess.thecvf.com/content_WACV_2020/papers/Ramasinghe_Blended_Convolution_and_Synthesis_for_Efficient_Discrimination_of_3D_Shapes_WACV_2020_paper.pdf).
* [January '20] Our paper "Learned and Hand-crafted Feature Fusion in Unit Ball for 3D Object Classification" won the best student paper award at ICPRAM 2020 [Link](https://www.scitepress.org/Papers/2020/93448/93448.pdf).
* [July '19] Our paper "Representation learning on unit ball with 3d roto-translational equivariance" got accepted to IJCV [Link](https://link.springer.com/content/pdf/10.1007/s11263-019-01278-x.pdf).
* [January '18] Our paper "A context-aware capsule network for multi-label classification" got accepted to ECCV workshops 2018 [Link](http://openaccess.thecvf.com/content_ECCVW_2018/papers/11131/Ramasinghe_A_Context-aware_Capsule_Network_for_Multi-label_Classification_ECCVW_2018_paper.pdf).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
