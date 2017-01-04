# TEST TEST TEST

## This is nothing but a test heroku php dyno plugged to my github repo
using composer for php dependencies and publishing my index.php in the public dir
Procfile is configured using 1 single (free) nginx dyno

### How-to deploy that ?
``` bash
git add .
git commit -am "A relevant description"
git push -u origin master
heroku logs --tail
```

### Heroku CLI vs Github
Pushing on github master branch triggers deploying on heroku

``` bash
git remote -v
```
currently lists heroku git and that github
both branches live separatly (need to push or 1 or the other) but a heroku deploy is triggered when anything is pushed in any of these

#### Sources
- https://devcenter.heroku.com/articles/deploying-php
- https://devcenter.heroku.com/articles/php-support#selecting-a-runtime
- https://help.github.com/articles/caching-your-github-password-in-git/#platform-linux
