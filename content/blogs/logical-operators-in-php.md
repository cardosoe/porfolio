+++
title = "Logical Operators in PHP"
author = ["Ezequiel Cardoso"]
date = 2022-07-08T19:16:00-03:00
lastmod = 2022-08-31T19:25:31-03:00
tags = ["php"]
draft = true
weight = 2010
foo = "bar"
baz = "zoo"
alpha = 1
beta = "two words"
gamma = 10
+++

{{< figure src="/images/Basic_PHP_Syntax.png" >}}


## LOGICAL OPERATORS IN PHP {#logical-operators-in-php}

Logical operators help us combine two or more statements in order
determine if a sentence is true or false. In most cases it
they need at least two statements and an operator.

To determine the truth of an expression we will use the so-called
"TRUTH TABLES".

Truth tables in logic are a tool represented in graphics
of rows and columns showing all possible scenarios and conditions
for a statement to be true or false.


### TYPES OF OPERATOR {#types-of-operator}


#### AND {#and}

It is used to check if two statements are true.
If both are true, then the entire sentence is true.
If one of them is false, then the entire sentence is false.
In PHP we can use them as follows:

<!--list-separator-->

-  $value_1 and $value_2

<!--list-separator-->

-  $value_1 &amp;&amp; $value_2

<!--list-separator-->

-  TRUTH TABLES

    | Value 1 | Operator | Value 2 | Result |
    |---------|----------|---------|--------|
    | True    | AND      | True    | True   |
    | True    | AND      | False   | False  |
    | False   | AND      | True    | False  |
    | False   | AND      | False   | False  |


#### OR {#or}

It is used to check if at least one of the statements is true.
If one is true, the sentence is true. If it is not, the sentence is false.
In PHP we can use them as follows:

<!--list-separator-->

-  $value_1 or $value_2

<!--list-separator-->

-  $value_1 || $value_2

<!--list-separator-->

-  TRUTH TABLES

    | Value 1 | Operator | Value 2 | Result |
    |---------|----------|---------|--------|
    | True    | OR       | True    | True   |
    | True    | OR       | False   | True   |
    | False   | OR       | True    | True   |
    | False   | OR       | False   | False  |


#### NOT {#not}

It is used to invert the value of an assertion.
In PHP we can use them as follows:

<!--list-separator-->

-  !$value

<!--list-separator-->

-  TRUTH TABLES

    | Operator | Value | Result |
    |----------|-------|--------|
    | NOT      | True  | False  |
    | NOT      | False | True   |


#### EXERCISE {#exercise}

```php

// define the variables
$michis_felines = true;
$michis_4_patas = true;
$michis_fly = false;
$michis_programan_con_PHP = false;

// Now we are going to do the operations with AND

var_dump($michis_felines && $michis_4_patas);

// with OR
var_dump($michis_fly || $michis_4_patas);

// NOT

var_dump( !$michis_4_legs );

// Exercise

$result = $michis_4_patas and $michis_programan_con_PHP;

var_dump( $result );
```

```php

$is_a_big_michi = true;
$he_likes_to_eat = true;
$knows_fly = false;
$has_2_legs = false;

var_dump($he_is_a_big_michi && $he_likes_to_eat); // True
var_dump($is_a_big_michi || $knows_fly); // True
var_dump($can_fly || $has_2_legs); //False
var_dump(!$he_likes_to_eat); //False
var_dump(!$he_likes_to_eat || $he_is_a_big_michi); // True
```

[//]: # "Exported with love from a post written in Org mode"
[//]: # "- https://github.com/kaushalmodi/ox-hugo"
