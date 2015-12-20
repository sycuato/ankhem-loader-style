# ankhem-loader-style
Ankhem Component: Loader for style

CSS, SASS

## Usage

Your webpack.config.js maybe like this:

```javascript
var ExtractTextPlugin = require('extract-text-webpack-plugin');

module.exports = {
	module: {
		loaders: [
			{
				test: /\.scss$/,
				exclude: /(node_modules|bower_components)/,
				loader: ExtractTextPlugin.extract('css!sass')
			}
		]
	}
};
```
