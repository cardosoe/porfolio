+++
title = "Constants in PHP"
author = ["Ezequiel Cardoso"]
date = 2022-07-06T18:37:00-03:00
lastmod = 2022-08-31T19:25:30-03:00
tags = ["php"]
draft = true
weight = 2006
foo = "bar"
baz = "zoo"
alpha = 1
beta = "two words"
gamma = 10
+++

{{< figure src="/images/Basic_PHP_Syntax.png" >}}


## CONSTANTS IN PHP {#constants-in-php}


### What is a constant {#what-is-a-constant}

A constant is an indicator for a single value. Unlike variables, constants cannot change a value once it has been assigned.
By default, a constant is case sensitive. By convention,
IDENTIFIERS OF CONSTANTS ARE ALWAYS DECLARED IN UPPERCASE.

A constant will always keep its value intact from the moment it is declared.


### Constants are always declared in uppercase. {#constants-are-always-declared-in-uppercase-dot}

For example, if we declare the constant "PI_NUMBER", the result will be the assigned value.

```php

define("PI_NUMBER", 3.14);

echo PI_NUMBER;
```

But if we try to declare the same constant again, the interpreter will throw the following error along with the originally assigned value.

```php

define("PI_NUMBER", 3.14);
define("PI_NUMBER", 14);
echo PI_NUMBER;
```

[//]: # "Exported with love from a post written in Org mode"
[//]: # "- https://github.com/kaushalmodi/ox-hugo"
