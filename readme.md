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

替换路径

```
$ cat index.html | sed \
    -e "s#'/lib/#'lib/#g" \
    -e "s#\"/lib/#\"lib/#g" \
    -e "s#\"/js/#\"js/#g" \
    -e "s#\"/css/#\"css/#g" \
    -e "s#'/plugin/#'plugin/#g" \
    -e "s#default.css#black.css#g" \
    > _index.html && mv _index.html index.html

```
