## Building

### Building the site

**Prerequisites**

- [Install Ruby](https://www.ruby-lang.org/en/documentation/installation/).
- [Install Bundler](https://bundler.io/).

**Installing packages**

```sh
bundle install
```

**Build once**

```sh
bundle exec jekyll build
```

**Build continuously**

```sh
bundle exec jekyll serve
```

View the site at `localhost:4000/rhcsa-open-guide/` in your browser.

**Verify links**

After building:

```sh
bundle exec htmlproofer --assume-extension ./_site
```

### Linting files

**Prerequisites**

- [Install Node 16](https://nodejs.org/en/download/).
- [Install Yarn v1](https://classic.yarnpkg.com/lang/en/docs/install).

**Installing packages**

```sh
yarn install
```

**Linting**

```sh
yarn lint
```

**Formatting**

```sh
yarn format
```

### Linting prose

**Prerequisites**

- [Install Vale](https://vale.sh/docs/vale-cli/installation/).

**Linting**

```sh
vale .
```
