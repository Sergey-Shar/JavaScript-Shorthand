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

## 4. . Decimal Base Exponents

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

