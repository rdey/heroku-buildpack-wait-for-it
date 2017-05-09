# Heroku buildpack: wait-for-it.sh

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) that installs a small tool for waiting on TCP ports to become available.

The tool itself is available at [vishnubob/wait-for-it](https://github.com/vishnubob/wait-for-it).

## Usage

You need to add this buildpack to your list of buildpacks:

```console
$ heroku buildpacks:add https://github.com/heroku/heroku-buildpack-addon-wait.git
```

Then you can use `bin/wait-for-it.sh` in your post-deploy scripts (see [here for details](https://devcenter.heroku.com/articles/setting-up-apps-using-the-heroku-platform-api#post-deployment-scripts)).
