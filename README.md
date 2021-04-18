# Template web-page

This web-page project is geared towards an academic audience.

Creation, modification and customization of the template is fairly easy since it powered by [Jekyll](https://jekyllrb.com/) and [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/).

## Prerequisites

### Set up your GitHub repository

1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
2. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right.
3. Rename the repository "[your GitHub username].github.io", which will also be your website's URL.

## Build your site locally

1. Clone the repository

2. Follow the [installation instructions](https://jekyllrb.com/docs/installation/) of [Jekyll](https://jekyllrb.com/) to get

  - Ruby
  - Bundler
  - Jekyll

3. Install the dependencies stored in the `Gemfile` file (`github-pages`, `minimal-mistakes-jekyll`, `jekyll-scholar`)

  ```bash
    cd <your-directory>
    git checkout master
    bundle install
  ```

4. Build and serve your site

```bash
  cd <path-to-your-directory.github.io>
  git checkout master
  bundle exec jekyll serve --livereload
```

Part of the output should look like

```bash
  ...
   Auto-regeneration: enabled for '<path-to-your-directory.github.io>'
  LiveReload address: http://127.0.0.1:35729
      Server address: http://127.0.0.1:4000
    Server running... press ctrl-c to stop.
  ...
```

More specifically,

- `bundle exec` builds the site and outputs `.html` files, stored in the `_site` folder
- `jekyll serve` opens a port to make the site available in a local server, here `http://127.0.0.1:4000`
- `--livereload` automatically refreshes the page according to each change made to the source files

## Modify the content of your site




## Deploy your site

Your site is

One could use,
However, the `jekyll-scholar` plugin used to render bibliography and make citations is incompatible with the GitHub Pages workflow.

Nevertheless, we can still make use of GitHub Pages to
Please consider using
Since we have used the jekyll-scholar plugin we can't

[GitHub gist](https://gist.github.com/cobyism/4730490#gistcomment-3288642)

- Make sure `_site` is not listed in the `.gitignore` file

```bash
  git push origin `git subtree split --prefix _site master`:gh-pages --force
```
