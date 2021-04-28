# the-allsite
A starter kit for your own Hugo site. Yes! You can see how this template / sample site looks by visiting https://oursite.pages.dev.

## This repository is meant for use with services like Cloudflare Pages. 

In order to use it:

1. Fork the repository
2. Add the forked repository  to your Cloudflare Pages account (authorize Pages to access the repository). 
3. In your project on cloudflare pages, select the forked repository. 
4. Deploy the repository, specifying Hugo as the Framework Preset, and use this environment variable- "HUGO_VERSION" : "0.82.1". 
5. Deploy!

You can see the results of this original repository being built into a site at: https://oursite.pages.dev :) 

### Changing Title, Author, Footer Text, Etc.

In the site directory, CONFIG.TOML is the file that contains the necessary information and parameters to control home page content.

For easy acces, you will see a number in parentheses next to the text so that you know which line to alter in CONFIG.TOML. Example:

In the upper left corner, the title is "TITLE (2)". To change it, go to line 2 of CONFIG.TOML and edit the entry on the right side of the equal sign. 

> title = "title (2)"  

To change the above, edit the text to the right of the equal sign, in betwen the quotes.

### Creating New Posts

All content posts go into the Content directory as markdown files. Anything in the Blog section should go under content/posts.
 
Steps:
1. Create a new file in the respective directory with an extension: .md (example: test.md)
2. In this new file, be sure to include front matter (metadata of sorts) in this format so the site generator knows how to handle the post:

START OF EXAMPLE: 

+++
title = "Your Title"
description = "Your description"
draft = "false"
date = 2021-04-26T20:37:10+08:00
tags = ["one", "two", "three"]
categories = ["one", "two"]
series = ["food", "water"]
+++

# Your Content goes here. (a hashtag followed by a space in Markdown files creates a Heading, size 1)
## More content here (heading, size 2, and so on.)

Normal text.

END OF EXAMPLE.

3. If you are editing on github.com directly, changes will go to your site as soon as you commit them to the master branch.
4. If you are editing remotely, changes go live as soon as you push changes to the master branch.



