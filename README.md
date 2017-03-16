# Performance matters

## Project setup

This project serves an adapted version of the [Bootstrap documentation website](http://getbootstrap.com/). It is based on the [github pages branche of Bootstrap](https://github.com/twbs/bootstrap/tree/gh-pages).

Differences from actual Bootstrap documentation:

- Added custom webfont
- Removed third party scripts
- The src directory is served with [Express](https://expressjs.com/).
- Templating is done with [Nunjucks](https://mozilla.github.io/nunjucks/)

## Getting started

- Install dependencies: `npm install`
- Serve: `npm start`
- Expose localhost: `npm run expose`

## Audit || Before

Here you can see what the site's performance was prior to doing performance stuff.

### Filmstrip
![filmstrip](./readme-images/PM-before-filmstrip.png)

### Chrome DevTools Audit
![DevTools Audit](./readme-images/PM-before-chromeAudit.png)

### PageSpeed Insights
![PageSpeed Insights](./readme-images/PM-before-PageSpeedInsights.png)

## Audit || gzip

Next we will add gzip on the server side.

### Filmstrip
the filmstrip stayed pretty much the same.

### Chrome DevTools Audit
gzip note dissapeared.

![DevTools Audit](./readme-images/PM-gzip-chromeAudit.png)

### PageSpeed Insights
Gained 13 points :tada:

![PageSpeed Insights](./readme-images/PM-gzip-PageSpeedInsights.png)
