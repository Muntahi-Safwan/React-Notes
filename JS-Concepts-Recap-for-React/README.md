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

---

#### Array Destructuring:

```js
const numbers = [42, 65];
const x = numbers[0];
const y = numbers[1];

const [x, y] = [42, 65];

// const [x, y] = numbers;

function boxify(num1, num2) {
    const nums = [num1, num2];
    return nums;
}

// const [first, second] = [90, 34]
const [first, second] = boxify(90, 34);

// console.log(boxify(90, 34));
const student = {
    name: "Salib Khan",
    age: 32,
    movies: ["king khan", "Dhakar Mastan"],
};

const [firstMovie, secondMovie] = student.movies;

// object destructuring
const { name, age } = { name: "alu", age: 14 };
const { name, age } = { id: 12, name: "alu", salary: 3400, age: 14 };

const employee = {
    ide: "VS Code",
    designation: "developer",
    machine: "mac",
    languages: ["html", "css", "js"],
    specification: {
        height: 66,
        weight: 67,
        address: "kumarkhali",
        drink: "water",
        watch: {
            color: "black",
            price: 500,
            brand: "garmin",
        },
    },
};

const { machine, ide } = employee;
const { weight, address } = employee.specification;
const { brand } = employee?.specification?.watch;
```

---

#### JSON methods and API Fetching:

```js
// 1. JSON => stringify, parse

const student = {
    name: "Salib Khan",
    age: 32,
    movies: ["king khan", "Dhakar Mastan"],
};
const studentJSON = JSON.stringify(student);
// console.log(student);
// console.log(studentJSON);

const studentObj = JSON.parse(studentJSON);
// console.log(studentObj);

//2. fetch
fetch("url")
    .then((res) => res.json())
    .then((data) => console.log(data));

// keys, values
const keys = Object.keys(student);
const values = Object.values(student);

// for
const numbers = [23, 54, 67, 87, 23, 78];
numbers.forEach((num) => console.log(num));
numbers.map((num) => num * 2);

// for of on array like object
// loop on an object using for in

// add or remove from an array
const products = [
    { name: "laptop", price: 3200, brand: "len", color: "silver" },
    { name: "phone", price: 7000, brand: "HTC", color: "golden" },
    { name: "watch", price: 3000, brand: "casio", color: "yellow" },
    { name: "sungalss", price: 300, brand: "ray", color: "black" },
    { name: "camera", price: 9000, brand: "canon", color: "gray" },
];

const newProduct = { name: "webcam", price: 700, brand: "Lal" };

// copy products array and then add newProduct
const newProducts = [...products, newProduct];
// create a new array without one specific item
// remove phone means create a new array without the phone
const remaining = products.filter((p) => p.name !== "phone");
```

---

#### Truthy-Falsy Boolean:

```js
// 'almas', 5, true, {}, []
// '', 0, false, null, undefined
// check truthy
let myVar = 5;
// check any truthy
if (myVar) {
    myVar = myVar * 100;
} else {
    myVar = 0;
}

let myMoney = 50;
// you check negative or falsy anything
if (!myMoney) {
}

const money = 800;
let food;
if (money > 100) {
    food = "biryani";
} else {
    food = "cha biscuit";
}

// ternary
let food1 = money > 100 ? "biryani" : "cha biscuit";
// console.log(food1);

let drink = money > 100 && myVar > 100 ? "coke" : "filter water";
// console.log(drink);

// number to string conversion
const num1 = 52;
// console.log(num1);
const numStr = num1 + "";
// console.log(numStr)

// string to number
const input = "560";
const inputNum = +input;
// console.log(inputNum);

//
let isActive = true;
const showUser = () => console.log("display User");
const hideUser = () => console.log("hide User");
// isActive ? showUser() : hideUser();
// use && if the left side is true then right side will be executed
isActive && showUser();
// use || if the left side is false then right side will be executed
isActive || hideUser();

// toggle boolean
isActive = !isActive;
```

---

#### Local Storage methods:

```js
const addToLocalStorage = () => {
    const idInput = document.getElementById("storage-id");
    const id = idInput.value;
    const valueInput = document.getElementById("storage-value");
    const value = valueInput.value;

    //
    if (id && value) {
        localStorage.setItem(id, value);
    }
    idInput.value = "";
    valueInput.value = "";
};
```

---

### Overall Summary:

##### Fundamentals

1.1 variable (let, const) three types variable
1.2 condition (<. >, ===, !==. <=, >=) && ||, if-else if-else
1.3 array: declare, length, index, push, pop, indexOf, includes
1.4 for loop, while
1.5 function return parameter
1.6 Object property, including array, object

---

##### ES6:

1. template string ${}
2. spread (...)
   2.1 copy an array then add a new element to an array
   2.1 use filter to remove an element from an array
3. Arrow function
   3.1 no parameter ()
   3.2 single parameter
   3.3 multiple parameters ()
   3.4 multi line
   4 destructuring : object destructuring array destructuring
4. object declaration shorthand
5. function parameter default value
6. Optional chaining (?.)

---

##### Browser API

1. local storage session stoage
2. location API
3. History API
4. fetch

---

##### Others:

1. array: map, forEach, filter, find
2. ternary operator
3. logical and logical or && ||
4. JOSN (stringify, parse)
5. +,
