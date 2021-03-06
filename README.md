# fuzzysearch

> Fuzzy search in JavaScript

Fuzzy searching allows for flexibly matching a string with partial input, useful for filtering data very quickly based on lightweight user input.

# Install

From `npm`

```shell
npm install --save fuzzysearch
```

# `fuzzysearch(query, data)`

Returns `true` if `query` matches `data` using a fuzzy-searching algorithm.

```js
fuzzysearch('twl', 'cartwheel') // <- true
fuzzysearch('cart', 'cartwheel') // <- true
fuzzysearch('cw', 'cartwheel') // <- true
fuzzysearch('ee', 'cartwheel') // <- true
fuzzysearch('art', 'cartwheel') // <- true
fuzzysearch('eeel', 'cartwheel') // <- false
fuzzysearch('dog', 'cartwheel') // <- false
```

# License

MIT
