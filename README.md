This is a project to run angular-seo (https://github.com/steeve/angular-seo) on heroku.

Angular SEO allows you to do server side rendering of angular applications.

To run.

create a cedar stack with phantomjs

modify procfile to point to the path you want to seo optimize.
git commit -am "changes"
heroku create
git push heroku master

I found I needed to set the following variables as well:

heroku config:add BUILDPACK_URL=http://github.com/stomita/heroku-buildpack-phantomjs.git
heroku config:set PATH="/usr/local/bin:/usr/bin:/bin:/app/vendor/phantomjs/bin"
