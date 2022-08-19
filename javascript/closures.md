# Closures

Closures is a really powerful feature in JavaScript. 

If we have a scenario where there is a nested function, one outer and one inner:

```js
const name = function(yourName) {

  const getName = function() {
    return yourName;
  }

  return getName
}
```
In the example above, our outer function, `name`, would not have access to any functions or variables defined inside of the `getName` function. But on the flip-side, `getName` has complete access to the functions and variables set in the outer function, `name`.

Now this is where closures come in. A closure is the combination of a function and its lexical environment. So with the given example above, the data that has been encapsulated, will not leak out!

Good resources:

- [Fireship video](https://www.youtube.com/watch?v=vKJpN5FAeF4)
- [MDN Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures#closure)
