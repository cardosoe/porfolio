+++
title = "Data type in PHP"
author = ["Ezequiel Cardoso"]
date = 2022-07-02
publishDate = 2022-07-12T00:00:00-03:00
lastmod = 2022-09-11T23:10:03-03:00
tags = ["php"]
draft = false
weight = 2005
foo = "bar"
baz = "zoo"
alpha = 1
beta = "two words"
gamma = 10
+++

{{< figure src="/images/Basic_PHP_Syntax.png" >}}


## Data Types in PHP {#data-types-in-php}

A data type is simply a way of differentiating data by across
its type for example: letters, numbers, words, etc...

PHP being a weakly typed language does not need you to explicitly define
a data type since by itself it can deduce what type you are using.


### Numeric: {#numeric}


#### Integer (integers) {#integer--integers}


#### Float (decimal) {#float--decimal}


#### Double (more precise decimal, with more number of decimals). {#double--more-precise-decimal-with-more-number-of-decimals--dot}


### Character string: {#character-string}


#### Char (character) {#char--character}


#### String (character string) {#string--character-string}


### Worthless: {#worthless}


#### Null (no value inside) {#null--no-value-inside}


#### Undefined (there is a variable defined but without a determined value) {#undefined--there-is-a-variable-defined-but-without-a-determined-value}


#### If the interpreter finds two different variables, it will automatically interpret which data type it should work with. {#if-the-interpreter-finds-two-different-variables-it-will-automatically-interpret-which-data-type-it-should-work-with-dot}

```php

<?php

    $number = "23";
    $new_number = $number + 2;

    var_dump($little number);
    var_dump($new_number);
    echo "\n";
```

:int(25)

```php

$number = 10;
$number = $number + 0.5;
var_dump($little number);
```

```php

$potatoes = "10 potatoes in the sack";
$how many_potatoes_are there = $potatoes + 5;

echo $how many_potatoes_are there;
```

[//]: # "Exported with love from a post written in Org mode"
[//]: # "- https://github.com/kaushalmodi/ox-hugo"
