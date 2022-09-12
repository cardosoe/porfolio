+++
title = "Relational Operators in PHP"
author = ["Ezequiel Cardoso"]
date = 2022-07-02
publishDate = 2022-07-19T00:00:00-03:00
lastmod = 2022-09-11T23:04:03-03:00
tags = ["php"]
draft = false
weight = 2007
foo = "bar"
baz = "zoo"
alpha = 1
beta = "two words"
gamma = 10
+++

{{< figure src="/images/Basic_PHP_Syntax.png" >}}


## RELATIONAL OPERATORS {#relational-operators}

These operators help us compare two values.


### OPERATOR == EQUAL {#operator-equal}

DOES NOT COMPARE TYPES OF DATA

```php

$a = 5;
$b = 5;
$b2 = "5";
$c = 9;
$d = 2;

var_dump( $a == $b ); //We ask PHP if $a is equal == to $b
```


### OPERATOR `==` IDENTICAL {#operator-identical}

IF YOU COMPARE TYPES OF DATA

```php

$a = 5;
$b = 5;
$b2 = "5";
$c = 9;
$d = 2;

var_dump( $a === $b ); //We ask PHP if $a is identical == to $b
var_dump( $a === $b2 ); //We ask PHP if $a is identical == to $b2
```


### OPERATOR != (!=) DIFFERENT {#operator-----different}

DOES NOT COMPARE TYPES OF DATA

```php

$a = 5;
$b = 5;
$b2 = "5";
$c = 9;
$d = 2;

var_dump( $a != $b ); //Ask PHP if $a is different == to $b
var_dump( $a != $b2 ); //Ask PHP if $a is different == to $b2
```


### OPERATOR !== (! ==) DIFFERENT {#operator-----different}

IF YOU COMPARE TYPES OF DATA

```php

$a = 5;
$b = 5;
$b2 = "5";
$c = 9;
$d = 2;

var_dump( $a !== $b ); //Ask PHP if $a is different == to $b
var_dump( $a !== $b2 ); //Ask PHP if $a is different == to $b2
```


### OPERATOR &lt; LESS THAN {#operator-less-than}

```php

$a = 5;
$b = 5;
$b2 = "5";
$c = 9;
$d = 2;

var_dump( $a < $b );
var_dump( $c < $b );
var_dump( $d < $b );
```


### OPERATOR &gt; GREATER THAN {#operator-greater-than}

```php

$a = 5;
$b = 5;
$b2 = "5";
$c = 9;
$d = 2;

var_dump( $a > $b );
var_dump( $c > $b );
var_dump( $d > $b );
```


### OPERATOR &gt;= GREATER OR EQUAL TO {#operator-greater-or-equal-to}

```php

$a = 5;
$b = 5;
$b2 = "5";
$c = 9;
$d = 2;

var_dump( $a >= $b );
var_dump( $c >= $b );
var_dump( $d >= $b );
```


### OPERATOR &lt;= LESS OR EQUAL TO {#operator-less-or-equal-to}

```php

$a = 5;
$b = 5;
$b2 = "5";
$c = 9;
$d = 2;

var_dump( $a <= $b );
var_dump( $c <= $b );
var_dump( $d <= $b );
```


### OPERATOR &lt;=&gt; (&lt; = &gt;) SPACESHIP {#operator-----spaceship}

The operator:

1.  It will return 0 if the numbers are equal.
2.  It will return 1 if the number on the left is greater than the one on
    It's on the right.
3.  It will return -1 if the number on the left is less than

the one on the right.

```php

$a = 5;
$b = 5;
$b2 = "5";
$c = 9;
$d = 2;

var_dump( $a <=> $b );
var_dump( $c <=> $b );
var_dump( $d <=> $b );
```

:int(0)
:int(1)
:int(-1)
:int(-1)


### OPERATOR ?? NULL MERGE {#operator-null-merge}

This operator tells us what is the first variable that is defined.

```php

$a = 5;
$b = 5;
$b2 = "5";
$c = 9;
$d = 2;

var_dump( $a ?? $b );
var_dump( $c ?? $b );
var_dump( $d ?? $b );
```

:int(5)
:int(9)
:int(2)

[//]: # "Exported with love from a post written in Org mode"
[//]: # "- https://github.com/kaushalmodi/ox-hugo"
