# JavaScript-Shorthand

## 1. The Ternary Operator 

Longhand:

```javascript
const x = 20;
let answer;

if (x > 10) {
    answer = "greater than 10";
} else {
    answer = "less than 10";
} 
```
Shorthand:

```javascript
const answer = x > 10 ? "greater than 10" : "less than 10";
```
## 2. Short-circuit Evaluation Shorthand

Longhand:

```javascript
if (value !== null || value !== undefined || value !== '') {
     let setValue = value;
}
```
Shorthand:

```javascript
const setValue = value || 'new';
```
```javascript
let value;
let setValue = value || 'bar';
console.log(setValue === 'bar'); // prints true
```
```javascript
value = 'foo';
setValue = value || 'bar';
console.log(setValue); // prints foo
```

## 3. If Presence Shorthand

Longhand:

```javascript
if (likeJavaScript === true)
if (likeJavaScript === false)
```
Shorthand:

```javascript
if (likeJavaScript)
if (!likeJavaScript)
```

## 4. Decimal Base Exponents

Longhand:

```javascript
for (let i = 0; i < 10000; i++) {}
```
Shorthand:

```javascript
for (let i = 0; i < 1e7; i++) {}

// All the below will evaluate to true
1e0 === 1;
1e1 === 10;
1e2 === 100;
1e3 === 1000;
1e4 === 10000;
1e5 === 100000;
```

## 5. JavaScript For Loop Shorthand

Longhand:

```javascript
const array = [4, 8, 15, null, 23, undefined]
const imperative = []
for (let i = 0, len = array.length; i < len; ++i) {
    if (array[i]) {
        imperative.push(array[i])
    }
}
```

Shothand:

```javascript
const declarative = array.filter(Boolean)
```

## 6. Object Property Shorthand

Longhand:

```javascript
const x = 1920, y = 1080;
const obj = { x:x, y:y };
```
Shorthand:

```javascript
const obj = { x, y };
```

## 7. Arrow Functions Shorthand

Longhand:

```javascript
function sayHello(name) {
  console.log('Hello', name);
}

setTimeout(function() {
  console.log('Loaded')
}, 2000);

list.forEach(function(item) {
  console.log(item);
});
```

Shorthand:

```javascript
sayHello = name => console.log('Hello', name);

setTimeout(() => console.log('Loaded'), 2000);

list.forEach(item => console.log(item));
```

## 8. Implicit Return Shorthand

Longhand:

```javascript
function calcCircumference(diameter) {
  return Math.PI * diameter
}
```

Shorthand:

```javascript
calcCircumference = diameter => (
  Math.PI * diameter;
)
```

## 9. Double Bitwise NOT Shorthand

Longhand:

```javascript
Math.floor(4.9) === 4  //true
```

Shorthand:

```javascript
~~4.9 === 4  //true
```
