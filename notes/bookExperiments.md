---
title: bookExperiments
title_custom: true
tags: [_Admin]
created: 2021-04-02T15:07:43.684Z
modified: 2022-01-22T19:27:34.003Z
---

# Jupyterbook Experiments


## Embedded Spreadsheets

Google sheets does not seem to work well, certainly not on rendered website.

<iframe width='70%' height='250' src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSuuPY8zzAnApMECZEb7VLjT-AGQr6B5ZsFweB3chmJ0QVwBO2R56uw7DzYW77BlFiAY-tKIUOK37HJ/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>


## Numbered Figures

Modeled after [this](https://jupyterbook.org/content/figures.html) jupyterbook documentation page, we should be able to get numbered figures.

Myst directive method:

```{figure} ../attachments/capital-intensity.png

---
height: 300px
name: cap-fig
---

Capital Intensity over time.
```

And another figure:

```{figure} ../attachments/Labor_demand1.png
---
height: 300px
name: lab-fig
---
A labor demand diagram.
```

Usual markdown image links also work (but less fine control over placement)
![](../attachments/boat.jpg)

Another method with colon fences (does not appear to work):

:::{figure-md} fig-target
:class: myclass

<img src="../attachments/boat.jpg" alt="boat" class="bg-primary mb-1" width="200px">

This is a caption in **Markdown**
:::

Capital Intensity over time.
:::


This seems to not work to caption figure with a number (need to list figure-md MyST extension on _config.yml... but maybe not working)

:::{figure-md} markdown-fig

<img src="../attachments/Labor_demand1.png" alt="Labor Demand" class="bg-primary mb-1" width="200px">

This is a caption in **Markdown**!

:::

Reference [](markdown-fig)

<!-- :::{note} -->
This text is **standard** _Markdown_
:::


```{note}
Here is a note
```

:::{admonition} This *is* also **Markdown**
:class: warning

This text is **standard** _Markdown_
:::


```{note}
Here is a note
```

