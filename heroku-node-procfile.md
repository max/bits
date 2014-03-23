You don't need a `Procfile` for simple Node.js apps on Heroku. Simply add a `start` script to your `package.json`:

```json
{
  scripts: {
    start: 'node index.js'
  }
}
```

This will work locally too: `npm start`.

If you would like to run with a slightly different setup in development (e.g. using nodemon to automatically restart your server on changes) try this:

```json
{
  scripts: {
    dev: 'nodemon index.js',
    start: 'node index.js'
  }
}
```

Note that `npm start` is a shortcut for `npm run start` which doesn't exist for keys so for your `dev` task you will have to run `npm run dev`.
