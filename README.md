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

```javascriprt
const setValue = value || 'new';

let value;
let setValue = value || 'bar';
console.log(setValue === 'bar'); // prints true
```
```javascript
value = 'foo';
setValue = value || 'bar';
console.log(setValue); // prints foo
```
