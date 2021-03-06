# egg-mongoose-redis

[![NPM version][npm-image]][npm-url]
[![build status][travis-image]][travis-url]
[![Test coverage][codecov-image]][codecov-url]
[![David deps][david-image]][david-url]
[![Known Vulnerabilities][snyk-image]][snyk-url]
[![npm download][download-image]][download-url]

[npm-image]: https://img.shields.io/npm/v/egg-mongoose-redis.svg?style=flat-square
[npm-url]: https://npmjs.org/package/egg-mongoose-redis
[travis-image]: https://img.shields.io/travis/ewinds/egg-mongoose-redis.svg?style=flat-square
[travis-url]: https://travis-ci.org/ewinds/egg-mongoose-redis
[codecov-image]: https://img.shields.io/codecov/c/github/ewinds/egg-mongoose-redis.svg?style=flat-square
[codecov-url]: https://codecov.io/github/ewinds/egg-mongoose-redis?branch=master
[david-image]: https://img.shields.io/david/ewinds/egg-mongoose-redis.svg?style=flat-square
[david-url]: https://david-dm.org/ewinds/egg-mongoose-redis
[snyk-image]: https://snyk.io/test/npm/egg-mongoose-redis/badge.svg?style=flat-square
[snyk-url]: https://snyk.io/test/npm/egg-mongoose-redis
[download-image]: https://img.shields.io/npm/dm/egg-mongoose-redis.svg?style=flat-square
[download-url]: https://npmjs.org/package/egg-mongoose-redis

Mongoose cache plugin for egg

## Install

```bash
$ npm i egg-mongoose-redis --save
```

## Usage

```js
// {app_root}/config/plugin.js
exports.mongooseRedis = {
  enable: true,
  package: "egg-mongoose-redis"
};
```

## Example

```javascript
// query
const results = await ctx.model.User.find({foo: "bar"}).cache(ttl || 7200, key);;
```

## License

[MIT](LICENSE)
