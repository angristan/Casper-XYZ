# Casper-XYZ

This is the [Ghost](https://github.com/tryghost/ghost/) theme of [angristan.xyz](https://angristan.xyz), based on [Casper](https://github.com/TryGhost/Casper).

I talked about it on my blog:
- [My custom Ghost theme](https://angristan.xyz/2018/02/my-custom-ghost-theme/)
- [Deploying a Ghost theme with GitHub actions](https://angristan.xyz/2020/05/deploy-ghost-theme-github-actions/)

For more information regarding how to use the theme with Ghost, please refer to the [original README](https://github.com/TryGhost/Casper)

Please credit me if you plan on reusing my theme. 🙂

---

I stopped using and maintaining it in may 2020. For the record, here is how it looks:

![screenshot](ghost-casper-xyz-theme.png)

## Fork

I keep my fork [up-to-date](https://github.com/angristan/Casper-XYZ/blob/master/UPDATE.md) with the upstream.

List of the modifications made in this fork:

* [Custom CSS](https://github.com/angristan/Casper-XYZ/blob/master/assets/css/custom.css)
  * Use the Open Sans Pro font
  * Header image is the same width as the content, and the content doesn't step on it
  * Use GitLab-like font for code blocks instead of ugly monospace
  * Disable dark mode
  * Isso (comments) style enhancements
  * A lot more, check the comments!
* [Removed share buttons in the header](https://github.com/angristan/Casper-XYZ/commit/b4530b973a71bcdfce82c02572525171a5fa9159)
* [Replaced Feedly links by original RSS links](https://github.com/angristan/Casper-XYZ/commit/c618bc702969c217b6f48277244b6bf04b4e46bd)
* [Host jQuery locally](https://github.com/angristan/Casper-XYZ/commit/d9105f2667ed7ae8de32a3cd36d1bea8a910f77d)
* [GitHub, Mastodon, Linkedin, Instagram and Shaarli links and SVG icons](https://github.com/angristan/Casper-XYZ/blob/master/partials/site-nav.hbs#L16)
* [Use GitHub Actions for CI instead of Travis (test + deploy)](https://github.com/angristan/Casper-XYZ/tree/master/.github/workflows)
* [Replaced estimated reading time on posts list by the release date](https://github.com/angristan/Casper-XYZ/pull/4)

### Hardcoded stuff

I try to make the theme reusable as possible, but I still have to hardcode some stuff.

* [Isso comments](https://github.com/angristan/Casper-XYZ/blob/master/post.hbs)
* [GitHub, Mastodon, Linkedin, Instagram and Shaarli links](https://github.com/angristan/Casper-XYZ/blob/master/partials/site-nav.hbs)
* [Vultr affiliate link](https://github.com/angristan/Casper-XYZ/blob/master/default.hbs)

**MAKE SURE TO UPDATE/REMOVE THEM IF YOU PLAN ON REUSING MY THEME!**

### External assets embedded

Here are the assets that I downloaded and included in the repo as I don't want to make call to 3rd-party services:

* [jQuery](https://github.com/jquery/jquery)
* [Source Sans Pro font from Google Fonts](https://fonts.google.com/specimen/Source+Sans+Pro)

They are all under their respective license.
