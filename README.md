Heroku buildpack: Nanoc with Nginx
==================================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpack)
for Nanoc with Nginx.

Usage
-----

```
heroku buildpacks:clear
heroku buildpacks:add heroku/ruby
heroku buildpacks:add https://github.com/anthonymoralez/heroku-buildpack-nanoc
```
Assumes you have a Procfile that runs a Rack server to server your content.
Just push your nanoc site containing the nanoc.yml file and the Gemfile to Heroku and you're ready to go.

Credits
-------

The buildpack is based on the Nginx buildpack of essh (https://github.com/essh/heroku-buildpack-nginx) and the Nanoc buildpack of bobthecow (https://github.com/bobthecow/heroku-buildpack-nanoc).
