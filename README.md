# JavaScript-Testing-Learning

## SetUp

```
npm install --save-dev jest
```

e.g.
sum.js
```
module exports = myFunction;
```

sun.test.js
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
