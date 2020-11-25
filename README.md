# Bita - Hugo theme
Bita is a minimal and clean theme for hugo with a markdown-ish UI.

Forked from [Archie theme](https://athul.github.io/archie/), which is forked from [Ezhil Theme](https://github.com/vividvilla/ezhil)

## Demo

[Check the Demo](https://eriverosr.github.io/bita/) hosted on GitHub Pages :smile: . You can find the source code to that in the `site` branch of this repository

![](/images/theme.png)
![](/images/bita-dark.png)
## Feature
- Matomo Script
- Callouts
- Tags
- Auto Dark Mode(based on system theme)
- tl:dr; frontamatter

## Installation
In your Hugo website directory, create a new folder named theme and clone the repo
```bash
$ mkdir themes
$ cd themes
$ git clone https://github.com/eriverosr/bita.git
```
Edit the `config.toml` file with `theme="bita"`
For more information read the official [setup guide](https://gohugo.io/overview/installing/) of Hugo.

## Writing Posts
Create a new `.md` file in the *content/posts* folder
```yml
---
title: Title of the post
description:
date:
tldr: (optional)
draft: true/false (optional)
tags: [tag names] (optional)
---
```

## Credits
Forked from [Ezhil Theme](https://github.com/vividvilla/ezhil) and Licensed under MIT License 
Inspired by design of blog.jse.li

----

## Config of the Demo Site

```toml
baseURL = "https://eriverosr.github.io/bita/"
languageCode = "en-us"
title = "Bita"
theme="bita"
copyright = "©"
# Code Highlight
pygmentsstyle = "solarized-dark"
pygmentscodefences = true
pygmentscodefencesguesssyntax = true

paginate=3 # articles per page

[params]
	mode="auto" # color-mode → light,dark or auto
	useCDN=false # don't use CDNs for fonts and icons, instead serve them locally.
	subtitle = "Minimal and Clean [blog theme for Hugo](https://github.com/eriverosr/bita)"

# Social Tags

[[params.social]]
name = "GitHub"
icon = "github"
url = "https://github.com/eriverosr/bita"

[[params.social]]
name = "Twitter"
icon = "twitter"
url = "https://twitter.com/adderou/"

[[params.social]]
name = "Linkedin"
icon = "gitlab"
url = "https://gitlab.com/eriverosr/"

# Main menu Items

[[menu.main]]
name = "Home"
url = "/"
weight = 1

[[menu.main]]
name = "All posts"
url = "/posts"
weight = 2

[[menu.main]]
name = "About"
url = "/about"
weight = 3

[[menu.main]]
name = "Tags"
url = "/tags"
weight = 4
```
