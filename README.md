# hexo-theme-octo

## What is this?

A Hexo theme based on the 'classic' theme for Octopress 2.

To install, clone this repository into a Hexo `themes/octo` folder and change `theme` in `_config.yml` to "octo".

When updating, remember not to overwrite your theme config.yml.

## Notes for Octopress users

### Migrating from Octopress

Octopress and Hexo use the same post markup language, so moving from one blog to the other is actually rather straightforward. See https://hexo.io/docs/migration.html#Octopress

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

## Codeblocks
{% codeblock %}
    beep.beep(thisIsMyCode).beep();
{% endcodeblock %}

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
  Archives: /archives
  # Title: /pageName - create using `hexo new page 'pageName'`

# Post social sharing features
social:
  twitter: your_twitter # set to your twitter handle

# Page sidebars
# Components will appear in the order they are specified
sidebars:
  recent: true # boolean to display 10 most recent posts
  featured: false # boolean to list all posts with tag 'featured'
  github: your_github # string to point to a Github profile | false to disable

# Disqus comments
disqus:
  enabled: false
  shortname: your_website_shortname

# Analytics
googleAnalytics: false # false | string (UA-xxxx ID)

# Link to atom.xml in nav bar?
# You can use https://github.com/hexojs/hexo-generator-feed to generate these
atom: true

# Stylesheets loaded in the <head>
stylesheets:

# Scripts loaded at the end of the body
scripts:
```

## Favicon
This theme will use your `source/images/favicon.png` image as a favicon.

## Limitations
This theme doesn't currently support image galleries. Let me know if you need it.
