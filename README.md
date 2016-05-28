# https-pushstate-server

A simple static http/https file server that works with HTML5 Pushstate.

Defaults all routes to `index.html` in the given root directory. Treats all other files to be static, and routes urls with the given static directories to make them relative to root.

For example,

* `localhost` or `localhost/a/pushstate/route` will always return `index.html`.

* `localhost/assets/emoji.png` or `localhost/a/pushstate/route/assets/emoji.png` will always return `assets/emoji.png` when `assets` directory is given as one of the static directories.



### Install

`npm install https-pushstate-server --save`   

`npm install https://github.com/aerofs/https-pushstate-server —save`

### Usage

```shell
$ https-pushstate-server -r rootDir -p 8000 -s -c certFile -k keyFile
```

