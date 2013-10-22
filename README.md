heroku-buildpack-sass is a [custom buildpack][1] for [Heroku][2] that compiles
[Sass][3]/SCSS files to CSS.

Unless you're deploying a static site, using no other languages, and serving
with magic(!), you'll probably want to combine this with other buildpacks using
[heroku-buildpack-compose][4] or [heroku-buildpack-multi][5].

This buildpack finds all .scss and .sass files, and compiles them to files
with the extension changed to .css and any parent directories named scss or
sass changed to css. So ./scss/style.scss becomes ./css/style.css.

[1]: https://devcenter.heroku.com/articles/buildpacks#using-a-custom-buildpack
[2]: https://www.heroku.com/
[3]: http://sass-lang.com/
[4]: https://github.com/bwhmather/heroku-buildpack-compose
[5]: https://github.com/ddollar/heroku-buildpack-multi
