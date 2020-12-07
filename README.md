# Pre-reqs

- [Bundler](https://bundler.io/)

```shell
$ bundle install
```

# Running Locally

```shell
$ bundle exec jekyll serve
```

# Publishing

1. Run locally and validate site works locally (see above.)

2. Commit and push your changes to the `site` repository. For example:

   ```shell
   git add .
   git commit -m "<describe your change>"
   git push
   ```

3. Build the site.

   ```shell
   bundle exec jekyll build
   ```

4. Push the changes from `_site` directory to the `hanriver.github.io` repository (see below.)

## Pushing changes to production (step 4)

1. If you haven't already, clone the `hanriver.github.io` repository next to the `site` repository.

2. Make sure it's up-to-date by running `git pull` in the `hanriver.github.io/` directory.

3. Copy the files from the `site/_site` directory to the `hanriver.github.io/` directory. For example:

   ```shell
   $ cp -r ./_site/ ../hanriver.github.io/
   ```

4. Publish changes by commiting it and pushing the changes in the `hanriver.github.io/` directory:

   ```shell
   $ cd ../hanriver.github.io/
   $ git add .
   $ git commit -m "<describe your change>"
   $ git push
   ```
