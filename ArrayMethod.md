# ১. Array Creation & Access
    bash```
    const arr = [1, 2, 3, 4];
    console.log(arr[0]); // 1
    console.log(arr.length); // 4
    ```

# ২. Adding / Removing Elements
- Method	Description	Example
- push()	Array-এর শেষে element যোগ করে	arr.push(5) → [1,2,3,4,5]
- pop()	Array-এর শেষ element remove করে	arr.pop() → [1,2,3,4]
- unshift()	Array-এর শুরুতে element যোগ করে	arr.unshift(0) → [0,1,2,3,4]
- shift()	Array-এর প্রথম element remove করে	arr.shift() → [1,2,3,4]
# ৩. Iteration Methods
- Method	Description	Example
- forEach()	Array-এর প্রতিটি element-এর উপর function চালায়	arr.forEach(n => console.log(n))
- map()	প্রতিটি element modify করে নতুন array দেয়	arr.map(n => n*2) → [2,4,6,8]
filter()	condition অনুযায়ী নতুন array দেয়	arr.filter(n => n>2) → [3,4]
- reduce()	Array-এর values combine করে single value দেয়	arr.reduce((acc,n)=>acc+n,0) → 10
# ৪. Searching / Finding
- Method	Description	Example
- indexOf()	element এর index খুঁজে বের করে	arr.indexOf(3) → 2
- includes()	element আছে কি না চেক করে	arr.includes(2) → true
- find()	first element matching function returns	arr.find(n => n>2) → 3
- findIndex()	first element matching function index returns	arr.- findIndex(n => n>2) → 2
# ৫. Sorting / Reversing / Joining
- Method	Description	Example
- sort()	Array sort করে	[3,1,2].sort() → [1,2,3]
- reverse()	Array reverse করে	[1,2,3].reverse() → [3,2,1]
- join()	Array elements string হিসেবে join করে	[1,2,3].join('-') → "1-2-3"
- split()	string কে array তে ভাগ করে	"a,b,c".split(',') → ["a","b","c"]
# ৬. Others
- Method	Description	Example
- slice(start, end)	Array-এর subarray return করে	[1,2,3,4].slice(1,3) → [2,3]
- splice(start, deleteCount, ...items)	Array modify করে	[1,2,3,4].- splice(1,2,5,6) → [1,5,6,4]
- concat()	Arrays join করে	[1,2].concat([3,4]) → [1,2,3,4]
- flat()	nested array flatten করে	[1,[2,3]].flat() → [1,2,3]
- fill(value, start, end)	Array elements fill করে	[1,2,3].fill(0,1,3) → [1,0,0]

💡 Tip:

## map(), filter(), reduce() মূলত functional programming এর জন্য ব্যবহার হয়।

## splice() মূল array modify করে, slice() নতুন array return করে।