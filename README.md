# @mattdesl/ghpages

[![experimental](http://badges.github.io/stability-badges/dist/experimental.svg)](http://github.com/badges/stability-badges)

A small, personalized shell script which switches to `gh-pages` branch, runs `npm run build`, commits and pushes the new changes, and then switches back to your previous branch.

## Install

```sh
npm install @mattdesl/ghpages -g
```

## Usage

In a module folder with `npm run build` script, and with a clean working directory on your default branch (i.e. `master`), simply run the following:

```sh
ghpages
```

## License

MIT, see [LICENSE.md](http://github.com/mattdesl/ghpages/blob/master/LICENSE.md) for details.
