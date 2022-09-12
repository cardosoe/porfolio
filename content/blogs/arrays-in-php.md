+++
title = "Arrays in PHP"
author = ["Ezequiel Cardoso"]
date = 2022-07-02
publishDate = 2022-07-23T00:00:00-03:00
lastmod = 2022-09-11T23:10:04-03:00
tags = ["php"]
draft = false
weight = 2009
foo = "bar"
baz = "zoo"
alpha = 1
beta = "two words"
gamma = 10
+++

{{< figure src="/images/Basic_PHP_Syntax.png" >}}


## ARRANGEMENTS IN PHP (ARRAYS) {#arrangements-in-php--arrays}

An array is a variable that can hold multiple values at once.

Let's look at two ways to declare an array:

Declaring values inside square brackets [ ]

```php

$ages = [20, 18, 40];

echo "One of the ages is " . $ages[1] . " " . "years";
```

Declaring the values inside the array() function

```php

$ages = array(20,18,40);

echo "One of the ages is " . $ages[1] . " " . "years";
```


### ASSOCIATIVE ARRANGEMENTS {#associative-arrangements}

A variable can hold multiple values ​​that we can access them by
through a word. They are the equivalent of JSON in JavaScript and are very useful
to create lists.

```php

$ages = array(
   "Charles" => 20,
   "Mr. Michi" => 18,
   "John" => 40, //trailing comma. It is optional and PHP will not throw an error.
    );

echo "Mr. Michi's age is " . $ages["Mr. Michi"];
```

```php

$coffees = array(
   "Cappuccino" => 50,
   "Latte" => 49,
   "American" => 70
echo "The price of American coffee is {$cafes['Americano']}";
```


### NESTED ARRANGEMENTS {#nested-arrangements}

```php

$people = array(
    "Charles" => array(
        "age"=> 20,
        "surname" => "Santana",
        )
    );

echo "Carlos' information is: Age: " . $people["Charles"]["age"]. ", " . "Surname: " . $people["Carlos"]["surname"];
```


## ARRAY MANIPULATION {#array-manipulation}

PHP has tons of functions for manipulating arrays (see documentation for
PHP) [PHP documentation for array manipulation]()

```php

    $ages = [18, 22,40, 34];

    //count
    echo count($ages);
    //output = 4
```

```php
//array_push
    $ages = [18, 22,40, 34];
    array_push($ages, 13);

    var_dump($ages);
```

```php
//is_array
    $ages = [18, 22,40, 34];
    $this_is_not_an_array = "";
    var_dump( is_array($this_is_not_an_array)); //bool(false)
    var_dump( is_array($ages)); //bool(true)
```

```php
//Explore
    $list_of_fruits = "strawberry, cherry, apple";
    $list_of_fruits_array = explode(",", $list_of_fruits);
    var_dump($list_of_fruits_array);
```

```php
// Implode is used to join through a concatenator, in this case the comma.
    $list_of_fruits_array = ["strawberry", "cherry", "apple"];
    $list_of_fruits = implode(",", $list_of_fruits_array);
    var_dump($list_of_fruits);
```

```php

$michis = array(
    array(
        "name"=> "toto",
        "occupation" => "scratcher",
        "color" => "brown",
        "food" => array(
        "favourite" => "mackerel",
        "hated" => "cat")
        ),
    array(
        "name"=> "tat",
        "occupation" => "scratcher",
        "color" => "blue",
        "food" => array(
        "favourite" => "sardine",
        "hated" => "cat")
        ),
    array(
        "name"=> "uncle",
        "occupation" => "scratcher",
        "color" => "brown",
        "food" => array(
        "favourite" => "fish",
        "hated" => "cat")
        ),
    );

//var_dump($michis);
 // echo "michi_1's name is" . " " . $michis["michi_1"]["name"] . "," . " " . "his occupation is" . " " . $michis["michi_1"]["occupation"] . "," . " " . "its color is" . " " . $michis["michi_1"]["color"]. "," . " " . "Her favorite food is" . " " . $michis["michi_1"]["food"]["favorite"]. "," . " " . "and his hated food is". " " . $michis["michi_1"]["food"]["hated"]. ".";


    // we can access the properties of an array by declaring a variable with the subscript we want to access, followed by the values ​​we want to know
   $tito = $michis[2];
   echo "Tito's favorite food is " . $tito['food']['favorite'];
   echo "\n"; // line break
    // or we can access it directly by declaring the desired subscript followed by the values ​​we want to access.
   echo "Tato's favorite food is " . $michis[1]['food']['favorite'] . "and his favorite color is". $michis[1]['color'];
```

[//]: # "Exported with love from a post written in Org mode"
[//]: # "- https://github.com/kaushalmodi/ox-hugo"
