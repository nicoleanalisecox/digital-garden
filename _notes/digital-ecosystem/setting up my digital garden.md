---
title: setting up my digital garden
---
It uses Maxime Vaillancourt's [digital garden Jekyll template](https://github.com/maximevaillancourt/digital-garden-jekyll-template) and I followed [his tutorial on how to set it up using Jekyll](https://maximevaillancourt.com/blog/setting-up-your-own-digital-garden-with-jekyll). This template is pretty gorgeous out of the box. 😍

I then followed The Refined Mind's [Obsidian Jekyll workflow](https://refinedmind.co/obsidian-jekyll-workflow) to connect my Obsidian to the Jekyll setup (using VSCode instead of Atom).

<hr>

After deploying the basic template files to Netlify, I also dug around the project files to personalise the existing config a bit more:

**in the page  files (in the `pages` directory)**:
- updated the content `index.md` file (this is the homepage)

**in the sass config file `_style.scss`**:
- changing the primary colour to indigo so the accent colour matches my personal site theme
- tweaking the margin and padding a little on different elements

**in the site config file `_config.yml`**:
- change the site title
- allowed embed tweets

**in the page layout files (in the `_includes` directory)**:
- updated the footer content in `footer.html`


Note: you made have to restart the server and rebuild to see some of the changes

To start development I run the terminal command  `bundle exec jekyll serve` in the directory of my project folder.

<hr>

> Now I can edit my notes in Obsidian then just commit and push the changes to my [digital garden GitHub repo](https://github.com/nicoleanalisecox/digital-garden) to deploy changes!

The first pages I started with were highly influence by some of [The Refined Mind's Digital Garden](https://refinedmind.co/).

- [[changelog]]
- [[digital gardening]]
- [[themes]]

I also added [[garden landscape 🌳]] as a starting point for visitor exploration.
