## The JavaScript Switch Statement Explained with Examples

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

The switch statement will evaluate the result of the expression and either execute the matching `case` statement or the `default` statement in the event that no `case` statements match.

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

Try running this code. Change the value of the `name` variable and notice how a different greeting is an output to the screen. 

Once control of a program enters a switch statement, the `expression` is first executed, then followed by matching the first case constant to the value of the expression result, in the case they match, the statements in that clause are executed.

In a scenario that they do not match, control of the program goes on to compare the expression’s result to the second clause, evaluating its statements when there is a match.

Once the statements of a given case clause are executed, where a `break` statement is used, this ends the switch case, and program control is returned to the main program. Since `break` statements are optional, when they are not available, the program will continue matching other case clauses that flow irrespective they matched the case without a break statement. This introduces some very unique usage for a switch statement.

In a scenario where non of the clauses match, the `default` clause if available is executed, calling all the statements for the default clause and then exiting the switch statement. When a `default` clause is not available, no statements within any of the switch cases would be executed.

## Flow Diagram

![flow diagram](https://i.imgur.com/pCyqvFL.png)

As shown above, the program starts by executing the given expression, then checking the results match/equal to the given case constant, in which case it would go-ahead to execute the statements for the matching case. When `break` statements are provided, the program exits the switch statement immediately, otherwise continues evaluating other cases. 

So how exactly does the Switch statement work in JavaScript? 

## How Switch Statement Works in JavaScript 

### JavaScript Keywords

#### Expression

In JavaScript, expressions are blocks of code that evaluate a value, meaning that the given expression must return a value. This is the value to be compared to the constant defined in each case clause. Switch statements evaluate a given expression only once.

#### Cases

Cases define how values from the expression compare to each given case. In JavaScript, the comparison of results is strict `===`, meaning values must be of the same type.

To retain changes made while executing a switch statement, variables are set outside of the switch block, and their values can be altered within the matching cases.

Variables can also be scoped within the case blocks of a given clause by using `let` and `const`.

One outstanding feature of cases is the different outcomes based on the provision of a `break` statement at the end of the case blocks. When provided, once it's encountered, the execution within the switch block ends, otherwise, other clauses are evaluated.

#### Default Case

The default case is optional and can be defined in whichever position within the switch block, it's evaluated when all the other cases do not match the value of the given expression. A `break` statement is not necessary in this case as the execution of the switch statement ends here anyway. 

## Examples of Switch Statements

Example to print name of the Day fetched from the day of the week of the current date-time. This can be used to modify the result of the expected day name says _' Monday'_ to something funky as _'Money Day'_.

```javascript
const epoch_day = new Date("January 1, 1970 00:00:00");
switch (epoch_day.getDay()) {
  case 0:
    console.log("Sunny Day");
    break;
  case 1:
    console.log("Money Day");
    break;
  case 2:
    console.log("Two Days");
    break;
  case 3:
    console.log("Wedding Day");
    break;
  case 4:
    console.log("Thus Day");
    break;
  case 5:
    console.log("Free Day");
    break;
  case 6:
    console.log("Sabbath Day");
    break;
  default:
    console.log("Not a day of the week.");
}
```

First a constant is defined with epoch time in JavaScript Date format. The expression evaluates the day of the week with `Date.protocol.getDay()` of the constant date variable, which returns an integer representing days of the week, i.e. 0-6 to Sunday to Saturday respectively.

The returned value is compared with the given result, returning a modified name of the day of the week of epoch time. 

## Executing Multiple Cases if Condition Satisfies

Considering that `break` statements are optional, multiple cases can be evaluated within the same switch block. When no `break` statement is provided, the program will continue to execute other case's statement block until a `break` statement is encountered.

For example, let's use a switch statement to find when epoch time was either a weekday or weekend.

```javascript
let epoch_date = new Date("January 1, 1970 00:00:00");
switch (epoch_date.getDay()) {
  case 1:
  case 2:
  case 3:
  case 4:
  case 5:
    console.log("Epoch was on a weekday");
    break;
  case 6:
  case 0:
    console.log("Epoch was on a weekend");
    break;
  default:
    console.log("Invalid day of the week");
}
```

In the above example, `break` statement having been omitted for the case blocks of the first 5 case clauses, ensures that once any of the case constant matches a given value, its code block will be executed, but since there are no defined statements, it goes on to execute other case clauses until encountering a `break` system, that exits the program from execution.

## Switch Statement vs If Else Statement

`if-else` statements is a conditional control structure that is used to compare against a pair of outcomes. This can only be either `true` or `false` responses, and any other custom matching required should always return a boolean. If else statements are used to evaluate at most 2 conditions.

Switch statements have better support for handling multiple result expressions, unlike if-else statement that mostly works on binary results of an expression, ie. there can only be 2 outcomes. Multiple conditions can be achieved with if-else statements, by nesting multiple if-else statements together.

Even though it’s possible to achieve similar control flow with `if-else` statements, `switch case` offers more readability of the code, as nested if conditions are not always quick to read through and understand the flow of a program.

An Example of a nested if-else statement usage.

```javascript
let epoch_date = new Date("January 1, 1970 00:00:00");
var day = epoch_date.getDay();
if (day === 0) {
  console.log("[IF] Epoch was on a weekend");
} else if (day <= 5) {
  console.log("[IF ELSE] Epoch was on a weekeday");
} else if (day === 6) {
  console.log("[IF ELSE] Epoch was on a weekend");
} else {
  console.log("[ELSE] Invalid day of the week");
}
```

## When to use Switch Statement

Perhaps, you might wonder why use switch statement if we have the alternative if-else, here is why:

For easier code readability and understanding, Switch statements, as we have explored in the examples, are better suited for multiple cases of an expected result. While an if-else statement would be better for cases with only 2 conditions.

## Wrap up

The `switch` conditional statements are often used to evaluate an expression and return a response on whether that expression is met. They are useful if you would like to compare against multiple possible outcomes.

In this article, we have discussed the fundamentals of conditional statements in JavaScript. We then explored the way to use the `switch` and `case` statements and went through an example of the way to use multiple `case` statements in an exceedingly `switch` block.

Now you've got the knowledge you need to use the JavaScript “switch case” statement like an expert! 

Enjoyed the article buy me a cup [Coffee ☕](https://www.buymeacoffee.com/lary),

Connect With me at [Twitter](https://twitter.com/larymak1) | [Insta](https://www.instagram.com/nextgencoders/) | [YouTube](https://www.youtube.com/channel/UCrT1ARRZfLOuf6nc_97eXEg) | [LinkedIn](https://www.linkedin.com/in/hillary-nyakundi)  | [GitHub](https://github.com/larymak) 

Enjoy Coding ❤