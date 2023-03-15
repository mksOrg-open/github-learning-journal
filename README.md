# Github Learning Journal

> Open source learning journal

### Run using docker

```
    docker build -f Dockerfile -t docsify/demo .
    docker run -itp 3000:3000 --name=docsify -v $(pwd):/docs docsify/demo

```

Ignoring Subheaders

When subMaxLevel is set, each header is automatically added to the table of contents by default. If you want to ignore a specific header, add <!-- {docsify-ignore} --> to it.

```markdown
# Getting Started

## Header <!-- {docsify-ignore} -->

This header won't appear in the sidebar table of contents.
```


To ignore all headers on a specific page, you can use <!-- {docsify-ignore-all} --> on the first header of the page.

```markdown
# Getting Started <!-- {docsify-ignore-all} -->

## Header

This header won't appear in the sidebar table of contents.
```



[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
