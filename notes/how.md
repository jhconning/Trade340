---
title: how
tags: [post]
created: '2021-01-04T05:16:39.780Z'
modified: '2021-01-28T02:14:58.788Z'
jupytext: {cell_metadata_filter: '-all', formats: md:myst, text_representation: {extension: .md, format_name: myst}}
kernelspec: {display_name: Python 3, language: python, name: python3}
---

# How this site was built

This site's content was written with [markdown](https://commonmark.org/help/) and jupyter notebook files and then rendered as this static HTML website (via github pages).  

This site supports the Spring 2021 Eco 340 [tophat course site](https://app.tophat.com/e/054232). Tophat is used to deliver online assignments and some reading,  multimedia and interactive content.  Much of the content mirrored there was first edited here. 

Tools used:

- [Jupyter Book](https://jupyterbook.org) - Creates website with markdown and jupyter notebooks.  Files used for site are listed in the [_toc.yml](_toc.yml) table of contents file.
- [Typora](https://typora.io/) - a WYSIWYG markdown editor.  Pages here look close to rendered HTML or tophat pages.
- [Notable](https://notable.app/) ([beta release](https://github.com/notable/notable-insiders/releases)). Useful markdown app that keeps things organized with tags. 

- [YAML headers](https://yaml.org/)  - if you look at the raw markdown files you will see metadata (title, date created, modified, tags, etc) information stored in the header (before the `---` separator).  Notable and jupyterbook use this information but it is hidden on rendered pages.

## Interactive 'apps'

On some pages you'll see interactive widgets that allow you to interact with graphs.  All the embedded geogebra apps (javascript) should be interactive in any browser with an internet connection. To interact with python apps you'll usually have to launch the page first using the binder or Google Colab buttons that you'll see on the page.

- [Geogebra](https://www.geogebra.org/) 
- [Econ-Teach/trade](https://github.com/jhconning/Econ-Teach/tree/master/notebooks) python applets  


