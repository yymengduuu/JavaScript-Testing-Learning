# JavaScript-Testing-Learning

## SetUp

```
npm install --save-dev jest
```

e.g.

sum.js
```
module. exports = myFunction;
```

sum.test.js
```
const myFunction = require(./sum)
```

---

## Basic concept in testing

text ( desciption, function)

- toBe

```
text('two plus two is four',() => {
  expect(2+2).toBe(4);
)
```

- toEqual

```
test('object assignment', () => {
  const data = { one: 1};
  date['two'] = 2;
  expect(data).toEqual({ one:1, two:2 });
})
```

- truthy & falsy
  
```
text('zero is falsy',() => {
  const n = 0;
  expect(n).toBeFalsy();
)
```

```
text('zero is truthy',() => {
  const n = 1;
  expect(n).toBeTruthy();
)
```

- error handling

```
text('throws on invalid input',() => {
  expect(() => {
    myFunction(invalidInput);
  }).toThrow();
)
```

---

## Testing Asynchronous Code

sum.js

```
function fetchData (callback) {
  setTimeout(() => {
    callback('peanut butter')
  }, 1000)
}

module. exports = fetchData;
```

sum.test.js

```
test('the data is peanut butter', done => {
  function callback (data) {
    try {
      expect (data). toBe('peanut butter');
      done ();
    } catch (error) {
        done (error);
    }
  }
  fetchData(callback);
})
```



---
