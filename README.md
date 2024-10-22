# Hugo CV Theme

Theme for create minimalistic multilingual CV site.

## Live Demo

See a live demo @ [levn.me](https://levn.me/)

## Quick Start

For fresh Hugo site:

1. Install Hugo and theme
```bash
$ hugo new site mycv
$ cd mycv
$ git init
$ git submodule add https://github.com/nemirlev/hugo-cv-theme themes/hugo-cv-theme

2. Configure your hugo.toml. See `Configuration` below.
3. Build your site with `hugo server` and see the result at http://localhost:1313/.

Or you can use example site from this repo:

```bash
git clone https://github.com/nemirlev/hugo-cv-site.git
cd hugo-cv-site
hugo server
```

and see the result at http://localhost:1313/.

## Configuration

```yml
baseURL: 'https://levn.me/'
languageCode: 'en'
title: 'Personal Site of Lev Nemirovskii'
theme: 'hugo-cv-theme'

# Language support
defaultContentLanguage: ru
defaultContentLanguageInSubdir: true
languages:
   en:
      languageName: EN
      languageDirection: ltr
      languageCode: en-US
      title: 'Personal Site of Lev Nemirovskii'
      weight: 1
   ru:
      languageCode: ru-RU
      languageDirection: 'ltr'
      languageName: 'RU'
      title: 'Персональный сайт Льва Немировского'
      weight: 2
   zh:
      languageCode: zh-CN
      languageDirection: ltr
      languageName: CN
      title: '个人网站 Lev Nemirovskii'
      weight: 3
```

## Content types

For articles use `post` archetype:

```bash
hugo new article/my-new-article.md
```

For events use `event` archetype:

```bash
hugo new events/my-new-event.md
```

For publications use `publication` archetype:

```bash
hugo new publications/my-new-publication.md
```

In publication video and presentation fields are optional.

CV see example in `data/experience/en.yml`. For using CV you need to copy files with you language code.

## License

Theme is released under the MIT License. Check the [original theme license](LICENSE) for additional licensing information.