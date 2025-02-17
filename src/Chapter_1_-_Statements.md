# Chapter 1 - Statements

## Procedural 
Php is a procedural language, this is in contrast to a declarative language. Procedural in this context means that when you write Php code you tell the php program what to do __in what order__.

The building blocks that are order sensitive we call statements, and are often ended with a semicolon `;` or by a code-block denoted by curly brackets `{}`.

In english we could have a "program" that describes how to wash the dishes.

- Fill sink with warm soapy water.
- Clean dishes.
- Replace soapy water with clean water.
- Rinse dishes
- Place dishes on a rack to dry.

These "statements" are instructions to the reader of how to clean dishes and the order matter, it describes the procedure.

## Php

The statements above only work for us humans, the php language has a much stricter set of statements that it understands, though order still matters.

Here are some different types of statements:

An echo statement, telling php to write "hello".
```php
echo "hello";
```

An if statement, with an echo statement in side of it.
```php
if (true) echo "world";  
```

An assignment statement, assigning the value of `42` to the variable named `$x` or `x` for short.
```php
$x = 42;
```

A foreach statement, with a code block, echoing the numbers 1 to 10.
```php
foreach (range(1, 10) as $number) {
    echo "$number\n";
}
```

## Exercises

### Echo your name

Start by creating a phpfile `echo_my_name.php`
```php
<?php
echo "My name here\n";
```
run it to make sure that it writes "My name here". After that change the text to your name, and make sure that it now prints your name instead of "My name here".

### Echo your initials

Copy the file from last exercise and call it `echo_my_initials.php`.

Change the echo statement to instead print out `#` and ` ` to create large letters.
Bellow is an example of printing an A
```php
<?php
echo " # \n";
echo "# #\n";
echo "###\n";
echo "# #\n";
echo "# #\n";
```
Using this technique, print your initials. Try to make it look good by adding other signs then letters, maybe a smiley. Try to figure out what `\n` on the end means, what happens if you remove it. 



