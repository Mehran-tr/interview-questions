# PHP Interview question

Hello , In this repository I add interview questions about PHP programming language I found on internet. I have

if you found these questions usefull click on Star 

You are very welcomed if You want to Contribute 🥳










**************************************************************************************************************************************



### Q. ***What does PEAR stand for?***

PEAR means “PHP Extension and Application Repository”. It extends PHP and provides a higher level of programming for web developers.


### Q. ***Is multiple inheritance supported in PHP?***

PHP supports only single inheritance; it means that a class can be extended from only one single class using the keyword ‘extended’.

### Q. ***What is the meaning of a final class and a final method?***

final’ is introduced in PHP5. Final class means that this class cannot be extended and a final method cannot be overridden.


### Q. ***How is the comparison of objects done in PHP?***

We use the operator ‘==’ to test is two objects are instanced from the same class and have same attributes and equal values. We can test if two objects are referring to the same instance of the same class by the use of the identity operator ‘===’.

### Q. ***How failures in execution are handled with include() and require() functions?***

If the function require() cannot access the file then it ends with a fatal error. However, the include() function gives a warning, and the PHP script continues to execute.

### Q. ***What is the main difference between require() and require_once()?***

require(), and require_once() perform the same task except that the second function checks if the PHP script is already included or not before executing it.
(same for include_once() and include())

### Q. ***How can we display information of a variable and readable by a human with PHP?***

To be able to display a human-readable result we use print_r().

### Q. ***What does the PHP error ‘Parse error in PHP – unexpected T_variable at line x’ means?***

This is a PHP syntax error expressing that a mistake at the line x stops parsing and executing the program

### Q. ***How can we check the value of a given variable is a number?***

It is possible to use the dedicated function, is_numeric() to check whether it is a number or not.

### Q. ***Is it possible to remove the HTML tags from data?***

The strip_tags() function enables us to clean a string from the HTML tags.

### Q. ***what is the static variable in function useful for?***

A static variable is defined within a function only the first time, and its value can be modified during function

### Q. ***What is the most convenient hashing method to be used to hash passwords?***

It is preferable to use crypt() which natively supports several hashing algorithms or the function hash() which supports more variants than crypt() rather than using the common hashing algorithms such as md5, sha1 or sha256 because they are conceived to be fast. Hence, hashing passwords with these algorithms can create vulnerability.

### Q. ***How can you pass a variable by reference?***

To be able to pass a variable by reference, we use an ampersand in front of it, as follows $var1 = &$var2

### Q. ***How is it possible to cast types in PHP?***

The name of the output type has to be specified in parentheses before the variable which is to be cast as follows:
* (int), (integer) – cast to integer
* (bool), (boolean) – cast to boolean
* (float), (double), (real) – cast to float
* (string) – cast to string
* (array) – cast to array
* (object) – cast to object


### Q. ***What is the function func_num_args() used for?***

The function func_num_args() is used to give the number of parameters passed into a function.


### Q. ***If the variable $var1 is set to 10 and the $var2 is set to the character var1, what’s the value of $$var2?***

$$var2 contains the value 10.

### Q. ***What does accessing  a class via :: means?***

:: is used to access static methods that do not require object initialization.

### Q. ***In PHP, objects are they passed by value or by reference?***

In PHP, objects are passed by reference.

### Q. ***What’s the difference between __sleep and __wakeup?***

__sleep() returns the array of all the variables that need to be saved, while __wakeup() retrieves them.

### Q. ***What is faster?***

1- Combining two variables as follows:
$variable1 = 'Hello ';

$variable2 = 'World';

$variable3 = $variable1.$variable2;
Or
2- $variable3 = "$variable1$variable2";
$variable3 will contain “Hello World”. The first code is faster than the second code especially for large large sets of data.

### Q. ***What does $GLOBALS mean?***

$GLOBALS is associative array including references to all variables which are currently defined in the global scope of the script.

### Q. ***What does $_SERVER mean?***

$_SERVER is an array including information created by the web server such as paths, headers, and script locations.

### Q. ***What does $_FILES means?***

$_FILES is an associative array composed of items sent to the current script via the HTTP POST method.

### Q. ***What does $_ENV mean?***

$_ENV is an associative array of variables sent to the current PHP script via the environment method.

### Q. ***What are PHP Scopes?***

*Variable Scopes: The scope of a variable is defined as its extent in the program within which it can be accessed, i.e. the scope of a variable is the portion of the program within which it is visible or can be accessed. Depending on the scopes, PHP has three variable scopes.
*Local variables: The variables declared within a function are called local variables to that function and have their scope only in that particular function. In simple words, it cannot be accessed outside that function. Any declaration of a variable outside the function with the same name as that of the one within the function is a completely different variable. For now, consider a function as a block of statements.

### Q. ***What does the array operator ‘===’ means?***

$a === $b TRUE if $a and $b have the same key/value pairs in the same order and of the same types.

### Q. ***What is the differences between $a != $b and $a !== $b?***

!= means inequality (TRUE if $a is not equal to $b) and !== means non-identity (TRUE if $a is not identical to $b).

### Q. ***What is the difference between the functions strstr() and stristr()?***

The string function strstr(string allString, string occ) returns part of allString from the first occurrence of occ to the end of allString. This function is case-sensitive. stristr() is identical to strstr() except that it is case insensitive.

### Q. ***What is the difference between “echo” and “print” in PHP?***

The main difference between echo and print in PHP are given below:

* echo can output one or more strings.
* print can only output one string and it always returns 1.
* echo is faster than print because it does not return any value.
* print is slower compared to echo.
If you want to pass more than one parameter to echo, a parenthesis should be used.
Use of parenthesis is not required with the argument list.

### Q. ***What is the purpose of @ in PHP?***

In PHP, @ is used for suppressing(stop) error messages. If any runtime error occurs on the line which consists @ symbol at the beginning, then the error will be handled by PHP.

### Q. ***Explain the main types of errors.***

The 3 main types of errors in PHP are:

* Notices: Notices are non-critical errors that can occur during the execution of the script. These are not visible to users. Example: Accessing an undefined variable.
* Warnings: These are more critical than notices. Warnings don’t interrupt the script execution. By default, these are visible to the user. Example: include() a file that doesn’t exist.
* Fatal: This is the most critical error type which, when occurs, immediately terminates the execution of the script. Example: Accessing a property of a non-existent object or require() a non-existent file.

### Q. ***What are traits?***

Traits are a mechanism that lets you create reusable code in PHP and similar languages where multiple inheritances are not supported. It’s not possible to instantiate it on its own.
A trait is intended to reduce the limitations of single inheritance by enabling a developer to reuse sets of methods freely in many independent classes living in different hierarchies of class

### Q. ***Explain Path Traversal***

Path traversal is a form of attack to read into the files of a web application. '../' (dot-dot-sequences) is a cross-platform symbol to go up in the directory. Path traversal makes use of this symbol to operate the web application file. The attacker can reveal the content of the file attacked using the path traversal outside the root directory of a web server or application. It is usually done to gain access to secret passwords, tokens, and other sensitive information stored in the files.
Path Traversal is also called “Directory Traversal”. It allows the attacker to exploit vulnerabilities present in the web file under attack.
Let’s take a simple example. Consider we have a “Show File” button that opens up some URL.
For a classic directory traversal attack, the attacker may try to access the system file /etc/passwd (assuming a UNIX/LINUX system). If the application receives the value of the file parameter from the URL and passes it to a system call, it would traverse the relative path ../../etc/passwd starting from /var/www and ask the system to load the password file.
This technique is also called a dot-dot-slash attack, because it usually uses the special characters ../ (or \.. on Windows) to climb to a higher-level directory

### Q. ***What is use of Spaceship Operator?***

This <=> operator will offer combined comparison in that it will:
* Return 0 if values on both side are equal
* Return 1 if value on the left is greater
* Return -1 if the value on the right is greater

### Q. ***Is PHP single or multi threaded?***

PHP is not single threaded by nature. It is, however, the case that the most common installation of PHP on unix systems is a single threaded setup, as is the most common Apache installation, and nginx doesn't have a thread based architecture whatever. In the most common Windows setup and some more advanced unix setups, PHP can and does operate multiple interpreter threads in one process.
PHP as an interpreter had support for multi-threading since the year 2000.

### Q. ***When should I use require_once vs require?***

* The require_once() statement is identical to require() except PHP will check if the file has already been included, and if so, not include (require) it again.

* Using require or include instead implies that your code is not reusable elsewhere, i.e. that the scripts you're pulling in actually execute code instead of making available a class or some function libraries.

### Q. ***When should I use 'self' over '$this'?***

Use $this to refer to the current object. Use self to refer to the current class. In other words, use $this->member for non-static members, use self::$member for static members.

### Q. ***What are startsWith() and endsWith() functions in PHP?***

PHP 8.0 and higher
Since PHP 8.0 you can use the
* str_starts_with — Checks if a string starts with a given substring
* str_starts_with Manual and
* str_ends_with — Checks if a string ends with a given substring
* str_ends_with Manual
Example
echo str_starts_with($str, '|');


### Q. ***What is StdClass use for?***

stdClass is PHP's generic empty class, kind of like Object in Java or object in Python (Edit: but not actually used as universal base class; thanks @Ciaran for pointing this out).
It is useful for anonymous objects, dynamic properties, etc.
An easy way to consider the StdClass is as an alternative to associative array. See this example below that shows how json_decode() allows to get an StdClass instance or an associative array. Also but not shown in this example, SoapClient::__soapCall returns an StdClass instance.

### Q. ***htmlentities() vs. htmlspecialchars()***

This function is identical to htmlspecialchars() in all ways, except with htmlentities(), all characters which have HTML character entity equivalents are translated into these entities.

Certain characters have special significance in HTML, and should be represented by HTML entities if they are to preserve their meanings. This function returns a string with some of these conversions made; the translations made are those most useful for everyday web programming. If you require all HTML character entities to be translated, use htmlentities() instead.
The difference is what gets encoded. The choices are everything (entities) or "special" characters, like ampersand, double and single quotes, less than, and greater than (specialchars).
I prefer to use htmlspecialchars whenever possible.

### Q. ***Why should use static method?***

When you use static, this is to call a function without an instance of the class. The main reason is often to represent a service class which should not be instantiated many times.

### Q. ***Why should use static method?***

I will give you 3 solutions (from the worst to the best) to achieve that:

Static

A static class (with only static functions) prevent you from using many OOP features like inheritance, interface implementation. If you really think of what is a static function, it is a function namespaced by the name of its class. You already have namespaces in PHP, so why add another layer?
Another big disadvantage is that you cannot define clear dependencies with your static class and the classes using it which is a bad thing for maintenability and scalability of your application.

Singleton

A singleton is a way to force a class to have only one instance:
```php
<?php

class Singleton {
    // Unique instance.
    private static $instance = null;

    // Private constructor prevent you from instancing the class with "new".
    private function __construct() {  
    }

    // Method to get the unique instance.
    public static function getInstance() {
        // Create the instance if it does not exist.
        if (!isset(self::$instance)) {
            self::$instance = new Singleton();  
        }

        // Return the unique instance.
        return self::$instance;
    }
}
```
It is a better way because you can use inheritance, interfaces and your method will be called on an instanciated object. This means you can define contracts and use low coupling with the classes using it. However some people consider the singleton as an anti pattern especially because if you want to have 2 or more instances of your class with different input properties (like the classic example of the connection to 2 different databases) you cannot without a big refactoring of all your code using the singleton.

Service

A service is an instance of a standard class. It is a way to rationalize your code. This kind of architecture is called SOA (service oriented architecture). I give you an example:
If you want to add a method to sell a product in a store to a consumer and you have classes Product, Store and Consumer. Where should you instantiate this method? I can guarantee that if you think it is more logical in one of these three class today it could be anything else tomorrow. This leads to lots of duplications and a difficulty to find where is the code you are looking for. Instead, you can use a service class like a SaleHandler for example which will know how to manipulate your data classes.
It is a good idea to use a framework helping you to inject them into each others (dependency injection) in order to use them at their full potential. In the PHP community, you have a nice example of implementation of this in Symfony for instance.

To sum up:

If you do not have a framework, singletons are certainly an option even if I personally prefer a simple file where I make manual dependency injection.


If you have a framework, use its dependency injection feature to do that kind of thing.


You should not use static method (in OOP). If you need a static method in one of your class, this means you can create a new singleton/service containing this method and inject it to the instance of classes needing it.



### Q. ***PHP - Access Modifiers***

* public - the property or method can be accessed from everywhere. This is default
* protected - the property or method can be accessed within the class and by classes derived from that class
* private - the property or method can ONLY be accessed within the class

### Q. ***PHP - What are Traits?***

PHP only supports single inheritance: a child class can inherit only from one single parent.
So, what if a class needs to inherit multiple behaviors? OOP traits solve this problem.
Traits are used to declare methods that can be used in multiple classes. Traits can have methods and abstract methods that can be used in multiple classes, and the methods can have any access modifier (public, private, or protected).
Traits are declared with the trait keyword

### Q. ***PHP Namespaces***

Namespaces are qualifiers that solve two different problems:
* They allow for better organization by grouping classes that work together to perform a task
* They allow the same name to be used for more than one class
For example, you may have a set of classes which describe an HTML table, such as Table, Row and Cell while also having another set of classes to describe furniture, such as Table, Chair and Bed. Namespaces can be used to organize the classes into two different groups while also preventing the two classes Table and Table from being mixed up.

### Q. ***PHP - What is an Iterable?***

An iterable is any value which can be looped through with a foreach() loop.

The iterable pseudo-type was introduced in PHP 7.1, and it can be used as a data type for function arguments and function return values.

####PHP - Using Iterables

The iterable keyword can be used as a data type of a function argument or as the return type of a function


### Q. ***What is function overloading?***

* Function overloading is the ability to create multiple functions of the same name with different implementations.
* Function overloading in PHP?
* Function overloading in PHP is used to dynamically create properties and methods. These dynamic entities are processed by magic methods which can be used in a class for various action types. Function overloading contains same function name and that function preforms different task according to number of arguments. For example, find the area of certain shapes where radius are given then it should return area of circle if height and width are given then it should give area of rectangle and others. Like other OOP languages function overloading can not be done by native approach. In PHP function overloading is done with the help of magic function __call(). This function takes function name and arguments.

Property and Rules of overloading in PHP:

* All overloading methods must be defined as Public.
* After creating the object for a class, we can access a set of entities that are properties or methods not defined within the scope of the class.
* Such entities are said to be overloaded properties or methods, and the process is called as overloading.
* For working with these overloaded properties or functions, PHP magic methods are used.
* Most of the magic methods will be triggered in object context except __callStatic() method which is used in a static context.

Types of Overloading in PHP: There are two types of overloading in PHP.
* Property Overloading
* Method Overloading

Property Overloading: PHP property overloading is used to create dynamic properties in the object context. For creating these properties no separate line of code is needed. A property associated with a class instance, and if it is not declared within the scope of the class, it is considered as overloaded property.

Following operations are performed with overloaded properties in PHP.

* Setting and getting overloaded properties.
* Evaluating overloaded properties setting.
* Undo such properties setting.

Before performing the operations, we should define appropriate magic methods. which are,

* __set(): triggered while initializing overloaded properties.
* __get(): triggered while using overloaded properties with PHP print statements.
* __isset(): This magic method is invoked when we check overloaded properties with isset() function
* __unset(): Similarly, this function will be invoked on using PHP unset() for overloaded properties.


