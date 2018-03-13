# tachyons 5.0.0-1

Functional CSS for humans

### Stats

522 | 39 | 39
---|---|---
bytes | selectors | declarations

## Installation

#### With [npm](https://npmjs.com)

```
npm install --save-dev tachyons
```

Learn more about using css installed with npm:
* https://webpack.github.io/docs/stylesheets.html
* https://github.com/defunctzombie/npm-css

#### With Git

http:
```
git clone https://github.com/tachyons-css/tachyons
```

ssh:
```
git clone git@github.com:tachyons-css/tachyons.git
```

## Usage

#### Using with [Postcss](https://github.com/postcss/postcss)

Import the css module

```css
@import "tachyons";
```

Then process the css using the [`tachyons-cli`](https://github.com/tachyons-css/tachyons-cli)

```sh
$ npm i -g tachyons-cli
$ tachyons path/to/css-file.css > dist/t.css
```

#### Using the css

##### CDN
The easiest and most simple way to use the css is to use the cdn hosted version. Include it in the head of your html with:

```
<link rel="stylesheet" href="http://unpkg.com/tachyons@5.0.0-1/css/tachyons.min.css" />
```

##### Locally
The built css is located in the `css` directory. It contains an unminified and minified version.
You can either cut and paste that css or link to it directly in your html.

```html
<link rel="stylesheet" href="path/to/module/css/tachyons">
```

#### Development

The source css files can be found in the `src` directory.
Running `$ npm start` will process the source css and place the built css in the `css` directory.

## The css

```css
/*!!!

# OPACITY

Please note that this module should be used
with the core opacity module. This only provides
responsive classes for opacity.

### Docs

http://tachyons.io/docs/addons/opacity-responsive/
http://tachyons.io/docs/themes/opacity/

### Base

- o = opacity

### Modifiers

- `-100` = literal value 1
- `-90`  = literal value .9
- `-80`  = literal value .8
- `-70`  = literal value .7
- `-60`  = literal value .6
- `-50`  = literal value .5
- `-40`  = literal value .4
- `-30`  = literal value .3
- `-20`  = literal value .2
- `-10`  = literal value .1
- `-05`  = literal value .05
- `-025` = literal value .025
- `-0`   = literal value 0

### Media Query Extensions

- `-s` = small
- `-m` = medium
- `-l` = large
*/
@media screen and (min-width: 30em) {
 .o-100-s { opacity: 1; }
 .o-90-s { opacity: .9; }
 .o-80-s { opacity: .8; }
 .o-70-s { opacity: .7; }
 .o-60-s { opacity: .6; }
 .o-50-s { opacity: .5; }
 .o-40-s { opacity: .4; }
 .o-30-s { opacity: .3; }
 .o-20-s { opacity: .2; }
 .o-10-s { opacity: .1; }
 .o-05-s { opacity: .05; }
 .o-025-s { opacity: .025; }
 .o-0-s { opacity: 0; }
}
@media screen and (min-width: 48em) {
 .o-100-m { opacity: 1; }
 .o-90-m { opacity: .9; }
 .o-80-m { opacity: .8; }
 .o-70-m { opacity: .7; }
 .o-60-m { opacity: .6; }
 .o-50-m { opacity: .5; }
 .o-40-m { opacity: .4; }
 .o-30-m { opacity: .3; }
 .o-20-m { opacity: .2; }
 .o-10-m { opacity: .1; }
 .o-05-m { opacity: .05; }
 .o-025-m { opacity: .025; }
 .o-0-m { opacity: 0; }
}
@media screen and (min-width: 60em) {
 .o-100-l { opacity: 1; }
 .o-90-l { opacity: .9; }
 .o-80-l { opacity: .8; }
 .o-70-l { opacity: .7; }
 .o-60-l { opacity: .6; }
 .o-50-l { opacity: .5; }
 .o-40-l { opacity: .4; }
 .o-30-l { opacity: .3; }
 .o-20-l { opacity: .2; }
 .o-10-l { opacity: .1; }
 .o-05-l { opacity: .05; }
 .o-025-l { opacity: .025; }
 .o-0-l { opacity: 0; }
}
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## Authors

* [mrmrs](http://mrmrs.io)
* [johno](http://johnotander.com)

## License

ISC
