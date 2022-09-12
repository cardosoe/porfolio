+++
title = "Debugging in PHP"
author = ["Ezequiel Cardoso"]
date = 2022-07-01
publishDate = 2022-07-04T00:00:00-03:00
lastmod = 2022-09-11T23:04:02-03:00
tags = ["php"]
draft = false
weight = 2002
foo = "bar"
baz = "zoo"
alpha = 1
beta = "two words"
gamma = 10
+++

{{< figure src="/images/Basic_PHP_Syntax.png" >}}


## DEBUGGING {#debugging}

Definition: Debugging is the process of detecting and removing of existing and
potential errors (also called as ‘bugs’) in a software code that can cause it to
behave unexpectedly or crash. To prevent incorrect operation of a software or
system, debugging is used to find and resolve bugs or defects. When various
subsystems or modules are tightly coupled, debugging becomes harder as any
change in one module may cause more bugs to appear in another. Sometimes it
takes more time to debug a program than to code it.Definition: Debugging is the
process of detecting and removing of existing and potential errors (also called
as ‘bugs’) in a software code that can cause it to behave unexpectedly or crash.
To prevent incorrect operation of a software or system, debugging is used to
find and resolve bugs or defects. When various subsystems or modules are tightly
coupled, debugging becomes harder as any change in one module may cause more
bugs to appear in another. Sometimes it takes more time to debug a program than
to code it.


## To debug php offers us two methods: {#to-debug-php-offers-us-two-methods}

1.  var_dump($...);

<!--listend-->

```php
$people = [
"Charles" => 22,
"Mr. Michi" => 15,
"John" => 65
];

var_dump($people);

 #+RESULTS:
: array(3) {
: ["Charles"]=>
:int(22)
: ["Mr.Michi"]=>
:int(15)
: ["John"]=>
:int(65)
: }
```

var_dump allows me to inspect the entire content of my variable

1.  print_r($...)

<!--listend-->

```php
$people = [
"Charles" => 22,
"Mr. Michi" => 15,
"John" => 65
];

print_r ($people);


#+RESULTS:
: array
: (
: [Charles] => 22
: [Mr. Michi] => 15
: [John] => 65
: )
```

print_r is also good for inspection but it doesn't give me as much information as var_dump.

-   To do debugging php offers us two methods:
-   var_dump($...);

<!--listend-->

```php
$people = [
"Charles" => 22,
"Mr. Michi" => 15,
"John" => 65
];

var_dump($people);

#+RESULTS:
: array(3) {
: ["Charles"]=>
:int(22)
: ["Mr.Michi"]=>
:int(15)
: ["John"]=>
:int(65)
: }
```

var_dump allows me to inspect the entire content of my variable

1.  print_r($...)

<!--listend-->

```php
$people = [
"Charles" => 22,
"Mr. Michi" => 15,
"John" => 65
];

print_r ($people);

#+RESULTS:
: array
: (
: [Charles] => 22
: [Mr. Michi] => 15
: [John] => 65
: )
```

print_r is also good for inspection but it doesn't give me as much information
as var_dump.

[//]: # "Exported with love from a post written in Org mode"
[//]: # "- https://github.com/kaushalmodi/ox-hugo"
