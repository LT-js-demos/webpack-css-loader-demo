#webpack-css-loader-demo

We want to add a css file to our application.

webpack can only handle JavaScript natively, so we need the `css-loader` to process CSS files. 
We also need the `style-loader` to apply the styles in the CSS file.

Run `npm install css-loader style-loader` to install the loaders. 
(They need to be installed locally, without `-g`) This will create a `node_modules` folder for you, in which the loaders will live.

##How to run
```
npm install -g webpack
npm install
webpack ./entry.js bundle.js
```
Then open `index.html`

###Note:

Or you can use:

```
webpack ./entry.js bundle.js --module-bind 'css=style!css'
```
that you can just write require('./index.css') in you js file.