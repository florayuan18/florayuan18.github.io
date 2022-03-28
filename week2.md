---
layout: page
title: Week 2 - Calculator
subtitle: Flora Yuan
---
## Challenges
**Week 2 - Calculator**

Challenges:
* Change to RPN to hold calculation
* Use power of operators

## Code Snippets
```javascript
switch (token) {

    case "(":
        tokenStack.push(token);
        break;
    case ")":
        while (tokenStack.peek() != null && !tokenStack.peek().equals("(")) {
            reverse_polish.add( (String)tokenStack.pop() );
        }
        tokenStack.pop();
        break;
    case "*":
    case "/":
    case "+":
    case "-":
    case "%":
    case "^":
```

* This snippet of the function I wrote to convert to reverse polish notation.  I originally tried by using an if statement, but it was not as effective.  I decided to use a switch statement instead because of the many cases that the operators could fall under.

```javascript
for (String token : this.reverse_polish) {
    if (!isOperator(token)) {
        stackCalculation.push(token); // if not an operator, placed in stack
    }
    else {
        Double operand1 = Double.valueOf( (String)stackCalculation.pop() ); // changing string to double
        Double operand2 = Double.valueOf( (String)stackCalculation.pop() ); // in order to actually calculate
//                System.out.println("operand1=" + operand1 + " operand2=" + operand2); // test code - checking which is which

        Double myResult;

        switch (token) { // switch is better than if for multiple cases
            case "*":
                myResult = operand2 * operand1;
                break;
            case "/":
                myResult = operand2 / operand1;
                break;
            case "+":
                myResult = operand2 + operand1;
                break;
            case "-":
                myResult = operand2 - operand1;
                break;
            case "%":
                myResult = operand2 % operand1;
                break;
            case "^":
                myResult = Math.pow(operand2, operand1);
                break;
            default:
                myResult = 0.00; // two decimals
```

* This is part of the function to dictate what would happen with each case, following the previous example.

* These challenges helped me better understand reverse polish notation.  I think the most difficult part of this challenge was definitely trying to figure out the concept behind it.  Even with the explanation in class, I still had trouble with it.  I think what helped me the most was the starter code that was given with the comments illustrating each step.  It reminds me to make sure my comments are as detailed as possible to ensure that my code is easy to read. 

## GitHub
[Challenge 1 & 2](https://github.com/florayuan18/just-to-suffer/commit/71c12b4f0cf4af825b848bb5944f2f695a88282a)

## Replit
[Replit](https://replit.com/@florayuan18/DataStructures#Main.java)