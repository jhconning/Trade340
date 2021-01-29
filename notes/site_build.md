---
title: site_build
title_custom: true
created: '2021-01-29T05:09:57.448Z'
modified: '2021-01-29T05:24:38.893Z'
---

# Site build details

### Jupyterbook

- key files are `_config.yml` and
-  `_toc.yml` specifies the markdown and notebook files that form part of the site navigation and content.
  - these are in local `book/` folder which is kept under version control at [github.com/jhconning/Trade340](https://github.com/jhconning/Trade340)
- `jb build book/`

### Notable markdown app
- I keep things organized on my local drive using the Notable app which uses tags.  These tags appear as YAML headers but don't show up in rendered site.


### Github Actions
- After every push a github action is triggered that builds a virtual machine on which an instance of jupyterbook will be installed to build the website and deploy it to https://jhconning.github.io/Trade340/
- You can see the deployment process by clicking the `Actions` tab at https://github.com/jhconning/Trade340
- It may take several minutes for the new site to show up on [jhconning.github.io/trade340/](https://jhconning.github.io/Trade340/)
