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

## Audit || loadCSS

Next step is to make the css load async instead.  I will be doing this with [filamentgroup/loadcss](https://github.com/filamentgroup/loadCSS).


### Filmstrip
It seems the html indeed loads on screen way earlier. But the complete render takes way longer.
![filmstrip](./readme-images/PM-loadCSS-filmstrip.png)

### Chrome DevTools Audit
Seems pretty much the same.
![DevTools Audit](./readme-images/PM-loadCSS-chromeAudit.png)

### PageSpeed Insights
I lost one point...
![PageSpeed Insights](./readme-images/PM-loadCSS-PageSpeedInsights.png)
