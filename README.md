![license](https://img.shields.io/badge/license-mit-blue.svg)

## Installing

```
yarn add d-grid
```
or via `npm`
```
npm install d-gird
```

##### In Template

```html
<link rel="stylesheet" href="node_modules/d-grid/d-grid.min.css">
```

##### ES-Module

```javascript
import 'd-grid';
```

##### In Sass

```sass
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

## Sass Variables

- `$gaps` - max range of gap classes
- `$fits` - max range of auto-fit classes
- `$fills` - max range of auto-fill classes
- `$minGap` - min gap size in `px`
- `$maxGap` - max gap size in `px`
- `$minWidth` - min column width in `px`
- `$maxWidth` - max column width in `px`

## Build

##### 1. Install dependencies.

```
yarn install
```
or via `npm`
```
npm install
```

##### 2. Run build command.

```
yarn build
```
or via `npm`
```
npm run build
```

##### 3. Check out `dist` folder.

```text
d-grid/
├── dist/
│   ├── d-grid.css
│   ├── d-grid.css.map
│   ├── d-grid.min.css
```
