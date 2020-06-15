# eGo^n project website

This repository contains the code for generating the site [ego-n.org](https://ego-n.org).

# Build and serve the site locally

Bot is possible, building the site with a local installation of Jekyll or containing Jekyll in a Docker container.

The site is served at [localhost:4000/](localhost:4000/) in both cases.

To work around Jekyll build errors, create to folders which are required

```
mkdir .jekyll-cache _site
```

## Local installation

```
jekyll serve --watch
```

The flag `--ẁatch` sets Jekyll in autoreload mode. Whenever a file is changed, its changed are served immediately.


## Docker container

```
docker run --rm -p 4000:4000 --volume="$PWD/vendor/bundle:/usr/loc/bundle" --volume="$PWD:/srv/jekyll" -it jekyll/jekyll:3.8 jekyll serve --watch
```

# Deploy to webserver

Use the deploy script and deploy files from dev or production purpose

# Development

...will be deployed to staging.ego-n.org with restricted access


```
./DEPLOY staging
```

# Development

...will be deployed publicly accessible to ego-n.org 


```
./DEPLOY productive
```

