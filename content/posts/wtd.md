---
title: "Better Docs"
date: "2015-10-06"
description: "Improve your work-flow and your docs"
categories: 
    - "wtd"
   
---


## X Tips to improve your docs

It is not a secret, good documentation will improve your product. Still lots of people are not writing documentation at all or think a comment in the code base is more than enough.
This is just sad .....

There are a lot of different ways how to document, often it is not about right or wrong but about what style fits you the best.

IMHO it doesn't matter which style of docs you choose, as far as you are consistent.


## Work-flow

Do micro-commits, meaning if you worked om something which needs documentation, do that now even if it is not fully perfect written yet, just document what you did in a few words or couple of lines, you still know what you did and why.

Doing that two weeks later will be much harder because you will not remember everything and you will also have less motivation. 

## Tools

There are a wide variety of tools which can help you with documentation, it also depends on your style of documentation and what kind of software you use.

For this posting we will use Sphinx as software of our choice and restructured text ``rst`` as language syntax we write in.

### Editor

Configure your editor of choice for spell-check and rst-linting.

![Sublime Editor](/img/editor.png) 

Use [OmniMarkupPreviewer](https://github.com/timonwong/OmniMarkupPreviewer) to review your docs.

OmniMarkupPreviewer is a plugin for both Sublime Text 2 and Sublime Text 3 that preview markups in web browsers. It also renders markups into htmls and send it to web browser in the backgound, which enables a live preview.

### Git

Use a githook to remind you to do documentation and for basic checks.

![Githook Example](/img/screen_githook_example.png) 

See the gist:

{{< gist 30ff90ad5796a244494f >}}

### mr.docs

Usually I work on documentation from different projects, which all have the same setup. I was looking for a way to install all the dependencies once into one place, why should I have to install the same packages all over and over again.

Since I always or let's say most of the time have the same setup, meaning we have a README and all documentation under /docs, written in plain ``rst``, build and tested with [Sphinx](http://sphinx-doc.org/), this was an easy one to solve.

Hello **mr.docs** !

[mr.docs](https://github.com/tiramisusolutions/mr.docs) is a fully pre-configured sphinx setup, running in a docker container. Please see the [project documentation](https://mrdocs.readthedocs.org/en/latest/) for more info.

See the video for a short introduction.


{{< youtube TsCUMRN41U0 >}}

mr.docs is not finished yet, I am still working on some rough edges, but for a 0.1 version the result makes me happy.


