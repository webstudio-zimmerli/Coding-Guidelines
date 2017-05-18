# PHP Coding Guidelines

The JavaScript guidelines are mostly equal to PHPs coding guidelines.

## 1. Naming conventions
### 1.1 Usefull names
We ever use full self explaining names for variables, constants, class- and method names etc.

**Do:**
````javascript
let calculationResult = 0,
    counter = 0;

calculateResult()
{
    // Do things
}
````

**Don't:**
````javascript
let cRes = 0,
    cnt = 0;

calcRes()
{
    // Do things
}
````

### 1.2 Booleans
For booleans we prefix variables with `is` `has` `can` verbs.

````javascript
var isAuthorized = false,
    canVote = false;
````

### 1.3 Filenames
Filenames equals the classnames `FooBarCalculation.js` equals `class FooBarCalculation { }`

## 2. Curly braces
We place curly braces in every case on the next line.

**Classes**
````javascript
class FileAdapter extends Adapter
{
    // Do things
}
````

**If-Else**

````javascript
// Comment A
if (a === b)
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
````javascript
items.forEach(function(value, index))
{
    // Do things
}
````

## 4. Method visibility
For private methods we use the _ prefix

````php
calculateResult()
{
    // Do things
}

_getValueItem()
{
    // Prefixed
}
````

## 5. Recommendation

### 5.1 Use spaces between parameters
````javascript
calculateResult(firstValue, secondValue, operator)
{
	// Do things
}

if ( ! firstValue)
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


