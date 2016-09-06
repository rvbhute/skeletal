# skeletal
Skeletal theme for Hugo based on the Skeleton CSS Framework providing a minimalist experience.

* [Hugo](https://gohugo.io/) v0.16
* [Skeleton](http://getskeleton.com/) v2.0.4

This theme looks for the following variables in your Hugo config:

``` yaml
languageCode:    "en-us"
title:           "My Hugo Blog"
params:
  Subtitle:       "my blog subtitle"
  Description:    "blog description"
  AuthorName:     "Author Name"
  CopyrightSince: "2016"
pygmentsuseclasses: false
pygmentscodefences: true
```
Content with type as  "post" is listed on the index and list pages. List pages for a particular taxonomy classification
are indicated as follows (example for tags): `Posts with tag "TAG"`. Only tag lists are being displayed and that too, on
the post page only.

Menu items are generated from content with the following post matter:

``` yaml
type: page
menu: main
```
