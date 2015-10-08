# @mattdesl/ghpages

[![experimental](http://badges.github.io/stability-badges/dist/experimental.svg)](http://github.com/badges/stability-badges)

A small, personalized shell script which switches to `gh-pages` branch, runs `npm run build`, commits and pushes the new changes, and then switches back to your previous branch.

## Install

```sh
npm install @mattdesl/ghpages -g
```

## Usage

`cd` to your module directory. Make sure it has a `build` script in `package.json`:

```json
{
  "scripts": {
    "build": "browserify index.js > bundle.js"
  }
}
```

If you don't have a `gh-pages`, make sure to create one:

```sh
git branch gh-pages
```


Now, with a clean git working directory, and on the default (i.e. `master`) branch, just run the following to push to gh-pages:

```sh
ghpages
```

This will check out `gh-pages` branch, merge master into it, `npm run build`, then commit and push the new build and switch back to master.

## License

MIT, see [LICENSE.md](http://github.com/mattdesl/ghpages/blob/master/LICENSE.md) for details.
