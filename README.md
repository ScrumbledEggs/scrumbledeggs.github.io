# scrumbledeggs.github.io

The website for the _BoardBot_ project for the Fall 2017 [Principles of Engineering](http://poe.olin.edu/) course at [Olin College of Engineering](http://www.olin.edu/).

Built with [Jekyll](https://jekyllrb.com/), [HTML5UP](https://html5up.net/), and [@andrewbanchich](https://github.com/andrewbanchich)'s [WIP Jekyll-ified "Editorial" theme](https://github.com/andrewbanchich/editorial-jekyll-theme).

## Building for poe.olin.edu/2017/boardbot/
The site is currently hosted in two places - GitHub Pages (scrumbledeggs.github.io/) and an Olin server (poe.olin.edu/2017/boardbot/). The settings in [`_config.yml`](_config.yml) are for building for GitHub Pages. In order to build the site correctly for deployment to the olin server, you'll need to change the `url`, `baseurl`, and `google_analytics` variables, which can be done by building the site with [`_linwebprod_config.yml`](_linwebprod_config.yml), as explained in [the Jekyll documentation](https://jekyllrb.com/docs/configuration/):
```shell
jekyll build --config _config.yml,_linwebprod_config.yml
```
