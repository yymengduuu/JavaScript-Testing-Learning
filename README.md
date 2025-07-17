# JavaScript-Testing-Learning

## SetUp

```
npm install --save-dev jest
```
---

## Basic concept in testing

- toBe
text(desciption, function)

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
  expect(data).yoEqual({ one:1, two:2 })
})
```


---
