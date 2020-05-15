## Jekyll boilerplate

Search-optimized Jekyll static site boilerplate. Includes basic pages and posts layouts, json-ld Schema for WebPage, BlogPosting, a sitemap.xml file, blog feed, and frontmatter fields mapping to on-page metadata head.html markup.

_This repository accompanies a live presentation from VirtuaCon on May 15th, 2020 - video replay coming._

- Simple and customizable components and layouts
- Quick setup and management via config file
- Light-weight, performant layouts for pages and posts
  - This is a boilerplate, with very little focus on design/styling
  - Utilizes Tachyons CSS framework and Normalize.css
- Easy, site-wide Google Analytics (via Google Tag Manager) setup
- Search engine friendly - optimized metadata, Schema markup, and more
- Social sharing metadata for Twitter, Facebook, and more
- Sitemap.xml, XML feed of posts, and 404 Page

![Jekyll boilerplate site Lighthouse score](https://raw.githubusercontent.com/scottmathson/virtuacon-jekyll-boilerplate/master/assets/images/jekyll-lighthouse-score-live.png)

---

- [Installation](#installation)
- [Deploying](#deploying)
- [Resources](#resources)

## Installation

### As a Fork

1. [Fork the repo](https://github.com/scottmathson/virtuacon-jekyll-boilerplate#fork-destination-box)
  - As mentioned, you can then update/edit things directly on github.com or continue onward to run locally
2. From your terminal, clone the repo with `$ git clone git@github.com:username/reponame.git`
3. Install gems with `$ bundle install` (_install first if need be with `$ gem install bundler`_)
4. Run Jekyll locally with `$ bundle exec jekyll serve`

You can also run the site with Docker, [similarly to this method](https://github.com/scottmathson/simpol-theme#installation).

## Deploying

To get a site live right away with Netlify, you can get started by clicking the button below: 

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/scottmathson/virtuacon-jekyll-boilerplate?utm_source=github&utm_medium=virtuacon-jekyll&utm_campaign=scottmathson)

**Checklist**:

1. Replace `https://example.com` with your domain in `_config.yml` and `robots.txt` files
  - This will point crawlers hitting the robots.txt file to the correct sitemap path, as well as update `rel="canonical"` and other `{{site.url}}` references throughout this repository
2. Change site name or [set up custom domain in Netlify](https://docs.netlify.com/domains-https/custom-domains/?utm_source=github&utm_medium=virtuacon-jekyll&utm_campaign=scottmathson)
  - _All optional_ - if you're just testing things out, Netlify provides you with a free `*.netlify.app` subdomain
  - [Use external DNS providers](https://docs.netlify.com/domains-https/custom-domains/configure-external-dns/?utm_source=github&utm_medium=virtuacon-jekyll&utm_campaign=scottmathson#configure-a-subdomain), deploying this site to a subdomain atop your existing domain, or utilize Netlify DNS and even [register a domain on Netlify](https://docs.netlify.com/domains-https/netlify-dns/domain-registration/?utm_source=github&utm_medium=virtuacon-jekyll&utm_campaign=scottmathson)
3. Update other site options and information throughout `_config.yml`
4. Add your Google Analytics ID in config `google_tracking_id` and Google Tag Manager container ID in `_includes/misc/ga-gtm.txt` and `_includes/gtm-body.html`

From there feel free to delete/update contents of index and blog pages, the "hello world" post, and [get familiar with markdown](https://scottmathson.com/blog/2017/04/15/markdown-overview-blogging-with-jekyll/?ref=virtuacon) if you're not already.

This is just one deployment option for this Jekyll starter site, a couple of other great options for building and deploying static sites include Cloudflare, GitHub Pages, and more.

## Resources

Check out these resources for help in deploying Jekyll sites, in general.

- [Deploy Jekyll to Netlify](https://www.netlify.com/blog/2015/10/28/a-step-by-step-guide-jekyll-3.0-on-netlify/?utm_source=github&utm_medium=virtuacon-jekyll&utm_campaign=scottmathson) (can skip directly to the ["Connecting to Netlify" section](https://www.netlify.com/blog/2015/10/28/a-step-by-step-guide-jekyll-3.0-on-netlify/?utm_source=github&utm_medium=virtuacon-jekyll&utm_campaign=scottmathson#connecting-to-netlify))
- [Deploy Jekyll to GitHub Pages](https://jekyllrb.com/docs/github-pages/)

Scott Mathson <https://scottmathson.com/> | [scottmathson on GitHub](https://github.com/scottmathson) | [scottmathson on Twitter](https://twitter.com/scottmathson), [Mathson Design, LLC](https://mathsondesignco.com/)

---

## License

Copyright (c) 2020 Mathson Design, LLC and Scott Mathson

Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.