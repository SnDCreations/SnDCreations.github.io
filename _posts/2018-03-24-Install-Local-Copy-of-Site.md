---
title: "Set up local copy of site"
layout: post
date: 2018-03-24
---

To day I have installed a local copy of this web site. Using **Jekyll**.
I have refered [Setting up your GitHub Pages site locally with Jekyll](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/) for that.

As per the instruction below command used for check the Ruby version.

```bash
ruby --version
```
I had to installed Ruby, then bundler but after completting most of the items, an error message popped up in the terminal.

> Failed to build gem native extension...

After searching this error message, I realised that this is due to missing header files. To avoid that we need to install Ruby dev version.

```bash
apt-get install ruby-dev

```
Then we can install bundle.

```bash
bundle install

```

After that we can start the Jekull server


```bash
bundle exec jekyll serve

```
We can preview local Jekyll site in the web browser at `http://localhost:4000`
