# html-minifier-loader   [![NPM version](https://badge.fury.io/js/html-minifier-loader.svg)](https://badge.fury.io/js/html-minifier-loader)

Webpack loader that minifies HTML by [html-minifier](https://github.com/kangax/html-minifier).

Installation
---
```console
npm install html-minifier html-minifier-loader --save
```

Example of webpack.config.js
---
You can pass [html-minifier](https://github.com/kangax/html-minifier) parameters by 'html-minifier-loader' property.
The default is `{removeComments: true, collapseWhitespace: true}`.
```js
module: {
    loaders: [
        {    test: /\.html$/,
             loader: 'raw-loader!html-minifier-loader'
        }
    ]
},
'html-minifier-loader': {
    removeComments: false,
    collapseWhitespace: true,
    conservativeCollapse: true,
    preserveLineBreaks: true
}
```
