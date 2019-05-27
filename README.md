# @sapper-dragon/remark

Decorate your [Sapper](https://sapper.svelte.dev/) project with Remark.

`@sapper-dragon/remark` utilizes [Remark](https://remark.js.org/) under the surface, which is a tool for converting markdown files to HTML.

## Installation

```
npm install @sapper-dragon/remark --save-dev
# or
yarn add @sapper-dragon/remark --dev
```

## Usage

This project requires the [@sapper-dragon/trimmings](https://github.com/sapper-dragon/trimmings) lib, so look there first for first instructions, then come back. 💫

`@sapper-dragon/remark` converts files from an `remark` folder and exports them to importable `*.svelte` files.

### Config

You can place a `trimmings.config.js` file in the root of your project to set configutations. These are the defaults:

```js
export default {
	remark: {
		watchPath: 'src/trimmings/remark', // path to watch *.md files:
		pathMatcher: /\.md$/, // pattern for files to watch:
		sveltePath: 'src/routes/_markdown', // svelte output path:
	},
	// ... additional settings from other @sapper-dragon packages...
}
```
