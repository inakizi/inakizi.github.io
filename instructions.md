# Instructions to build this project/site

## What is this Project?
This is a web page made using Jekyll that is published in GitHub pages

## To start the test server to view pages locally
```bash
bundle exec jekyll serve
```



## To update pages

### Create new pages
Just add and .md file in any nested folder or main folder, but the header of the .md file needs this content:
```yaml
---
layout: home
title: My website
subtitle: This is where I will try to share as much useful info as I can
---
```

### Add or remove links to pages in NavBar
Edit the file _config.yml
```yaml
navbar-links:
#  About Me: "aboutme"
  Apps&nbsp&nbsp&nbsp&nbsp&nbsp:
    - False Tap Stop: "FalseTapStop"
```
