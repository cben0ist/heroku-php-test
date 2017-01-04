# TEST TEST TEST

## This is nothing but a test heroku php dyno plugged to my github repo
using composer for php dependencies and publishing my index.php in the public dir
Procfile is configured using 1 single (free) nginx dyno

### How-to deploy that ?
``` bash
git add .
git commit -am "welcome home"
git push -u origin master
heroku logs --tail
```

### Heroku CLI vs Github
Pushing on github master branch triggers deploying on heroku

``` bash
git remote -v
```
currently lists heroku git and that github

#### Sources
- https://devcenter.heroku.com/articles/deploying-php
- https://devcenter.heroku.com/articles/php-support#selecting-a-runtime