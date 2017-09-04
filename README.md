# sass-theme-defaults

[![npm version](https://badge.fury.io/js/sass-theme-defaults.svg)](https://badge.fury.io/js/sass-theme-defaults)

Importable personal default classes and variables I use in my projects

[Github Pages Demo](https://torch2424.github.io/sass-theme-defaults/).
[NPM Module Link](https://www.npmjs.com/package/sass-theme-defaults).

## Usage

Install to the project:

```
npm install --save sass-theme-defaults
```

Simply import at the top of a sass file to get going:

```scss
@import './node_modules/sass-theme-defaults/index.scss';

// Other Sass down here...
```

I'd highly suggest visiting the [Github Pages Demo](https://torch2424.github.io/sass-theme-defaults/) for the classes and variables. but here is a quick run down of all of them:

`$standard` - The dark color, should be used for things like font color


`$sub-standard` - The light-dark color, should be used for things like sub text


`$inverse` - The opposite of $standard. The light color, could be used for a page background color


`$links` - The light blue color. Should be used for links outside of the current page


`$transparent-x` - Available 'x' values are 25, 50, 75. A dark transparent color, could be used to darken the page when a sidebar opens.


`$transparent-light-x` - Available 'x' values are 25, 50, 75. A light transparent color, could be used to lighten parts of the page.


`.center` - centers a div or display: block element


`.center-text` - centers a div and its text elements


`.center-children` - centers a divs children horizontally and vertically


`.center-children-horizontal` - centers a divs children only horizontally


`.center-children-vertical` - centers a divs children only vertically


## Example

In HTML on an element:

```html
<div class="center-text">
  I am centered! 🖥️
</div>
```

Within Sass:

```sass
.my-awesome-class {
  @extends .center

  background-color: $standard;
}
```

## Contributing

Clone the project:

```
git clone https://github.com/torch2424/sass-theme-defaults.git
```

Install devDependencies:

```
npm install
```

Run the command: `npm run build`, to continuously see changes to the `index.html` in the `docs` folder. Sorry, but no livereload or watch is set up for this (Since it's just a simple little package).

## LICENSE

[MIT](https://choosealicense.com/licenses/mit/#)
