---
title: how
title_custom: true
tags: [_Book/Modules, _Book/Modules/M95_Site, x/posted]
created: '2021-01-04T05:16:39.780Z'
modified: '2021-02-23T16:22:50.061Z'
jupytext: {cell_metadata_filter: '-all', formats: md:myst, text_representation: {extension: .md, format_name: myst}}
kernelspec: {display_name: Python 3, language: python, name: python3}
---

# How this site was made (and why)

## The Problem

Learning Management Systems (LMS) such as Tophat (or Blackboard, Canvas, etc) render content as HTML in the browser but have proprietary ways for creating, editing, and storing content.  

Although these LMS page creation tools appear to be built around open standard formats such as markdown, HTML and Katex (for math), they make it hard to take content that you might have typed into the LMS back out again.  For example in Tophat: 
- You usually can't simply copy content from a Tophat page and paste it into a word processor, or vice-versa.
- Once you insert an image or embed using an `<iframe>` there is no evident way to recover the image filename or the iframe syntax you used.
- You can upload certain types of questions in text form, but once uploaded you cannot export back to text.

All this frustrates logical content creation and feedback loop processes. It becomes all but impossible to keep content under version control.   

Large content creation providers (and any corporation that wants to manage website updates in a logical coherent manner) have, of course, long recognized this problem.  LMS systems do in principle support exchanging content using a standard called SCORM.  There are 'SCORM authoring systems' that allow users to create and organize content on the authoring platform and then export to whatever LMS system is needed.  But these authoring systems can be expensive or hard to use, and LMS systems such as Blackboard and Tophat don't at all make it easy for consumer users to access this functionality (e.g. Tophat mentions on its website that it is SCORM compatible but no evident import or export functionality is made available).

## A solution of sorts

It's become quite easy to create nice looking websites using markdown, katex and a few simple tools. 

My aim here is to show how we can have a markdown-based content creation system to organize content into a website that can be kept under version control and can then be rendered in HTML in a format that largely replicates what things will look like in the LMS (minus actually working autograded questions). 

My immediate use, is to help me keep materials organized for teaching my Eco 100 (Intro to Economics) and Eco 340 (International Trade) courses.  A longer term goal is to use workflows like these to make it easier to collectively write and edit the 'Hunter Experience' textbook.

## Some details of how it works

All the content of this site written in [markdown](https://commonmark.org/help/) either in simple markdown files or using markdown and code in jupyter notebooks. The files are kept under version control in a github repository. 
I use the jupyterbook package to create a static HTML website that renders the content files as HTML (similar to how they might look on an LMS).  I can render this website locally on my computer or trigger online via github pages.  


and a mock-up of the [tophat course site](https://app.tophat.com/e/054232) materials for a course. Tophat is used to deliver online assignments and some reading,  multimedia and interactive content.  Much of the content mirrored there was first edited here. 

Tools used:

- [Jupyter Book](https://jupyterbook.org) - Creates website with markdown and jupyter notebooks.  Files used for site are listed in the [_toc.yml](_toc.yml) table of contents file.
- [Typora](https://typora.io/) - a WYSIWYG markdown editor.  Pages here look close to rendered HTML or tophat pages.
- [Notable](https://notable.app/) ([beta release](https://github.com/notable/notable-insiders/releases)). Useful markdown app that keeps things organized with tags. 

- [YAML headers](https://yaml.org/)  - if you look at the raw markdown files you will see metadata (title, date created, modified, tags, etc) information stored in the header (before the `---` separator).  Notable and jupyterbook use this information but it is hidden on rendered pages.



## Interactive 'apps'

On some pages you'll see interactive widgets that allow you to interact with graphs.  All the embedded geogebra apps (javascript) should be interactive in any browser with an internet connection. To interact with python apps you'll usually have to launch the page first using the binder or Google Colab buttons that you'll see on the page.

- [Geogebra](https://www.geogebra.org/) 
- [Econ-Teach/trade](https://github.com/jhconning/Econ-Teach/tree/master/notebooks) python applets  
- Embedded videos 


