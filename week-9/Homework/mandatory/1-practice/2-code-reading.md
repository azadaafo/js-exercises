# Code reading

## Question 1

Take a look at the following code:

```
1    let x = 1;
2    {
3        let x = 2;
4        console.log(x);
5    }
6    console.log(x);
```

Explain why line 4 and line 6 output different numbers. 
## line 4 has a local scope, so the value of x is 2. 
## line 6 outpods 1 which is the value of x, and x is a global scope variable outside curly braces.
## Question 2

Take a look at the following code:

```
let x = 10

function f1()
{
    console.log(x)
    let y = 20
}

console.log(f1())
console.log(y)
```

## What will be the output of this code. Explain your answer in 50 words or less.
## we get 10 because x is a global variable that can be accessed even within the function.
## the function itself and y outpuds undefined because the call is made outside the function while y is not global variable.

## Question 3

Take a look at the following code:
## i need Mitch to explain this to me.
```
const x = 9;

function f1(val) {
  val = val + 1;
  return val;
}

f1(x);
console.log(x);

const y = { x: 9 };

function f2(val) {
  val.x = val.x + 1;
  return val;
}

f2(y);
console.log(y);
```

What will be the output of this code. Explain your answer in 50 words or less.
