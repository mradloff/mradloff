# mradloff
Website for Michael Radloff, using jekyll as the site generator

# Editing the Site
This website is using jekyll + markdown. Markdown provides a very simple way to separate content from formatting (mostly). To get started with makrdown, check out this excellent [Markdown Guide](https://help.ghost.org/hc/en-us/articles/224410728-Markdown-Guide).

## Adding a new page
To add a new page to the site, just add a new file inside the `pages` folder. Name it something like `newpage.md` (the `.md` is important). In addition to making this new file, add this to the following top of the file. This lets jekyll the website generator know how to link things up. Just edit the things that say `replaceme`.

```
---
layout: default
title: REPLACEME
permalink: /replaceme/
---
```

Below this information, you can add anything you want like normal.

## Editing an existing page
Most pages are contained within the `pages` folder. The only one that is not here is `index.html` which is the main page.

## Other Information
To edit things like name, contact info, etc modify `_config.yaml`. To include these variables into pages, you do something like this anywhere in your pages:

```
_config.yml
...
phone: 123-456-7890

pages/page1.md
...
This is my phone number: {{site.phone}}
```
