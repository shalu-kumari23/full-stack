# full-stack

# JavaScript Practice Programs

This project contains basic JavaScript programs written inside an HTML `<script>` tag.
The programs demonstrate fundamental programming concepts such as loops, variables, arithmetic operations, and number manipulation.

---

# Programs Included

1. Fibonacci Series
2. Factorial
3. Sum of Numbers
4. Palindrome Number
5. Triangle Pattern

---

# Full Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>JavaScript Practice</title>
</head>
<body>

<script>
// fibonacci
let n = 10;
let a = 0, b = 1;
document.write(`fibonacci <br>`)
for (let i = 1; i <= n; i++) {
    document.write(`${a} <br>`)
    let next = a + b;
    a = b;
    b = next;
}

// factorial
let m = 5;
let fact = 1;
document.write("Factorial : ")
for(let i = 1; i <= m; i++){
    fact *= i;
}

document.write(`${fact}<br>`);

// sum of number 
let k = 5;
let sum = 0;

for(let i = 1; i <= k; i++){
    sum += i;
}

document.write(` sum : ${sum}<br>`);

// palindrome
let l = 12121;
let j = l;
let p = l.toString().length;
let pal = 0;

for(let i = 0; i < p; i++){
    let digit = l % 10;
    pal = pal * 10 + digit;
    l = Math.floor(l / 10);
}

if(j == pal){
    document.write(`${pal} is palindrome <br>`);
}
else{
    document.write(`${pal} is not palindrome <br>`);
}

// pattern
for(let i = 1; i <= 5; i++){
    for(let j = 1; j <= i; j++){
        document.write("*");
    }
    document.write("<br>");
}

</script>

</body>
</html>
```

---

# Concepts Used

## 1. Fibonacci Series

The Fibonacci sequence is a series where each number is the sum of the previous two numbers.

Example:
0, 1, 1, 2, 3, 5, 8, ...

Concepts used:

* Variables
* `for` loop
* Arithmetic operations
* Updating values inside loop

Logic:

* Start with `a = 0` and `b = 1`
* Print `a`
* Calculate next value using `a + b`
* Shift values forward

---

## 2. Factorial

Factorial of a number `n` is the product of all positive integers from `1` to `n`.

Example:
5! = 5 × 4 × 3 × 2 × 1 = 120

Concepts used:

* Variables
* `for` loop
* Multiplication operator
* Accumulator variable

Logic:

* Start with `fact = 1`
* Multiply `fact` by numbers from `1` to `n`

---

## 3. Sum of Numbers

This program calculates the sum of numbers from `1` to `k`.

Example:
1 + 2 + 3 + 4 + 5 = 15

Concepts used:

* Variables
* `for` loop
* Addition operator

Logic:

* Initialize `sum = 0`
* Add each number from `1` to `k`

---

## 4. Palindrome Number

A palindrome number reads the same forward and backward.

Example:
121, 1331, 12321

Concepts used:

* Loops
* Modulus operator `%`
* Integer division
* Number reversal logic
* Conditional statements (`if-else`)

Logic:

* Extract digits using `% 10`
* Reverse the number
* Compare reversed number with original

---

## 5. Triangle Pattern

This program prints a star (`*`) triangle pattern.

Example:

```
*
**
***
****
*****
```

Concepts used:

* Nested loops
* `for` loops
* Pattern printing
* HTML line break `<br>`

Logic:

* Outer loop controls rows
* Inner loop prints stars in each row

---

# Technologies Used

* HTML
* JavaScript

---

# Output Method

The output is displayed using:

```
document.write()
```

which writes content directly to the webpage.

---

# Purpose

This project helps beginners understand:

* Basic JavaScript syntax
* Looping structures
* Mathematical logic
* Pattern printing
* Number manipulation
