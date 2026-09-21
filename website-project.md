---
layout: single
title: "Portfolio Website"
permalink: /portfolio/website-project/
---
[← Back to Portfolio](/portfolio/){: .btn .btn--info}
![BNM Repo](assets/images/website-screenshot.jpg){: .align-center width="600px"}
This website itself is a project, being a GitHub Pages site built on the Minimal Mistakes Jekyll theme to house my resume, portfolio, and blog. Going in, I didn't have much hands-on HTML experience, so this became as much a learning project as a finished product. Some learning takeaways were figuring out how a static site generator actually works, how Jekyll's templating and front matter fit together, and how to debug real configuration issues when something broke.

## Working with AI as a Learning Tool

I built this site with Claude as a pair programmer. I didn't have the HTML/Jekyll background to have built this from scratch on day one, so I used AI the way I'd use a more experienced developer sitting next to me. Conversations between the AI assistant and me included prompts such as asking what a piece of syntax does before using it, getting explanations for why something broke, and working through fixes step by step rather than copy-pasting a fully built site. The result is that I came out the other side actually understanding how the pieces fit together, including front matter, Liquid templating, YAML configuration, and Jekyll's build process, rather than just having a working site I couldn't explain.

## The Pagination Bug

The most instructive bug came from a conflict I didn't see coming. Early on, I renamed my homepage from `index.html` to `index.md` to fix a rendering issue. Markdown-formatted buttons were showing up as plain text instead of styled links, because Jekyll only runs its Markdown converter on `.md` files, not `.html` files. At the time, that fix worked perfectly. But later, when I wanted the homepage to automatically show my most recent blog posts, I ran into a wall: Jekyll's classic pagination plugin (the only one available on GitHub Pages) has a hard-coded requirement that the paginated page be named exactly `index.html`. The two fixes were in direct conflict.

The solution was to go back to `index.html`, but instead of relying on Markdown syntax for the buttons, write them as plain HTML directly in the file. Since Jekyll still processes front matter and Liquid tags on `.html` files, this let me keep both the styled buttons and working pagination at the same time.

## Takeaways

Building this site was a crash course in how static site generators work, how to read and act on error messages instead of being intimidated by them, and how to use AI assistance in a way that actually builds understanding rather than just producing output. It's a small project in scope, but it's the one piece of my portfolio that's live and actively evolving, considering my constant additions to it.
