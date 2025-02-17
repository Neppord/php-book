# Chapter 2 - Expressions

Expressions are declarative, it means that in nature they don't describe how to do things but rather what to do. A example of a expression could be a mathematical expression like `1 + 2 + 3` which is equal to 6, but even though there is an order in which someone would calculate that it is `6` the expression itself doesn't tell you in what order to do that. But using assignment statements we can force an order:

```php
<?php
$a = 2 + 3;
$b = 1 + $a;
```
In the code above we use the order of the two assignments to force the computer to calculate `2 + 3` before adding the `1`. We may also use parenthesis to force the order in an expression `1 + (2 + 3)`, this however at least philosophically is not the same thing, since it "changes" the problem given to the computer and is not a way to instruct the computer how to solve the same problem.

So even though expressions don't tell the computer what order to do tings in it sometimes doesn't have a choice and there is only one way to do it. We should for the most part trust that the computer will do its best (read "better than we can") when picking the order in how it evaluates an expression.

## Examples

Here is a list of example expressions, printed out using the echo statement from earlier.

Calculates `1 + 2 + 3`
```php
echo 1 + 2 + 3;
```

Calculates the absolute value of `-42`
```php
echo abs(-42);
```

Joins (also known as concatenates) `"hello "` with `"world"` into `"hello world"`.

```php
echo "hello " . "world";
```

Uses a boolean expression to check if `true` is true and then prints the string `"true is true"`. The `&&` is used to combine two expressions. If the thing to the left of te `&&` is truthy (evaluates to true) then it will result in what is on the right-hand side of the `&&` otherwise it will result in what it evaluated on the left-hand side.
```php
echo true && "true is true";
```

A more complete example having an expression of `15 > 10` which is true.
```php
echo 15 > 10 && "15 is larger than 10";
```

## Exercises