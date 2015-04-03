# DoSomething.org Tech Blog

This repository contains the template, configuration, and markdown files that Jekyll uses to build our blog as a static site.

Each time a commit is merged to master, GitHub Pages triggers a rebuild. The live site is updated within seconds.

![DoSomething Tech Blog](/assets/images/dosomething-tech-blog.jpg "DoSomething Tech Blog")

### Setting up your local development environment

You don't need to set up a local development environment to write a blog post, but it's nice for previewing what your post looks like.

1. Install Jekyll locally in one fell swoop using `gem install github-pages`. This mirrors the plug-ins used by GitHub Pages on your local machine; including Jekyll, Sass, and more.
1. Create your own fork of this repository and git clone it down.

### Writing your blog post

1. Create a new branch for your post.
1. Create a file for your new post in `/_drafts/` (take a look at [`/_drafts/2015-01-01-Post-Template.md`](https://github.com/DoSomething/dosomething.github.io/blob/master/_drafts/2015-01-01-Post-Template.md) as an example)
1. Write your post in markdown :eyeglasses:
1. Place any images that you use in `/images/`.
1. Run `jekyll serve --drafts` and go to [`http://0.0.0.0:4000`](http://0.0.0.0:4000) to view your post locally as you write.
1. Create a pull request to get feedback and track the progress of your post.
1. When your first draft is done, assign it to [Barry](https://github.com/barryclark/) and @mention [Matt](http://www.github.com/mshmsh5000) for review.

### Writing your blog post (without local dev)

1. Fork this repository.
1. Create a file for your new post in `/_drafts/` (take a look at [`/_drafts/2015-01-01-Post-Template.md`](https://github.com/DoSomething/dosomething.github.io/blob/master/_drafts/2015-01-01-Post-Template.md) as an example)
1. Write your post in markdown :black_nib:
1. Place any images that you use in `/images/`.
1. Use the preview tab on GitHub.com to view a rough version of what it will look like.
1. Create a pull request to get feedback and track the progress of your post.
1. When your first draft is done, assign it to [Barry](https://github.com/barryclark/) and @mention [Matt](http://www.github.com/mshmsh5000) for review.

### Adding your author info

1. Hop into [_config.yml](https://github.com/DoSomething/dosomething.github.io/blob/master/_config.yml)
1. You'll find author information near the top. Copy/paste mine and add your own info in.
1. When writing a post, add `author: yourname` to the front-matter at the top to pull in your author information and GitHub avatar.

### Contributing to the theme

- Template files are in `_layout` (except the homepage template, which is located at `/index.html` - slightly confusing I know :neckbeard:)
- Compiled CSS is pulled in from [DS Neue](http://neue.dosomething.org) located at `/ds-neue/` and blog specific style overrides are made in `/blog.scss`.
- Sitewide variables and Jekyll settings are contained in `_config.yml`. Note that changes to `_config.yml` won't be picked up by jekyll serve, you'll need to kill the process and re-run it.

When you're done, open a PR and assign [Dave](http://www.github.com/dfurnes/) and [Barry](http://www.github.com/barryclark) for review.

For more info on how the tech blog works, check out [Building A Blog With Jekyll and GitHub Pages](http://www.smashingmagazine.com/2014/08/01/build-blog-jekyll-github-pages/).
