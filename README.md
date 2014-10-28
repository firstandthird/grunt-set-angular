# grunt-set-ionic

## Structure

```sh
dev/
  modules/
  directives/
  services/
  styles/
  images/
  fonts/
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

`dev` - start up dev server and watch for changes

`dist` - build and minify

`deploy` - deploy to s3


