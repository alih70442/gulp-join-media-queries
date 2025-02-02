# gulp-join-media-queries

> Combine matching media queries into one media query definition. Useful for CSS generated by preprocessors using nested media queries.


This plugin is the further development of the originally fork [gulp-merge-media-queries](https://github.com/1ven/gulp-merge-media-queries).
Which is inspired from [grunt-combine-media-queries](https://github.com/buildingblocks/grunt-combine-media-queries).

## Install

```
npm install gulp-join-media-queries --save-dev
```

## Usage
```javascript
var jmq = require('gulp-join-media-queries');

gulp.task('jmq', function () {
  gulp.src('src/**/*.css')
    .pipe(jmq({
      log: true
    }))
    .pipe(gulp.dest('dist'));
});
```

## Options

### log

Type: `boolean` Default: `false`

Log processed media queries.

### use_external

Type: `boolean` Default: `false`

Writes media queries into external file, named as [src].responsive.css

## License

(MIT License)

Copyright (C) 2017-2019 by Mausbrand Informationssysteme GmbH.

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
