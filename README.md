# Symmetry Jobs Site

This project is based on hugo with the axiom theme. It is cloned from the [axiom example project](github.com/marketempower/axiom-example). There are good docs available at https://axiomtheme.com/docs as well as on https://gohugo.io

## Content Creation

> NOTE: This repo uses a git submodule for the axiom theme.

run `git clone --recurse-submodules git@github.com:symmetryinvestments/jobs-website`.

or do a manual `git submodule update --init --recursive` after a regular clone.

### Setup

Make sure you have installed hugo, then run `hugo server --disableFastRender` in a terminal and open the local dev website in your browser. Any changes you make are reflected in your browser window.

> NOTE: sometimes not all changes are updated, just kill the dev server and start a fresh one.

### Writing

Just create markdown files in `content/posts`. Other pages are available as .md files in the content folder as well.

## Customizations

### Markup

Since the original axiom theme is included as a submodule we won't be able to edit those files directly. Instead we copy them into the `layouts` folder and edit them there. Hugo will favor them over the ones from the theme.

### Style

Axiom uses the tailwindcss framework. This requires a post process step so you will need to install `npm` and run `npm install` and `npm run watch` in a terminal as well. In development it will produce a large css file, but for the production it will generate a minimized file.

Axiom also uses some class selectors and they can be overwritten by using the `src/custom.css`.

### Switching Themes

Some things have to be modified to switch to another theme. The content files do stay the same.

## Production build

Run `npm run assets:prd` and `npm run hugo:prd`. The website can be found in the `public` folder.

# Original README.md

# Axiom - Example Project

Axiom is designed to make the readers of your content and the search engines happy. Designed with a modular structure, and fully customizable in every way, Axiom adapts to your project, instead of forcing an opinionated structure.

🙌 Follow [Axiom](https://twitter.com/intent/follow?screen_name=axiomtheme) on Twitter to stay up-to-date with the latest news.

## Getting Started

To learn more, see the Quick Start, Documentation, and Live Example resources below:

- Axiom Resources:
  - [Quick Start](https://www.axiomtheme.com/docs/quick-start/)
  - [Documentation](https://www.axiomtheme.com/docs/)
  - [Live Example](https://axiom-example.netlify.app/)
- Axiom Repositories:
  - [Axiom Theme](https://github.com/marketempower/axiom)
  - [Axiom Example](https://github.com/marketempower/axiom-example)

![Axiom Screenshot](https://github.com/marketempower/axiom/raw/master/images/example.png)

# License

Creative Commons Attribution-ShareAlike 4.0 International License: [CC-BY-SA-4.0](https://github.com/marketempower/axiom-example/blob/master/LICENSE).

Copyright 2020 [Jhaura Wachsman](https://www.jhaurawachsman.com/)
