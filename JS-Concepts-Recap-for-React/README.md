## **Brushing Up on JavaScript Fundamentals:** <span style="font-size: 24px; font-weight: 200"> A Pre-Requisite for Mastering React JS </span>

---

Before plunging headfirst into the realm of React JS, it's critical to have a firm grasp on the fundamental JavaScript ideas. Here, we'll take a step back and review the essential JavaScript building blocks you'll need to get the most out of your React adventure. This subsection will walk you through the basic principles that form the backbone of modern web development using React, whether you're new to JavaScript or just need a fast refresher. Let's get started on this important pre-React JS preparation.

---

#### Declaring variables and constants:

```js
let name = "Muntahi";
const age = 21;
```

---

#### Arrays:

```js
const numbers = [89, 35, 98, 12];
numbers[0] = 56;
```

---

#### If-else condition:

```js
if (fatherName === "arnold" || season === "rainy") {
} else if (fatherName === "Arnold") {
} else {
}
```

---

#### For-else loop:

```js
for (let i = 0; i < numbers.length; i++) {
    const number = numbers[i];
    confirm.log(number);
}
```

---

#### Function:

```js
function multiply(num1, num2) {
    const result = num1 * num2;
    return result;
}

const output = multiply(35, 78);
```

---

#### Object:

```js
const student = {
    name: "Salib Khan",
    age: 32,
    movies: ["king khan", "Dhakar Mastan"],
};

const myVariable = "age";

// 3 ways to access property by name
console.log(student.age); // direct by property
console.log(student["age"]); // access via property name string
console.log(student[myVariable]); // access via property name in a variable
```

---

#### Template String:

```js
const numbers = [89, 35, 98, 12];
const student = {
    name: "Salib Khan",
    age: 32,
    movies: ["king khan", "Dhakar Mastan"],
};

const about = `My Name is ${student.name} age of ${student.age} has number ${numbers[2]} also liked movies ${student.movies[0]}`;
console.log(about);
```

---

#### Arrow Function:

```js
const getFiftyFive = () => 55;
const addSixtyFive = (num) => num + 65;
const isEven = (x) => x % 2 == 0;
const addThree = (x, y, z) => x + y + z;
const doMath = (num1, num2) => {
    const sum = num1 + num2;
    return sum;
};
```

---

#### Spread Operator:

```js
const numbers = [89, 35, 98, 12];

const newNumbers = [...numbers];
// create a new array from an older array and add an element
const currentNumbers = [...numbers, 55];

numbers.push(99);
numbers.push(99);
numbers.push(99);

console.log(numbers);
console.log(newNumbers);
console.log(currentNumbers);
```

---

#### Different Array Methods (map, filter, find etc):

```js
const products = [
    { name: "laptop", price: 3200, brand: "lenovo", color: "silver" },
    { name: "phone", price: 7000, brand: "iphone", color: "golden" },
    { name: "watch", price: 3000, brand: "casio", color: "yellow" },
    { name: "sungalss", price: 300, brand: "ray", color: "black" },
    { name: "camera", price: 9000, brand: "canon", color: "gray" },
];

const brands = products.map((product) => product.brand);
// console.log(brands);
const prices = products.map((product) => product.price);
// console.log(prices);

// products.forEach(product => console.log(product))
// products.forEach(product => console.log(product.color))
products.forEach((product) => {});

// 3. filter
const cheap = products.filter((product) => product.price <= 5000);
// console.log(cheap);

const specificName = products.filter((p) => p.name.includes("n"));
// console.log(specificName);

// 4. find
const special = products.find((p) => p.name.includes("n"));
console.log(special);
```
