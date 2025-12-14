# waline-plugins-tms

A Waline plugin that adds Tencent Cloud TMS content moderation to Waline when a new comment is posted.

## How to Install

```sh
npm i waline-plugins-tms
```

## How to Use

```js
// index.js
const Waline = require('@waline/vercel');
const TencentTMS = require('waline-plugins-tms');

module.exports = Waline({
  plugins: [
    TencentTMS({
      secretId: 'xxx',
      secretKey: 'xxx',
      region: 'ap-beijing',
    })
  ]
});
```

## Acknowledgements

Derived from `@waline-plugins/tencent-tms`.
