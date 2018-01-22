# skeletal
Skeletal theme for Hugo providing a minimalist experience using a trimmed down Bootstrap framework.

* [Hugo](https://gohugo.io/) v0.33
* [Bootstrap](https://getbootstrap.com/) v4.0.0
* [Font Awesome](http://fontawesome.io/) v4.7.0

#### There is no index.html file in this theme!
Skeletal renders a list on its home page by design. See Hugo's [documentation](https://gohugo.io/templates/homepage/).

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
pygmentsStyle:      "trac"
params:
  Subtitle:       "my blog subtitle"
  Description:    "blog description"
  AuthorName:     "Author Name"
  CopyrightSince: "2016"
```

Only content with type as **post** is listed on the list page and in the RSS feed. List pages for a particular taxonomy
classification are indicated as follows (example for tags): `Posts with tag "example"`. Individual page posts display
tag lists if set.

Menu items in footer are generated from content with the following post matter:

``` yaml
menu: main
```
