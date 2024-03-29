# UI Suite Bootstrap Demo

## Summary

A demo site for [pdureau/ui\_suite\_bootstrap](https://github.com/pdureau/ui_suite_bootstrap) theme.

With a focus on those example pages:

- [https://getbootstrap.com/docs/4.5/examples/album/](https://getbootstrap.com/docs/4.5/examples/album/)
- [https://getbootstrap.com/docs/4.5/examples/pricing/](https://getbootstrap.com/docs/4.5/examples/pricing/)
- [https://getbootstrap.com/docs/4.5/examples/carousel/](https://getbootstrap.com/docs/4.5/examples/carousel/)


## Installation

On your system, you need [git](https://git-scm.com/), [composer](https://getcomposer.org/), [sqlite](https://www.sqlite.org) installed.

Then:

```
$ composer create-project drupal/recommended-project ui_suite_bootstrap_demo
$ cd ui_suite_bootstrap_demo
```


## Config & site building

There are many ways to build those examples pages in Drupal. For example, a card wall can be an entity reference formatter, or a view style. A button can be an entity reference formatter or a link formatter. A grid can be a view style or a layout. etc.

Here is what we did in this demo:

Album:

- Mainly based on entity reference fields.
- Full page display: /admin/structure/types/manage/album/display
- Cards display: /admin/structure/media/manage/image/display/card
- Cards image style: /admin/config/media/image-styles/manage/card

Carousel:

- A mix beween entity reference fields and inline blocks in layout.
- Full page display: /admin/structure/types/manage/carousel/display
- Marketing: /admin/structure/block/block-content/manage/marketing
- Slide image style: /admin/config/media/image-styles/manage/slide
- Marketing image style: /admin/config/media/image-styles/manage/marketing
- Featurette: /admin/structure/block/block-content/manage/featurette
- Featurette image style: /admin/config/media/image-styles/manage/featurette

Pricing:

- Mainly based on a views query and the ability of overriding layout by content (for the first package button).
- Full page display: /admin/structure/types/manage/pricing/display
- Package: /admin/structure/block/block-content/manage/package/display
- Packages: /admin/structure/views/view/packages

## Default content

Some example content is automatically imported during the installation:

- An album page: /node/1
- A carousel page: /node/2
- A pricing page: /node/3


