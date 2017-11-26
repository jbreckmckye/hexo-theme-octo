# hexo-theme-octo

## What is this?

A Hexo-theme based on the 'classic' theme for Octopress 2.

Read the Hexo theme [installation instructions](https://github.com/hexojs/hexo/wiki/Themes#install).

## Notes for Octopress users

### This theme won't make Hexo understand Octopress markup

Hexo and Octopress use completely different markup languages for posts and pages. This theme won't solve this problem for you - it just makes your Hexo blog look like Octopress. To migrate your posts, try using [hexo-migrator-octopress](https://www.npmjs.com/package/hexo-migrator-octopress).

### Writing in Hexo

You can use all the same great Octopress tags in your new Hexo blog:

```markdown
# Heading

## Subheading

### Subsubheading
Welcome to [Hexo](https://hexo.io/)!

<!-- more -->
## Pullquotes

My super pullquote. Pullquotes are right-aligned by default:

{% pullquote left %}
Left-hand pullquote
{% endpullquote %}

This right pullquote turns all the heads.

{% pullquote right %}
Right-hand pullquote
{% endpullquote %}

## Images

{% img class_names /path/to/image the_width the_height  [the_title [alt text]] %}

## JSFiddle embeds

{% jsfiddle my_fiddle_id html,css,result dark %}

The syntax is: jsfiddle ID, tab list, and theme ('dark' or 'light').

## Iframes

{% iframe http://my.smashing.url %}

## Github Gists

{% gist gist_id filename %}

## YouTube embeds

{% youtube video_id %}
```

### Tags and categories

Hexo uses tags where Octopress uses categories. Hexo does have 'categories', but they are hierarchical: a page with categories `[cooking, french]` will be understood as belonging to `category: cooking / subcategory: french cooking`.

## Theme options:

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

## Favicon
- this theme will use your source/images/favicon.png image as the tab / shortcut icon

## Still to do
- analytics
- disqus
- post pagination
