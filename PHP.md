# PHP Coding Guidelines

We mostly complain the [PSR-2 coding style guide](http://www.php-fig.org/psr/psr-2/) (have a read).

## 1. Naming conventions
### 1.1 Usefull names
We ever use full self explaining names for variables, constants, class- and method names etc.

**Do:**
````php
$calculationResult = 0;
$counter = 0;

public function calculateResult()
{
    // Do things
}
````

**Don't:**
````php
$cRes = 0;
$cnt = 0;

public function calcRes()
{
    // Do things
}
````

### 1.2 Booleans
For booleans we prefix variables with `is` `has` `can` verbs.

````php
$isAuthorized = false;
$canVote = false;
````

### 1.3 Filenames
Filenames equals the classnames `FooBarCalculation.php` equals `class FooBarCalculation { }`

## 2. Curly braces
We place curly braces in every case on the next line.


**Classes**
````php
class FileAdapter extends Adapter implements AdapterInterface
{
    // Do things
}
````

**If-Else**

````php
// Comment A
if ( $a === $b )
{
    // Do things
}
// Comment B
else
{
    // Do other things
}
````

**For-Each**
````php
foreach ( $items as $item )
{
    // Do things
}
````

**Closures**
````php
$myClosureResult = function ( $item ) use ( $anotherItem )
{
    // Do things
}
````

## 3. Use Statements
We use classes always with the `use` statement at the top of the file.

**Do:**
````php
use \Foo\Foobar;

...

$instance = new Foobar();
````

**Don't:**
````php
$instance = new \Foo\Foobar();
````

## 4. Method visibility
We always set the method visibility in a classes.

**Do:**
````php
public function calculateResult()
{
    // Do things
}

private function getValueItem()
{
    // We don't prefix private methods with _
}
````

**Don't:**
````php
function calculateResult()
{
    // Do things
}

private function _getValueItem()
{
    // We don't prefix private methods with _
}
````

## 5. Recommendation

### 5.1 Use spaces between parameters
````php
public function calculateResult( $firstValue, $secondValue, $operator )
{
	// Do things
}

if ( ! $firstValue )
{
    // Do things
}
````

### 5.2 Use TODO and FIXME comments
````php
// TODO: Check conditions
// FIXME: When $item is null ...
````

### 5.3 Strings
Use single quotes for strings as a default (exception proves the rule).


