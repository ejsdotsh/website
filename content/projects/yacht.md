---
title: "YACHT Another Custom Hugo Theme"
draft: false
# image: //via.placeholder.com/640x150
alt_text: "YACHT Another Custom Hugo Theme"
summary: "YACHT Another Custom Hugo Theme"
status: "active"
tech_used:
  - SCSS
  - HTML
---

when graduating from high school, i was voted *"most likely to own a yacht"* by my senior class. i don't think this is
what they meant...

***YACHT** **A**nother **C**ustom **H**ugo **T**heme*

## what is YACHT

***YACHT*** is a punny and recursively named theme for the [Hugo][1] static site generator which uses the [Catppuccin
Palettes][2] and aims to be simple, mobile-first, accessible, responsive, and to have minimal external dependencies.

***under construction***

## getting your own YACHT

after it's been constructed, the preferred way of getting your own **YACHT** is by using `Hugo modules`

in `config.toml`:

```toml
[module]
[[module.imports]]
path = "github.com/ejsdotsh/yacht-hugo-theme"
```

or in `config.yaml`:

```yaml
module:
  imports:
    path: "github.com/ejsdotsh/yacht-hugo-theme"
    disable: false
```

then run:

```txt
hugo mod get -u ./...
```

## references and inspiration

- [Catppuccin](https://github.com/catppuccin/catppuccin)
- Brian P. Hogan's [Build Websites with Hugo](https://pragprog.com/titles/bhhugo/build-websites-with-hugo)
- [Every Layout](https://every-layout.dev/)
- [Andy Bell's](https://github.com/Andy-set-studio/personal-site-eleventy) personal site
- CUBECSS [blog](https://piccalil.li/blog/cube-css/) post
- [CUBECSS](https://cube.fyi/)
- Lorenze Setale's [My Hugo blog now is fast and light](https://blog.setale.me/2022/01/31/My-Hugo-blog-now-is-fast-and-light/)

[1]: <https://gohugo.io> "Hugo"
[2]: <https://github.com/catppuccin/palette> "Catppuccin Palettes"
