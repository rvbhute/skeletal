# skeletal
Skeletal theme for Hugo providing a minimalist experience using a trimmed down Bootstrap framework.

* [Hugo](https://gohugo.io/) v0.18
* [Bootstrap](https://getbootstrap.com/) v3.3.7

#### There is no index.html file in this theme!
Skeletal renders a list on its home page by design. I found the `index.html` converging on `_default\list.html`, hence
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
languageCode:       "en-us"
title:              "My Hugo Blog"
pygmentsUseClasses: false
pygmentsCodeFences: true
pygmentsStyle: "trac"
params:
  Subtitle:       "my blog subtitle"
  Description:    "blog description"
  AuthorName:     "Author Name"
  CopyrightSince: "2016"
```

`pygments` settings are required for correct styling of code blocks. It uses the trac theme for code styling.

Only content with type as "post" is listed on the list page. List pages for a particular taxonomy classification are
indicated as follows (example for tags): `Posts with tag "example"`. Only tag lists are being displayed and that too, on
the post page only.

Menu items in footer are generated from content with the following post matter:

``` yaml
menu: main
```
