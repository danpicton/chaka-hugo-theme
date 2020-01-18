# Chaka

Minimalistic and Responsive blog theme for hugo, forked from [natarajmb/charaka-hugo-theme](https://github.com/natarajmb/charaka-hugo-theme). Removes highlight.js syntax highlighting, adds custom notice shortcode for info boxes. 

Image from original charaka project:
 
![](https://github.com/natarajmb/charaka-hugo-theme/blob/master/images/screenshot.png)

## Getting Started

All instructions to be undertaken from root folder of site.

Clone this repository to your hugo theme directory.

```
mkdir themes
cd themes
git clone https://github.com/danpicton/chaka-hugo-theme chaka
```

If you use git to version control your site, highly recommended, it's best to add the chaka theme as a submodule.

```
mkdir themes
cd themes
git submodule add https://github.com/danpicton/chaka-hugo-theme chaka
````

## Updating

```
git submodule update --remote --merge
```

## Configuration

Take a look in the [exampleSite](https://github.com/natarajmb/charaka-hugo-theme/tree/master/exampleSite) folder.

This directory contains an example config file and the content for the demo.
It serves as an example setup for your documentation.

Copy the `config.toml` in the root directory of your website. Overwrite the existing config file if necessary.

__[config.toml](https://github.com/natarajmb/charaka-hugo-theme/blob/master/exampleSite/config.toml)__:

```toml
baseurl = "https://example.com"
languageCode = "en"
title = "Charaka"
theme = "charaka-hugo-theme"
copyright = "&copy; <a href=\"https://github.com/natarajmb\">Nataraj Basappa</a> 2018"
disqusShortname = ""
googleAnalytics = ""

[params]

[params.highlight]
  style = "zenburn"

[[params.social]]
  url = "about.html"
  fa_icon = "fas fa-info" 

[[params.social]]
  url = "https://github.com/natarajmb"
  fa_icon = "fab fa-github"

[[params.social]]
  url = "https://www.linkedin.com/in/natarajmb/"
  fa_icon = "fab fa-linkedin-in"

[[params.social]]
  url = "https://twitter.com/natarajmb"
  fa_icon = "fab fa-twitter"
```

## Front matter parameters
Worth mentioning are:
|hidden|"true"/"false"|Hides page from site index list and search engine crawlers|
|index|"true"/"false"|Indexes page for search engine crawlers|
|showthedate|"true"/"false"|Displays the creation date of a page (defaults to true)|

## Build

```
hugo server
```

You can go to localhost:1313 and this theme should be visible.

## Inspirations
- [Hemingway](https://themes.gohugo.io/hemingway/)
- [Journal](https://themes.gohugo.io/hugo-journal/)
- Apple iBooks colour scheme

## How to tweak
- Once you have activited the theme as above and running hugo in server mode
- Install [npm](https://www.npmjs.com/get-npm)
- Get inside checked-out theme directory and run `npm install`
- Make required changes to style.scss and run `npm run css-build && npm run css-watch` to live update your changes

## License

Charaka is licensed under the [MIT License](LICENSE.md).

## Author

[Nataraj Basappa](https://github.com/natarajmb)
[Dan Picton](https://github.com/danpicton)
