# gatsby-spon-scss-postcss

Based almost entirely on gatsby-plugin-sass

Provides drop-in support for SASS/SCSS stylesheets

## Install

`npm install --save gatsby-spon-scss-postcss`

## How to use

1.  Include the plugin in your `gatsby-config.js` file.
2.  Write your stylesheets in SASS/SCSS and require/import them

```javascript
// in gatsby-config.js
plugins: [`gatsby-spon-scss-postcss`]
```

```javascript
// in gatsby-config.js
plugins: [
	{
		resolve: `gatsby-spon-scss-postcss`,
		options: {
			postCssPlugins: [tailwind('./tailwind.config.js'), autoprefixer()],
			precision: 8
		}
	}
]
```
