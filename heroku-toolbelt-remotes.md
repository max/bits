When you have several Heroku apps set up as remotes (e.g. dev, staging, and prod) you can use remote names instead of app names:

```
heroku info -r dev
heroku config-set FOO=BAR -r prod
```
