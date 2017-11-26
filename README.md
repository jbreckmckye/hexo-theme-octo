# hexo-theme-octo

## What is this?

A Hexo-theme based on the 'classic' theme for Octopress 2.

## Notes for Octopress users

### This theme doesn't make Hexo understand Octopress markup

Because Octopress is based on Jekyll, it uses the [liquid template language](https://jekyllrb.com/docs/templates/) for posts. Hexo uses a completely different one. This theme only styles a Hexo blog to look like Octopress - it won't migrate your posts for you. To do that, you'll need to use something like [hexo-migrator-octopress](https://www.npmjs.com/package/hexo-migrator-octopress)

### Tags and categories

Hexo uses tags where Octopress uses categories. Hexo does have 'categories', but they are hierarchical: a page with categories `[cooking, french]` will be understood as belonging to `category: cooking / subcategory: french cooking`).

## Customising the theme:

Change the way your blog works by editing your `/themes/octo/_config.yml` file:

```yaml
# Page language (html attribute)
language: en

# Main menu navigation items
menu:
  Blog: /
  About: /about
  Archives: /archives

# Post social sharing features (only twitter at present)
social:
  twitter: yournamehere # set to your twitter handle | false to disable

# Page sidebars
# Components will appear in the order they are specified
sidebars:
  recent: true # boolean to display 10 most recent posts
  featured: false # boolean to list all posts with tag 'featured'
  github: jbreckmckye # list Github repositories | false to disable

# Link to atom.xml in nav bar?
# Use https://github.com/hexojs/hexo-generator-feed to generate these
atom: true

# Stylesheets loaded in the <head>
stylesheets:

# Scripts loaded at the end of the body
scripts:

```

## What works?
- blockquotes
- code blocks
- images (left / right / center)
- gists
- headings
- pullquotes (left, right [= default])
- jsfiddle embeds
- youtube videos


## Favicon
- this theme will use your source/images/favicon.png image as the tab / shortcut icon

## Still to do
- analytics
- disqus
- post pagination
