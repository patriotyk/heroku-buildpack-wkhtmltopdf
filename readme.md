# Heroku Buildpack: wkhtmltopdf

Downloads wkhtmlto* binaries, verifies, then makes them available in the $PATH.

## Tested against following

- wkhtmltopdf 0.12.3

## Usage

```
$ heroku buildpacks:add https://github.com/nexto/heroku-buildpack-wkhtmltopdf

$ heroku config:set WKHTMLTOPDF_URL=http://download.gna.org/wkhtmltopdf/0.12/0.12.3/{wkhtmltox-0.12.3_linux-generic-amd64.tar.xz,SHA1SUMS}

$ git commit --allow-empty
$ git push heroku

$ heroku run wkhtmltopdf -V
$ heroku which wkhtmltopdf

# profit!
```

## Reference

[Heroku Buildpacks](https://devcenter.heroku.com/articles/buildpacks)
