---
title: jb_tricks
title_custom: true
tags: [_Book/Modules, _Book/Modules/M95_Site]
created: '2021-01-30T03:39:42.302Z'
modified: '2021-02-23T14:08:57.122Z'
---

# Using Jupyterbook

The website was created using the [jupyterbook](https://jupyterbook.org/) project (which in turn builds on [Sphinx](https://www.sphinx-doc.org/))

The site serves partly as a mock-up website with rendered output very similar to the final content we will move into the Tophat course site. This is useful because once content is placed in a tophat page it can't be easily retrieved or placed under version control.

Some of the pages don't get transferred to Tophat and instead contain draft material, or notes on how this site and other things are organized.

## Useful Jupyterbook methods and tricks

The jupyterbook project builds on Sphinx to provide syntax and directives to perform tasks and control the appearance of the final documents. We don't really need them much for our purposes, but some might be useful as a way to indicate formatting or leave comments as margin notes.

### Margin notes

```{margin} This is a margin note
On the rendered site it shows up as a note in the right margin of the page. We can use this to leave ourselves comments.  When we paste other content into tophat we'll ignore the margin notes.
```

### Links

One can link to other pages using either:
- `[Instructors](Instructors.md)` --> [Instructors](Instructors.md).

- `[Instructors](Instructors)` --> [Instructors](Instructors)

Links are more clunky in tophat (need to link to URL of target page)

### References and Citations

JB has syntax for [citations and references](https://jupyterbook.org/content/citations.html). 


### Inserting Images
These two ways will work to insert a image that will be visible both in markdown editor rending and in JB rendered HTML

The easiest is:
`![](../attachments/geogebra_embed.png)`

But we get more control (e.g. image sizing) with HTML

`<img src="media/geogebra_embed.png" style="zoom:60%;" />`







