# Pre-reqs

- [Bundler](https://bundler.io/)

```shell
$ bundle install
```

# Running Locally

```shell
$ bundle exec jekyll serve
```

# Publishing to production

1. Run locally and validate site works locally.
2. Commit and push your changes to the `site` repository.
3. Build the site.
4. Push the changes from `_site` directory to the `hanriver.github.io` repository.

## Building the site (step 3)

```shell
$ bundle exec jekyll build
```

## Push changes to production (step 4)

1. If you haven't already, clone the `hanriver.github.io` repository.

2. Make sure it's up-to-date by running `git pull`

3. Copy the files from the `site/_site` directory to the `hanriver.github.io/` directory.

4. Publish changes by commiting it and pushing it.

   ```shell
   $ git add .
   $ git commit
   $ git push
   ```
