# hello-world-vue-pre-rendered

[![CircleCI](https://circleci.com/gh/mtlynch/hello-world-vue-pre-rendered.svg?style=svg)](https://circleci.com/gh/mtlynch/hello-world-vue-pre-rendered) [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](LICENSE)

## Overview

This is an example of a [Vue](https://vuejs.org) + [Nuxt](https://nuxtjs.org) configuration that generates the simplest possible pre-rendered, static web app.

## Detailed walkthrough

For a detailed walkthrough of this project, see the blog post, ["A Simple Pre-Rendered Web App Using Vue + Nuxt"](https://mtlynch.io/simple-vue-pre-rendered/) on mtlynch.io.

## Requirements

- [Node.js](https://nodejs.org/en/download/)

## Quick Start

```bash
npm install
npm run dev
```

Visit [http://localhost:3600](http://localhost:3600) to see the site running.

## Deploying to production

To pre-render your website, run

```bash
npm install
npm run generate
```

This will generate all the files for a static, pre-rendered version of your website under the `dist/` folder. You can upload these files to any service that suports static website hosting, such as:

- [Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/dev/WebsiteHosting.html)
- [Google Cloud Storage](https://cloud.google.com/storage/docs/hosting-static-website)
- [Netlify](https://www.netlify.com/blog/2016/10/27/a-step-by-step-guide-deploying-a-static-site-or-single-page-app/)

The [circleci-firebase](https://github.com/mtlynch/hello-world-vue-pre-rendered/tree/circleci-firebase) branch of this repo includes an example configuration that automatically builds your site using Circle CI and deploys it to Firebase.

## Customization

To customize this template for your project:

1. Find/replace "https://hello-world-vue-pre-rendered.web.app" with your app's hostname.
1. Find/replace "hello-world-vue-pre-rendered" with your repo name.

## Live Demo

The live version of this project is at:

- [https://hello-world-vue-pre-rendered.web.app](https://hello-world-vue-pre-rendered.web.app)

## Pre-Vue

[Pre-Vue](https://github.com/mtlynch/pre-vue) is a free, open source, MIT-licensed Vue project template that extends this demo and adds features such as:

- Generates a sitemap (for SEO)
- Generates a robots.txt (for SEO)
- Supports unique `<title>` tags for each page (for SEO)
- Adds unique opengraph tags to each page (for social sharing)
- Adds a favicon
- Handles 404s
