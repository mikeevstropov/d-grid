![npm version](https://badge.fury.io/js/d-grid.svg)
![license](https://img.shields.io/badge/license-mit-blue.svg)

## D-Grid

- To avoid media queries.
- To display the tiles grid.
- To split content to equal columns.
- Adaptivity is related to the parent width instead of window width.

## Installing

```
yarn add d-grid
```
or via `npm`
```
npm install d-gird
```

#### In Template

```html
<link rel="stylesheet" href="node_modules/d-grid/d-grid.min.css">
```

#### ES-Module

```javascript
import 'd-grid';
```

#### In Scss

```scss
@import "~d-grid";
```

## Classes

#### `.d-grid`

Applying `display: grid;` style.

#### `.grid-gap-{n}`

- `n` - gap size in range 1-12  

Applying gap between rows and columns.

#### `.row-gap-{n}`

- `n` - gap size in range 1-12  

Applying gap between rows only.

#### `.col-gap-{n}`

- `n` - gap size in range 1-12 

Applying gap between columns only.

#### `.fit-min-{n}`

- `n` - column min-width in range 1-12 

Expand columns to available space and apply column min-width.


#### `.fill-min-{n}`

- `n` - column min-width in range 1-12 

Fill the row to maximum number of columns and apply column min-width.

## Fit or Fill

The difference between *auto-fill* and *auto-fit* for sizing columns is only noticeable when the first row is wide enough to fit more columns in it.

If you’re using *auto-fit*, the content will stretch to fill the entire row width. Whereas with *auto-fill*, the browser will allow empty columns to occupy space in the row like their non-empty neighbors — they will be allocated a fraction of the space even if they have no grid items in them, thus affecting the size/width of the latter.

[read more](https://css-tricks.com/auto-sizing-columns-css-grid-auto-fill-vs-auto-fit/)

## Scss Variables

- `$gaps: 12` - max range of gap classes
- `$fits: 12` - max range of auto-fit classes
- `$fills: 12` - max range of auto-fill classes
- `$minGap: 2px` - min gap size in `px`
- `$maxGap: 190px` - max gap size in `px`
- `$minWidth: 40px` - min column width in `px`
- `$maxWidth: 1000px` - max column width in `px`

## Build

#### 1. Install dependencies.

```
yarn install
```

#### 2. Run build script.

```
yarn build
```

#### 3. Check out `dist` folder.

```text
d-grid/
├── dist/
│   ├── d-grid.css
│   ├── d-grid.css.map
│   ├── d-grid.min.css
```
