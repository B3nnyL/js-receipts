# Map 

## Invert a map
given a map, and I want to a new map with inverted key and values
```js
	const map = new Map([...givenMap.entries()].map(
		([key, value]) => ([value, key]))
	)
```
