---
permalink: /
title: Introduction
---
This is the template used for the [Jekyll](http://jekyllrb.com/)-based [18F
Guides](http://pages.18f.gov/guides/), derived from
[CFPB/DOCter](https://github.com/CFPB/DOCter). It's structured to act as an
18F Guides Guide. The repository for this template is
[18F/guides-template](https://github.com/18F/guides-template/).

## Creating a guide

To create a brand new guide, first follow the instructions in the
[README.md](https://github.com/18F/guides-template/blob/18f-pages/README.md)
file of this guide's GitHub repository to create a local clone of this
template.

Once you've created a new clone, click the _Adding a New Page_ entry in the
table of contents.

## Updating an existing guide

Add the [`guides_style_18f` gem](https://github.com/18F/guides-style) to your
Guide's `Gemfile` if it's not already present. You may also wish to copy the
`./go` script from the template if your guide doesn't already have one.

To receive layout updates, as well as any new styles or scripts associated
with them, you will need to run `./go update_theme`. (Or, if you aren't using
a `./go` script, you can run `bundle update --source guides_style_18f`
manually.)

If your repository already has a `gh-pages` branch, you can create an
`18f-pages` branch from it by running these commands:

```
$ git checkout -b 18f-pages gh-pages
$ git push origin 18f-pages
```

Follow the instructions in _Updating the Config File_ to update your
`_config.yml` accordingly. You may also need to consult the _GitHub Setup_ and
_Post Your Guide_ chapters to ensure your guide is correctly published to
`pages.18f.gov` and linked from the main [18F
Guides](http://pages.18f.gov/guides/) site.
