## Compile the website on github
Typically if you're only making minor changes to the `.md` files, you can just push it to the remote. Github should build and deploy it automatically.
You can check if deployment is successful and the logs under 'Deployment' on the right sidebar.

## Compile the website locally
The site is built by Jekyll. You can follow Jekyll instruction here: https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll.

Below is my setup.

I'm using rbenv to set up the Ruby environment.
```
rbenv local 2.7.1
[path to .rbenv]/shims/bundle install
```

To build and serve the site locally, run
```
[path to .rbenv]/shims/bundle exec jekyll serve
```

## For TAs: Edit course website
- `staff.md`: add your personal information in `_staffers`; your photos should go in `assets`.
- `calendar.md`: this is where we post most course content for students. Note that ideally you should only add link to the files on this page. The actual content is added to a different repo, [`course-material`](https://github.com/nyu-cs2590/course-material).
