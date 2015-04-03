# 移动端快速开发指南

> [传送门](http://junmer.github.io/mobile-dev-get-started)

## run

```
$ npm i -g reveal-md
$ reveal-md index.md
```

## build reveal

```
$ npm install reveal.js
$ cp -r node_modules/reveal.js/{js,css,lib,plugin} .
$ wget http://localhost:1948/index.md -O index.html
```

修改 `index.html` 中的 `/css/theme/${theme}.css`
