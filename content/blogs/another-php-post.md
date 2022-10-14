+++
title = "Basic syntax in PHP"
author = ["Ezequiel Cardoso"]
date = 2022-07-02T22:07:00-03:00
lastmod = 2022-10-14T19:57:47-03:00
tags = ["php"]
draft = false
weight = 2009
foo = "bar"
baz = "zoo"
alpha = 1
beta = "two words"
gamma = 10
+++

## Basic PHP syntax {#basic-php-syntax}

Although PHP is a fairly simple and very flexible language, we must take into account
It has some rules regarding its syntax and structure.

When the interpreter parses a php file, always looks for opening and closing
tags &lt;?php and ?&gt; allowing PHP to start and stop interpreting code between them.

```php
<?php
some php code...//parsed
?>
```

There are three types of tags in PHP:

```php
//NORMAL TAG
// When the document has some PHP code embedded in html.
<?php
print("hello world")
?>
//output: hello world

//If your document has only PHP code, don't use the closing tag.
<?php
$var = 1;
print $var;

//output: 1
```

```php
//THE SHORT ECHO TAG
// if you want to print something
<?="hello world" ?>
output: hello world
```

```php
//It is recomended not to be used as short tag can be disabled.
<? ?>
```


### Semicolon: {#semicolon}

All PHP commands needs to be close with a semicolon (;)

```php
$x += 10;
```

The missing semicolon at the end of a command is probably the most common cause.
frequent errors. When this happens, PHP treats multiple statements as
only one not being able to interpret them correctly and throwing a message of
parse error "Parse error".

```php
$x += 10

//Output: PHP Parse error: syntax error, unexpected end of file in Standard input code on line 3
```

PHP Parse error: syntax error, unexpected end of file in Standard input code on line 3


### The $ symbol {#the-symbol}

In PHP you must write the $ sign in front of all variables. The interpreter
PHP will recognize them regardless of whether they are numbers, arrays,
arrays etc.

```php
<?php
$myNumber = 1;
$myString = "One";
$myArray = array('one', 'two', 'three');

echo $myNumber . " " . $myString . " " . $myArray;

//: Warning: Array to string conversion in Standard input code on line 6
//: 1 One Array
```

[//]: # "Exported with love from a post written in Org mode"
[//]: # "- https://github.com/kaushalmodi/ox-hugo"
