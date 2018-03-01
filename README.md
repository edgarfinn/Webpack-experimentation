# Webpack-experimentation
Webpack-experimentation

- Loading CSS
- Loading images
  - checkout also:
    - [image-webpack-loader](https://github.com/tcoopman/image-webpack-loader)
    - [url-loader](https://webpack.js.org/loaders/url-loader/)
- Loading fonts
- Loading Data
- Global Assets

### Loaders
Loaders are additional node modules that work to transform various types of files (css, scss, js, jsx etc...) of a developer's source code, and convert them into modules that can be used in an application's dependency graph.

When multiple loaders are chained together in one array, they pass input / output from right-to-left or end-to-beginning of the array. So in the below example ```css-loader``` takes the developer's source code, transforms it, and passes it on to ```style-loader```.

```js
module: {
  rules: [
    {
      test: /\.css$/,
      use: [
        'style-loader', 'css-loader'
      ]
    }
  ]
}
```
