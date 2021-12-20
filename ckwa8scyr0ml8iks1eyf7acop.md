## The JavaScript Switch Statement Explained with Examples

[Full article available on <mark>Sweetcode</mark> for free](https://sweetcode.io/the-javascript-switch-statement-explained-with-examples/) 

**When learning any programming language, you will come across the concept of control flow. This is when we want our program to behave differently, based on the information and values we supply to it.**

One popular control flow structure is a switch statement. This will evaluate an expression and perform an action, based on the resulting value. In this article, we are going to learn how switch statements are implemented in JavaScript and how they differ from other control structures, such as `if...else` statements.

Let’s get right to it.

## The Syntax of a Switch Statement

The basic syntax of a switch statement is like so:

```javascript
switch (expression) {
  case value_1:
    statement_1;
    break;
  case value_2:
    statement_2;
    break;
  default:
    default_statement;
}
```

As you can see, the switch statement receives an expression. An expression is any unit of code, that resolves to a value. For example:

- `3 + 4`
- `'hello' + 'world'`
- `a > 20`
- `false`

You can read more about expressions on [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#expressions).

The switch statement will evaluate the result of the expression and either execute the matching `case` statement, or the `default` statement in the event that no `case` statements match.

Let's look at this using a practical example:

```javascript
const name = 'lary';

switch (name) {
  case 'lary':
    alert('Hi lary!');
    break;
  case 'Hillary':
    alert('Hi Hillary!');
    break;
  default:
    alert('Howdy stranger!');
}
```

Try running this code. Change the value of the `name` variable and notice how a different greeting is output to the screen. 

Once control of a program enters a switch statement, the `expression` is first executed, then followed by matching the first case constant to the value of the expression result, in the case they match, the statements in that clause are executed.

In a scenario that they do not match, control of the program goes on to compare the expression’s result to the second clause, evaluating its statements when there is a match.

Once the statements of a given case clause are executed, where a `break` statement is used, this ends the switch case, and program control is returned to the main program. Since `break` statements are optional, when they are not available, the program will continue matching other case clauses that flow irrespective they matched the case without a break statement. This introduces some very unique usage for a switch statement.

In a scenario where non of the clauses match, the `default` clause if available is executed, calling all the statements for the default clause and then exiting the switch statement. When a `default` clause is not available, no statements within any of the switch cases would be executed.

## Flow Diagram

Check out the complete [Article](https://sweetcode.io/the-javascript-switch-statement-explained-with-examples/) on Sweetcode. 

*No registration is needed to access the article*

Connect With me at [Twitter](https://twitter.com/larymak1) | [Insta](https://www.instagram.com/nextgencoders/) | [YouTube](https://www.youtube.com/channel/UCrT1ARRZfLOuf6nc_97eXEg) | [LinkedIn](https://www.linkedin.com/in/hillary-nyakundi)  | [GitHub](https://github.com/larymak) 

Enjoy Coding ❤