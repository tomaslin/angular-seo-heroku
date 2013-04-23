This is a project to run angular-seo (https://github.com/steeve/angular-seo) on heroku.

Angular SEO allows you to do server side rendering of angular applications.

To run.

create a cedar stack with phantomjs

heroku create --stack cedar --buildpack http://github.com/stomita/heroku-buildpack-phantomjs.git

modify procfile to point to the path you want to seo optimize.
