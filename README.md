<p align="right">
  <a href="https://github.com/rbong/rhcsa-open-guide/actions/workflows/pages/pages-build-deployment"><img src="https://github.com/rbong/rhcsa-open-guide/actions/workflows/pages/pages-build-deployment/badge.svg" alt="pages-build-deployment"></a>
  <a href="https://github.com/rbong/rhcsa-open-guide/actions/workflows/verify-html.yml"><img src="https://github.com/rbong/rhcsa-open-guide/actions/workflows/verify-html.yml/badge.svg" alt="verify-html"></a>
  <a href="https://github.com/rbong/rhcsa-open-guide/actions/workflows/lint-files.yml"><img src="https://github.com/rbong/rhcsa-open-guide/actions/workflows/lint-files.yml/badge.svg" alt="lint-files"></a>
  <a href="https://github.com/rbong/rhcsa-open-guide/actions/workflows/lint-prose.yml"><img src="https://github.com/rbong/rhcsa-open-guide/actions/workflows/lint-prose.yml/badge.svg" alt="lint-prose"></a>
</p>

# RHCSA Open Guide

### [Read the guide here](http://rbong.github.io/rhcsa-open-guide)

## Overview

This is an open study guide for becoming a [Red Hat Certified Systems Administrator](https://www.redhat.com/en/services/certification/rhcsa) (RHCSA)
by passing the [EX200 exam from Red Hat](https://www.redhat.com/en/services/training/ex200-red-hat-certified-system-administrator-rhcsa-exam).
It has written lessons, exercises, and other reading material.

You can [read it here](http://rbong.github.io/rhcsa-open-guide).

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
