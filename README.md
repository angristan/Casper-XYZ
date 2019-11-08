# Casper

<<<<<<< HEAD
[![pipeline status](https://gitlab.com/angristan/Casper-XYZ/badges/master/pipeline.svg)](https://gitlab.com/angristan/Casper-XYZ/pipelines)
=======
The default theme for [Ghost](http://github.com/tryghost/ghost/). This is the latest development version of Casper! If you're just looking to download the latest release, head over to the [releases](https://github.com/TryGhost/Casper/releases) page.
>>>>>>> upstream/master

This is the [Ghost](https://github.com/tryghost/ghost/) theme of [angristan.xyz](https://angristan.xyz), based on [Casper](https://github.com/TryGhost/Casper).

<<<<<<< HEAD
For more information regarding how to use the theme with Ghost, please refer to the [original README](https://github.com/TryGhost/Casper)
=======
![screenshot-desktop](https://user-images.githubusercontent.com/353959/66987533-40eae100-f0c1-11e9-822e-cbaf38fb8e3f.png)
>>>>>>> upstream/master

## Fork

I keep my fork up-to-date with the upstream.

List of the modifications made in this fork:

<<<<<<< HEAD
* [Custom CSS (lots of stuff, commented)](https://github.com/Angristan/Casper-XYZ/blob/master/assets/css/custom.css)
* [Removed share buttons in the header](https://github.com/Angristan/Casper-XYZ/commit/b4530b973a71bcdfce82c02572525171a5fa9159)
* [Replaced Feedly links by original RSS links](https://github.com/Angristan/Casper-XYZ/commit/c618bc702969c217b6f48277244b6bf04b4e46bd)
* [Added Isso for comments](https://github.com/Angristan/Casper-XYZ/blob/master/post.hbs#L71)
* [Host jQuery locally](https://github.com/Angristan/Casper-XYZ/commit/50b425d7c1a370bd44d599d597b25623f8c8936b)
* [Use the Open Sans Pro font](https://github.com/Angristan/Casper-XYZ/blob/master/assets/css/custom.css#L1)
* [Header image is the same width as the content, and the content doesn't step on it](https://github.com/Angristan/Casper-XYZ/commit/1c0fd7d699651d7413028d130f59e20dbcab498e)
* [GitHub, Mastodon, Linkedin, Instagram and Shaarli links and SVG icons](https://github.com/Angristan/Casper-XYZ/blob/master/partials/site-nav.hbs#L16)
* Added [GitLab CI](https://gitlab.com/angristan/Casper-XYZ/pipelines)
* [Use GitLab-like font for code blocks instead of ugly monospace](https://github.com/angristan/Casper-XYZ/blob/master/assets/css/custom.css#L163)
* [Replaced estimated reading time on posts list by the release date](https://github.com/angristan/Casper-XYZ/pull/4)
* [Backported AMP template to theme for customisation (Google Analytics and Matomo)](https://github.com/angristan/Casper-XYZ/blob/master/amp.hbs)
=======
This theme has lots of code comments to help explain what's going on just by reading the code. Once you feel comfortable with how everything works, we also have full [theme API documentation](https://ghost.org/docs/api/handlebars-themes/) which explains every possible Handlebars helper and template.
>>>>>>> upstream/master

### Hardcoded stuff

<<<<<<< HEAD
I try to make the theme reusable as possible, but I still have to hardcode some stuff.

* [Isso comments block](https://github.com/Angristan/Casper-XYZ/blob/master/post.hbs#L71)
* [GitHub, Mastodon, Linkedin, Instagram and Shaarli links](https://github.com/Angristan/Casper-XYZ/blob/master/partials/site-nav.hbs#L16)
* [Vultr affiliate link](https://github.com/angristan/Casper-XYZ/blob/master/default.hbs#L32)

### External assets embedded
=======
- `default.hbs` - The parent template file, which includes your global header/footer
- `index.hbs` - The main template to generate a list of posts, usually the home page
- `post.hbs` - The template used to render individual posts
- `page.hbs` - Used for individual pages
- `tag.hbs` - Used for tag archives, eg. "all posts tagged with `news`"
- `author.hbs` - Used for author archives, eg. "all posts written by Jamie"

One neat trick is that you can also create custom one-off templates by adding the slug of a page to a template file. For example:

- `page-about.hbs` - Custom template for an `/about/` page
- `tag-news.hbs` - Custom template for `/tag/news/` archive
- `author-ali.hbs` - Custom template for `/author/ali/` archive
>>>>>>> upstream/master

Here are the assets that I downloaded and included in the repo as I don't want to make call to 3rd-party services:

* [jQuery](https://github.com/jquery/jquery)
* [Source Sans Pro font from Google Fonts](https://fonts.google.com/specimen/Source+Sans+Pro)

<<<<<<< HEAD
They are all under their respective licence.
=======
Casper styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
# install dependencies
yarn install

# run development server
yarn dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

```bash
# create .zip file
yarn zip
```

# PostCSS Features Used

- Autoprefixer - Don't worry about writing browser prefixes of any kind, it's all done automatically with support for the latest 2 major versions of every browser.
- Variables - Simple pure CSS variables
- [Color Function](https://github.com/postcss/postcss-color-function)


# SVG Icons

Casper uses inline SVG icons, included via Handlebars partials. You can find all icons inside `/partials/icons`. To use an icon just include the name of the relevant file, eg. To include the SVG icon in `/partials/icons/rss.hbs` - use `{{> "icons/rss"}}`.

You can add your own SVG icons in the same manner.


# Copyright & License

Copyright (c) 2013-2019 Ghost Foundation - Released under the [MIT license](LICENSE).
>>>>>>> upstream/master
