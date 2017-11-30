### It will take an entire array and paste it to index
 
```js
['alpha', 'bravo', 'charlie', 'delta'].copyWithin(2, 0);
// ["alpha", "bravo", "alpha", "bravo"]

```

Why is that? It takes all array ["alpha", "bravo", "alpha", "bravo"] and paste it at index 2. Everything else is trimmed.

```js
['alpha', 'bravo', 'charlie', 'delta'].copyWithin(3, 0);
// ["alpha", "bravo", "charlie", "alpha"]
// Insert all that at index 3.

['alpha', 'bravo', 'charlie', 'delta'].copyWithin(1);
// ["alpha", "alpha", "bravo", "charlie"]

```
#### Specify range by setting start and end

```js
['alpha', 'bravo', 'charlie', 'delta'].copyWithin(1, 3);
// ["alpha", "delta", "charlie", "delta"]
['alpha', 'bravo', 'charlie', 'delta'].copyWithin(1, 2);
// ["alpha", "charlie", "delta", "delta"]
['alpha', 'bravo', 'charlie', 'delta'].copyWithin(1, 1);
// ["alpha", "bravo", "charlie", "delta"]
```

```js
['alpha', 'bravo', 'charlie', 'delta'].copyWithin(1, -1);
(4) ["alpha", "delta", "charlie", "delta"]
['alpha', 'bravo', 'charlie', 'delta'].copyWithin(1, -2);
(4) ["alpha", "charlie", "delta", "delta"]
```