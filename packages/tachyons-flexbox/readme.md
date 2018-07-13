# tachyons 5.0.0-1

Functional CSS for humans

### Stats

1189 | 192 | 192
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

# FLEXBOX

### Docs

http://tachyons.io/docs/layout/flexbox/

### Media Query Extensions

- `-s` = small
- `-m` = medium
- `-l` = large
*/
.flex { display: flex; }
.inline-flex { display: inline-flex; }
.flex-1 { flex: 1; }
.flex-auto { flex: 1 1 auto; }
.flex-initial { flex: initial; }
.flex-none { flex: none; }
.flex-column { flex-direction: column; }
.flex-row { flex-direction: row; }
.flex-wrap { flex-wrap: wrap; }
.flex-nowrap { flex-wrap: nowrap; }
.flex-wrap-reverse { flex-wrap: wrap-reverse; }
.flex-column-reverse { flex-direction: column-reverse; }
.flex-row-reverse { flex-direction: row-reverse; }
.items-start { align-items: flex-start; }
.items-end { align-items: flex-end; }
.items-center { align-items: center; }
.items-baseline { align-items: baseline; }
.items-stretch { align-items: stretch; }
.self-start { align-self: flex-start; }
.self-end { align-self: flex-end; }
.self-center { align-self: center; }
.self-baseline { align-self: baseline; }
.self-stretch { align-self: stretch; }
.justify-start { justify-content: flex-start; }
.justify-end { justify-content: flex-end; }
.justify-center { justify-content: center; }
.justify-between { justify-content: space-between; }
.justify-around { justify-content: space-around; }
.content-start { align-content: flex-start; }
.content-end { align-content: flex-end; }
.content-center { align-content: center; }
.content-between { align-content: space-between; }
.content-around { align-content: space-around; }
.content-stretch { align-content: stretch; }
.order-0 { order: 0; }
.order-1 { order: 1; }
.order-2 { order: 2; }
.order-3 { order: 3; }
.order-4 { order: 4; }
.order-5 { order: 5; }
.order-6 { order: 6; }
.order-7 { order: 7; }
.order-8 { order: 8; }
.order-last { order: 99999; }
.flex-grow-0 { flex-grow: 0; }
.flex-grow-1 { flex-grow: 1; }
.flex-shrink-0 { flex-shrink: 0; }
.flex-shrink-1 { flex-shrink: 1; }
@media screen and (min-width: 30em) {
 .flex-s { display: flex; }
 .inline-flex-s { display: inline-flex; }
 .flex-1-s { flex: 1; }
 .flex-auto-s { flex: 1 1 auto; }
 .flex-initial-s { flex: initial; }
 .flex-none-s { flex: none; }
 .flex-column-s { flex-direction: column; }
 .flex-row-s { flex-direction: row; }
 .flex-wrap-s { flex-wrap: wrap; }
 .flex-nowrap-s { flex-wrap: nowrap; }
 .flex-wrap-reverse-s { flex-wrap: wrap-reverse; }
 .flex-column-reverse-s { flex-direction: column-reverse; }
 .flex-row-reverse-s { flex-direction: row-reverse; }
 .items-start-s { align-items: flex-start; }
 .items-end-s { align-items: flex-end; }
 .items-center-s { align-items: center; }
 .items-baseline-s { align-items: baseline; }
 .items-stretch-s { align-items: stretch; }
 .self-start-s { align-self: flex-start; }
 .self-end-s { align-self: flex-end; }
 .self-center-s { align-self: center; }
 .self-baseline-s { align-self: baseline; }
 .self-stretch-s { align-self: stretch; }
 .justify-start-s { justify-content: flex-start; }
 .justify-end-s { justify-content: flex-end; }
 .justify-center-s { justify-content: center; }
 .justify-between-s { justify-content: space-between; }
 .justify-around-s { justify-content: space-around; }
 .content-start-s { align-content: flex-start; }
 .content-end-s { align-content: flex-end; }
 .content-center-s { align-content: center; }
 .content-between-s { align-content: space-between; }
 .content-around-s { align-content: space-around; }
 .content-stretch-s { align-content: stretch; }
 .order-0-s { order: 0; }
 .order-1-s { order: 1; }
 .order-2-s { order: 2; }
 .order-3-s { order: 3; }
 .order-4-s { order: 4; }
 .order-5-s { order: 5; }
 .order-6-s { order: 6; }
 .order-7-s { order: 7; }
 .order-8-s { order: 8; }
 .order-last-s { order: 99999; }
 .flex-grow-0-s { flex-grow: 0; }
 .flex-grow-1-s { flex-grow: 1; }
 .flex-shrink-0-s { flex-shrink: 0; }
 .flex-shrink-1-s { flex-shrink: 1; }
}
@media screen and (min-width: 48em) {
 .flex-m { display: flex; }
 .inline-flex-m { display: inline-flex; }
 .flex-1-m { flex: 1; }
 .flex-auto-m { flex: 1 1 auto; }
 .flex-initial-m { flex: initial; }
 .flex-none-m { flex: none; }
 .flex-column-m { flex-direction: column; }
 .flex-row-m { flex-direction: row; }
 .flex-wrap-m { flex-wrap: wrap; }
 .flex-nowrap-m { flex-wrap: nowrap; }
 .flex-wrap-reverse-m { flex-wrap: wrap-reverse; }
 .flex-column-reverse-m { flex-direction: column-reverse; }
 .flex-row-reverse-m { flex-direction: row-reverse; }
 .items-start-m { align-items: flex-start; }
 .items-end-m { align-items: flex-end; }
 .items-center-m { align-items: center; }
 .items-baseline-m { align-items: baseline; }
 .items-stretch-m { align-items: stretch; }
 .self-start-m { align-self: flex-start; }
 .self-end-m { align-self: flex-end; }
 .self-center-m { align-self: center; }
 .self-baseline-m { align-self: baseline; }
 .self-stretch-m { align-self: stretch; }
 .justify-start-m { justify-content: flex-start; }
 .justify-end-m { justify-content: flex-end; }
 .justify-center-m { justify-content: center; }
 .justify-between-m { justify-content: space-between; }
 .justify-around-m { justify-content: space-around; }
 .content-start-m { align-content: flex-start; }
 .content-end-m { align-content: flex-end; }
 .content-center-m { align-content: center; }
 .content-between-m { align-content: space-between; }
 .content-around-m { align-content: space-around; }
 .content-stretch-m { align-content: stretch; }
 .order-0-m { order: 0; }
 .order-1-m { order: 1; }
 .order-2-m { order: 2; }
 .order-3-m { order: 3; }
 .order-4-m { order: 4; }
 .order-5-m { order: 5; }
 .order-6-m { order: 6; }
 .order-7-m { order: 7; }
 .order-8-m { order: 8; }
 .order-last-m { order: 99999; }
 .flex-grow-0-m { flex-grow: 0; }
 .flex-grow-1-m { flex-grow: 1; }
 .flex-shrink-0-m { flex-shrink: 0; }
 .flex-shrink-1-m { flex-shrink: 1; }
}
@media screen and (min-width: 60em) {
 .flex-l { display: flex; }
 .inline-flex-l { display: inline-flex; }
 .flex-1-l { flex: 1; }
 .flex-auto-l { flex: 1 1 auto; }
 .flex-initial-l { flex: initial; }
 .flex-none-l { flex: none; }
 .flex-column-l { flex-direction: column; }
 .flex-row-l { flex-direction: row; }
 .flex-wrap-l { flex-wrap: wrap; }
 .flex-nowrap-l { flex-wrap: nowrap; }
 .flex-wrap-reverse-l { flex-wrap: wrap-reverse; }
 .flex-column-reverse-l { flex-direction: column-reverse; }
 .flex-row-reverse-l { flex-direction: row-reverse; }
 .items-start-l { align-items: flex-start; }
 .items-end-l { align-items: flex-end; }
 .items-center-l { align-items: center; }
 .items-baseline-l { align-items: baseline; }
 .items-stretch-l { align-items: stretch; }
 .self-start-l { align-self: flex-start; }
 .self-end-l { align-self: flex-end; }
 .self-center-l { align-self: center; }
 .self-baseline-l { align-self: baseline; }
 .self-stretch-l { align-self: stretch; }
 .justify-start-l { justify-content: flex-start; }
 .justify-end-l { justify-content: flex-end; }
 .justify-center-l { justify-content: center; }
 .justify-between-l { justify-content: space-between; }
 .justify-around-l { justify-content: space-around; }
 .content-start-l { align-content: flex-start; }
 .content-end-l { align-content: flex-end; }
 .content-center-l { align-content: center; }
 .content-between-l { align-content: space-between; }
 .content-around-l { align-content: space-around; }
 .content-stretch-l { align-content: stretch; }
 .order-0-l { order: 0; }
 .order-1-l { order: 1; }
 .order-2-l { order: 2; }
 .order-3-l { order: 3; }
 .order-4-l { order: 4; }
 .order-5-l { order: 5; }
 .order-6-l { order: 6; }
 .order-7-l { order: 7; }
 .order-8-l { order: 8; }
 .order-last-l { order: 99999; }
 .flex-grow-0-l { flex-grow: 0; }
 .flex-grow-1-l { flex-grow: 1; }
 .flex-shrink-0-l { flex-shrink: 0; }
 .flex-shrink-1-l { flex-shrink: 1; }
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
