+++
title = "Other Operators in PHP"
author = ["Ezequiel Cardoso"]
date = 2022-07-10T10:10:00-03:00
lastmod = 2022-08-31T19:25:32-03:00
tags = ["php"]
draft = true
weight = 2013
foo = "bar"
baz = "zoo"
alpha = 1
beta = "two words"
gamma = 10
+++

{{< figure src="/images/Basic_PHP_Syntax.png" >}}


## OTHER OPERATORS IN PHP {#other-operators-in-php}


### ASSIGNMENT OPERATOR {#assignment-operator}

This operator resembles the variable that is to the left of the sign
equals ( = ) to anything to the right of the equals sign ( = ).

```php

$age_of_jaimito = ($age_of_pepito = 18) + 5;

echo "Jumpy's age is $Jumpy's_age" . " Y " . "Jaimito's age is $jaimito_age.";
```


### INCREMENT OPERATOR ++ {#increment-operator-plus-plus}

This operator increments the value of the initialized variable to the right of the = sign.

```php

$counter = 2;
$counter ++;

echo $counter;
```


### CONCATENATION OPERATOR {#concatenation-operator}

This operator concatenates the value of the initialized variable together with what is declared to the right of the = sign.

```php

$name = "Pepe";
$name .= " " . "leaks"; // Very important the . (dot) to concatenate the name before the = sign

echo $name;
```

[//]: # "Exported with love from a post written in Org mode"
[//]: # "- https://github.com/kaushalmodi/ox-hugo"
