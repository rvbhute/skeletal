# skeletal
Skeletal theme for Hugo based on the Skeleton CSS Framework providing a minimalist experience.

* [Hugo](https://gohugo.io/) v0.16
* [Skeleton](http://getskeleton.com/) v2.0.4

#### There is no index.html file in this theme!
Skeletal renders a list on its home page by desgin. I found the `index.html` converging on `_default\list.html`, hence
I removed the `index.html` file. Hugo's documentation [mentions](https://gohugo.io/templates/homepage/) that:

> Hugo will use the following prioritized list. If a file isn’t present, then the next one in the list will be used

```
... [layouts] ...
/themes/THEME/layouts/index.html
/themes/THEME/layouts/_default/list.html
/themes/THEME/layouts/_default/single.html
```

#### Config Variables
This theme looks for the following variables in your Hugo config:

``` yaml
languageCode:    "en-us"
title:           "My Hugo Blog"
params:
  Subtitle:       "my blog subtitle"
  Description:    "blog description"
  AuthorName:     "Author Name"
  CopyrightSince: "2016"
```

Only content with type as "post" is listed on the list page. List pages for a particular taxonomy classification are
indicated as follows (example for tags): `Posts with tag "TAG"`. Only tag lists are being displayed and that too, on
the post page only.

Menu items are generated from content with the following post matter:

``` yaml
type: page
menu: main
```
