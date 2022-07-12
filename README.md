[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/lgdd/lfr-react-remote-app)

# Liferay React Remote App

This is a template intended for tests & demos. The webpack configuration included is not optimized for production environments.

## Using this template

By default, the custom element name is `lfr-react-remote-app`. You can change it in [src/index.js](src/index.js#7):

```js
const ELEMENT_ID = 'lfr-react-remote-app';
```

This template is using a custom webpack configuration to build your application in a single file (`bundle.js`) making easier to create a _Remote App_ in Liferay DXP/Portal.

You can find multiple scripts in [package.json](package.json#14) not using `react-scripts`:

- `start`: watch files under `src/` and run `serve` if there is any change (allows you to keep the single file approach on localhost).
- `serve`: run the `build` script and `serve` the result on port `3000`.
- `build`: transpile your application to a `build` folder using webpack and its [configuration](webpack.config.js).
