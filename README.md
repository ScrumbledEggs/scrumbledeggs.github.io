# scrumbledeggs.github.io

The website for the _BoardBot_ project for the Fall 2017 [Principles of Engineering](http://poe.olin.edu/) course at [Olin College of Engineering](http://www.olin.edu/).

Built with [Jekyll](https://jekyllrb.com/), [HTML5UP](https://html5up.net/), and [@andrewbanchich](https://github.com/andrewbanchich)'s [WIP Jekyll-ified "Editorial" theme](https://github.com/andrewbanchich/editorial-jekyll-theme).

## Building for poe.olin.edu/2017/boardbot/
The site is currently hosted in two places - GitHub Pages (scrumbledeggs.github.io/) and an Olin server (poe.olin.edu/2017/boardbot/). The settings in [`_config.yml`](_config.yml) are for building for GitHub Pages. In order to build the site correctly for deployment to the olin server, you'll need to change the `url`, `baseurl`, and `google_analytics` variables, which can be done by building the site with [`_linwebprod_config.yml`](_linwebprod_config.yml), as explained in [the Jekyll documentation](https://jekyllrb.com/docs/configuration/):
```shell
jekyll build --config _config.yml,_linwebprod_config.yml
```

Original README from HTML5 UP:

```
Editorial by HTML5 UP
html5up.net | @ajlkn
Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)


Say hello to Editorial, a blog/magazine-ish template built around a toggleable "locking"
sidebar (scroll down to see what I mean) and an accordion-style menu. Not the usual landing
page/portfolio affair you'd expect to see at HTML5 UP, but I figured for my 41st (!!!)
template I'd change it up a little. Enjoy :)

Demo images* courtesy of Unsplash, a radtastic collection of CC0 (public domain) images
you can use for pretty much whatever.

(* = not included)

AJ
aj@lkn.io | @ajlkn


Credits:

	Demo Images:
		Unsplash (unsplash.com)

	Icons:
		Font Awesome (fortawesome.github.com/Font-Awesome)

	Other:
		jQuery (jquery.com)
		html5shiv.js (@afarkas @jdalton @jon_neal @rem)
		Misc. Sass functions (@HugoGiraudel)
		Respond.js (j.mp/respondjs)
		Skel (skel.io)
```
