+++
title = "Variables in PHP"
author = ["Ezequiel Cardoso"]
date = 2022-07-04T21:15:00-03:00
lastmod = 2022-08-31T19:25:30-03:00
tags = ["php"]
draft = true
weight = 2004
foo = "bar"
baz = "zoo"
alpha = 1
beta = "two words"
gamma = 10
+++

{{< figure src="/images/Basic_PHP_Syntax.png" >}}


## Variables in PHP {#variables-in-php}


### What is a variable? {#what-is-a-variable}

A variable is something that can hold anything inside it and can modify,
replace or remove the item you are saving at any time.

We can imagine a variable as a CONTAINER that can hold any VALUE!


#### Rules for naming variables {#rules-for-naming-variables}

When creating our variables in PHP we must follow the following
four rules;

1.  Variable names, after the $ sign, must start with a
    letter of the alphabet or the character _ (underscore).
2.  Variable names can only contain the characters [a-z, A-Z,
    0-9 and _ ].
3.  Variable names cannot contain spaces. If the name has
    more than one word the character _ (underscore) must be used, eg.
    ($first_name).
4.  Variable names are case sensitive.


#### Structure of the variables {#structure-of-the-variables}

Variables in PHP always! start with a $ sign and in the example that we
occupies the quotes tells the interpreter that it is a string of
characters (string). Once the content/value is assigned to the variable $name,
If we want to see what the assigned content/value was, we can do it through
from the command echo $...;

```php
$name = "Charlie";

echo $name;
```

We could also assign the content of $name to another variable, eg $user_name

```php
<?php //test.php
$name = "Charlie";
echo $name . " ";
$user_name = $name;
echo $user_name;
?>
```


#### Numeric variables: {#numeric-variables}

Variables in PHP can also contain whole numbers (integers) and
floating point (float).

```php
$account_1 = 17;
$account_2 = 17.5;

echo $account_1 . " " . $account_2;
```


#### Matrices (Arrays) {#matrices--arrays}

We can think of arrays as a series of values ​​that share a
set. For example: a basketball team of five people share the
variable (set) equipment.

The structure of an array is composed of the constructor array('...','...'); who
inside it contains strings, each of them separated by commas.

```php
$team = array('Jose', 'Ana', 'Lorena', 'Pepe', 'Carla');
//If we wanted to know the name of player number 1 we should:
echo $team[1];
```

The reason the result shows Ana and not José is because the first
element of an array is position 0 (zero), not 1.

[//]: # "Exported with love from a post written in Org mode"
[//]: # "- https://github.com/kaushalmodi/ox-hugo"
