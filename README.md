# Images Responsiver

[![Build Status](https://github.com/nhoizey/images-responsiver/workflows/Tests%20CI/badge.svg)](https://github.com/nhoizey/images-responsiver/actions)
[![GitHub stars](https://img.shields.io/github/stars/nhoizey/images-responsiver.svg?style=social)](https://github.com/nhoizey/images-responsiver/stargazers)

Images Responsiver tries to **help developers make it easy for content authors to tackle responsive images needs**.

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Why does this project exist?](#why-does-this-project-exist)
- [One repository, multiple projects](#one-repository-multiple-projects)
  - [A Node.js package to ease responsive images: `images-responsiver`](#a-nodejs-package-to-ease-responsive-images-images-responsiver)
  - [A plugin for Eleventy: `eleventy-plugin-images-responsiver`](#a-plugin-for-eleventy-eleventy-plugin-images-responsiver)
- [Sources and documentations](#sources-and-documentations)
- [Contributing](#contributing)
  - [Contribution guidelines](#contribution-guidelines)
  - [Tools and automations](#tools-and-automations)
- [License](#license)
- [Authors](#authors)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Why does this project exist?

As Steve Jobs [once said](https://www.youtube.com/watch?v=oeqPrUmVz-o):

> You've got to start with the customer experience and run backwards to the technology.

**Responsive images are one of the most difficult topics nowadays** for front end developers and content authors, they involve multiple features and syntaxes, but they are **required to provide a good performance to Web users**.

Most content authors should not have to learn the complex responsive images HTML syntax, how and it is used by browsers to load the right image for current viewing context.

## One repository, multiple projects

Multiple projects are managed inside this shared monorepo.

### A Node.js package to ease responsive images: `images-responsiver`

Images Responsiver transforms plain, simple `<img src="…">` HTML tags into better responsive images syntax with `srcset` and `sizes` attributes.

Knowing that [`<picture>` is only required for rare advanced usages](https://cloudfour.com/thinks/dont-use-picture-most-of-the-time/), **Images Responsiver should be enough for most use cases**, where the need is known as Resolution Switching.

Read [this article on Cloudfour's blog to know more of the theory](https://cloudfour.com/thinks/responsive-images-the-simple-way/).

### A plugin for Eleventy: `eleventy-plugin-images-responsiver`

Images Responsiver is also available as a plugin for [Eleventy](https://www.11ty.dev/), an awesome Static Site Generator.

It allows authors to use the simple and **standard Markdown syntax for images** — `![alt text](image.jpg)` — and yet get responsive images in the generated HTML.

## Sources and documentations

| **package**                          | **source**                                                                                                     | **npm**                                                                 | **docs**                                                                                 |
| ------------------------------------ | -------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `images-responsiver`                 | [source](https://github.com/nhoizey/images-responsiver/tree/main/packages/images-responsiver)                  | [npm](https://www.npmjs.com/package/images-responsiver)                 | [docs](https://nhoizey.github.io/images-responsiver/images-responsiver/)                 |
| `eleventy-plugin-images-responsiver` | [source](https://github.com/nhoizey/images-responsiver/tree/main/packages/eleventy-plugin-images-responsiver/) | [npm](https://www.npmjs.com/package/eleventy-plugin-images-responsiver) | [docs](https://nhoizey.github.io/images-responsiver/eleventy-plugin-images-responsiver/) |

## Contributing

First, thank you for considering contributing to `images-responsiver`! It's people like you that make the open source community such a great community! 😊

### Contribution guidelines

There are many ways to contribute to this project.

[Get started here](https://github.com/nhoizey/images-responsiver/blob/master/CONTRIBUTING.md).

### Tools and automations

- This monorepo is managed with [Lerna](https://lerna.js.org/).
- Tests are run by [jest](https://jestjs.io/) and written in [the `__tests__` folder](https://github.com/nhoizey/images-responsiver/tree/main/packages/images-responsiver/__tests__) for each package.
- Pull Requests are checked with tests run on [GitHub Actions](https://github.com/nhoizey/images-responsiver/actions) (see [configuration](https://github.com/nhoizey/images-responsiver/blob/main/.github/workflows/tests.yml))
- Dependencies updates are automated with [dependabot](https://github.blog/2020-06-01-keep-all-your-packages-up-to-date-with-dependabot/) (see [configuration](https://github.com/nhoizey/images-responsiver/blob/main/.github/dependabot.yml))
- Pull Requests are rebased as necessary, and merged automatically by [Kodiak](https://kodiakhq.com/) if there is an `automerge 🤞` label (set by dependabot for example) and GitHub Actions CI check is OK (see [configuration](https://github.com/nhoizey/images-responsiver/blob/main/.kodiak.toml))
- The documentation is written as Markdown files in [the `docs/` folder](https://github.com/nhoizey/images-responsiver/tree/main/docs), and transformed into HTML by [Jekyll](https://jekyllrb.com/) powered [GitHub Pages](https://pages.github.com/): <https://nhoizey.github.io/images-responsiver/>

## License

This project is licensed under the [MIT License](LICENSE.md).

## Authors

- [Nicolas Hoizey](https://github.com/nhoizey): Idea and initial work, maintainer

See also the list of [contributors](https://github.com/nhoizey/images-responsiver/contributors) who participated in this project.
