# grunt-set-angular

A set of grunt tasks to help with angular development.

## Features

* jshint js files
* run ngmin on js files
* automatically add bower dependencies
* pre-process less files
* load `*.html` files into angular template cache
* convert `data/*.yaml` into angular constants
* convert `translations/*.yaml` into angular constants
* watch files for changes and automatically run correct task
* start up a dev server with livereload
* auto copy over images and fonts to the `dist` folder
* deploy to s3

## Suggested Folder Structure

```
dev/
  modules/
    some-module/
      module.js
      styles.less
      view.html
  directives/
    some-directive/
      directive.js
      view.html
      style.less
  services/
    some-service.js
  styles/
    vars.less
    base.less
  images/
    logo.png
  fonts/
    app.ttf
  app.js
```

## Options

```javascript
{
  dev: 'dev'
  dist: 'www',
  //only needed if deploying to s3
  aws: {
    accessKeyID: '',
    secretAccessKey: '',
    bucket: ''
  }
}
```

## Commands

* `dev` - start up dev server and watch for changes
* `dist` - build and minify
* `deploy` - deploy to s3


