# socialcount.js

Easily get social share counts for a url.

[![browser support](https://ci.testling.com/olahol/socialcount.js.png)
](https://ci.testling.com/olahol/socialcount.js)

## Example

```js
Socialcount.get("twitter", "http://github.com", function (count) {
  console.log(count); // 1164
});
```

```js
Socialcount.all("http://github.com", function (counts) {
  console.log(counts); // { twitter: 1164, facebook: 11111, pinterest: 6 }
});
```

## Methods

### Socialcount.get(provider, url, cb(count))

Get share count for `url` from `provider` (currently twitter, facebook and pinterest.)

* * *

### Socialcount.all(url, cb(counts))

Get all share counts for `url` from available providers, counts is an
object with the providers as keys and the counts as values.

## License

MIT