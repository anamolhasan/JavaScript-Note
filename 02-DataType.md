# Data Type

### primitive data types
- প্রিমিটিভ ডাটা টাইপ হলো সহজ, মৌলিক মান যা অবজেক্ট নয় এবং পরিবর্তনযোগ্য নয়

**Number** 
```bash
let age = 25;
let pi = 3.14
```
**string**
```bash
let name = 'Anam'
```
**Boolean**
```bash
let isTrue = true;
let isFalse = false;
```
***Non-Zero Values এবং Boolean Context***
#### JavaScript-এ non-zero মান অর্থ শূন্য ব্যতীত যেকোনো সংখ্যা।
 - উদাহরণ: 1, 5, 3.14
#### Boolean context (যেমন if statement) এ JavaScript বিবেচনা করে:
- 0 → false
- Non-zero → true
*উদাহরণ:*
```bash
let x = 5; // true

if (x) {   // x non-zero
  console.log("x is non-zero"); // চলবে
}

let y = 0;

if (y) {   // y zero
  console.log("y is non-zero"); // চলবে না
}
```
*সংক্ষেপে:*

- 0 → falsy

- Non-zero → truthy

Falsy মানসমূহ: false, 0, -0, "" (empty string), null, undefined, NaN
<br/>
Truthy মানসমূহ: -1, 1, "0", "false", [], {}

## ব্যবহার ক্ষেত্র (Use Cases)
1. Conditional Checks (শর্ত চেক করা)
```bash 
let itemsInCart = 3;

if (itemsInCart) {
  console.log("Proceed to checkout"); // Non-zero → চলে
} else {
  console.log("Cart is empty"); // Zero → চলে যদি itemsInCart = 0
}
```
2. Loops (লুপ)
```bash
let count = 5;

while (count) {  // Non-zero → true
  console.log(count);
  count--;       // count 0 হলে লুপ থামে
}
```
3. Mathematical Computations (গণিত)
```bash
let score = 0;

if (score === 0) {
  console.log("No points scored yet"); // Zero value check
}
```
4. Default Values / fallbacks
```bash
function calculateDiscount(price) {
  let discount = price ? price * 0.1 : 0; // Zero price → no discount
  return discount;
}
```
**Null এবং Undefined**
- Null: অভিপ্রেত “কোনো মান নেই” বোঝাতে।
```bash 
let data = null;
```
*উদাহরণ*:
```bash
let user = {
  name: "Adnan",
  phone: null  // ফোন নম্বর এখনও দেওয়া হয়নি
};
```
- Undefined: একটি ভেরিয়েবল ডিক্লেয়ার করা হয়েছে কিন্তু মান দেওয়া হয়নি।
```bash
let x;  //undefined
```
**সংক্ষেপ:**

- *null → স্পষ্টভাবে কোনো মান নেই*

- *undefined → মান দেওয়া হয়নি*
---
**String Indices (স্ট্রিং ইন্ডেক্স)**
```bash
let str = "Hello";
console.log(str[0])  // output: 'H'
console.log(str[3])  // output: 'l'
```
**Concatenation (স্ট্রিং যোগ)**    