---
title: Names, Tags, and Tricks
tags: [how]
created: '2021-02-09T15:59:35.366Z'
modified: '2021-02-23T20:03:42.985Z'
---

# Names, Tags, and Tricks


## Names
Each question gets a question name or label, which is also the note name.  
For example, take the note [RMM101.md](./RM1101.md). The `RM` indicates the question topic is the Ricardian Model, the next `M` indicates this is a multiple choice question.  The first digit in `101` indicates that this is an easy question (levels 1, 2, and 3) and the remaining digits are just arbitrary numbering.

The aim is to end up with a unique question identifier that quickly conveys some information.

In addition to this we will use tags which notable will place into the YAML note header. These will help us quickly sort things inside notable and keep track of things such as whether the question is draft or finished, when it might have been used, etc.

## See [TagSystem](TagSystem.md)

Tags help us keep questions organized by topic, whether the question still needs a fix or not, whether it's been sent to tophat yet, etc. 




## Comments
We want to be able to enter comments to ourselves in the markdown that don't get exported to HTML or to Tophat.

Currently preferred method (in effect an incomplete footnote):
```
[^comment]: This is a long comment 
   If we indent we can continue.
   The content will not be exported.
```


Here are a few other methods:
- Enter a comment in the header YAML (in notable Ctrl+Alt+Shift+E). For example: `comment: the image source is ...`
- Use syntax like the following anywhere in the note:

One method (there must be a blank line before): 

`[//]: # (This will be a comment)`  

[//]: # (This will be a comment)

Another method using html tags (this seems to not work... markdown exports will send this):
`<!--Another (HTML) way to do comments    -->`

<!--Another (HTML) way to do comments    -->
This will show up in the editor view but not in any rendered view or export.
