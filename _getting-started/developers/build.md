### Dependencies

- Ruby 2.3.1
- Node.js v5.0.0+

Install dependencies:

```
npm install
```

We use Bourbon 4.2.7. We include its `.scss` files directly rather than calling it via its node (or gem) package. Bourbon and Neat live under `/assets/sass/vendor`.

### Using npm

Run a build:
```
npm run-script build
```

Run a build with livereloading:
```
npm start
```

The UI-Kit CSS is at `./build/latest/ui-kit.css`

### Key libraries

- gulp ^3.9.1
- gulp-sass ^2.3.1
- kss ^3.0.0-beta.14
- sass-lint ^1.7.0

^ = compatible with version (see <a href="https://docs.npmjs.com/misc/semver#caret-ranges-123-025-004" rel="external">semver</a>)

The build also uses:
- `sass-lint` for linting
- `cssnano` for CSS compression
- `autoprefixer` for adding CSS vendor prefixes
- `AusDTO/gulp-html` for HTML validation

The CI build is available as a shell script at `bin/cibuild.sh`.