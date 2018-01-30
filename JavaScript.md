# JAVASCRIPT NOTES

Javascript is prototype based.  What is that?

JavaScript is a scripting language.  It is interpreted by the browser when  it is loaded.

### Data Types

*  numbers
*  strings
*  arrays
*  objects

### Variables

Variable names may be made up of letters, numbers, underscores and dollar signs.
Variable names should begin with a letter (or _ or $, but usually a letter).  They are case sensitive.

### Variable naming style conventions

  **Camel Case**
    - var camelCase;

  **Partial Case**
    - var PartialCase;

  **Underscore**
    - var underscore_case;

**Dash**
    - var dash-case;

### Arrays

    .push()

    .length()

    .sort()

    .reverse()

### Loops

  **For loop**  
```
    for (var i = 0; i < 10; i++){
      //code here
    }
```


  **While loop**
```
    var i = 0;
    while(i < 10){
      //code here
      i++
    }
```


  **forEach loop**
```
    var array = [1,2,3];
    numbers.forEach(function(){
      // iterate through array
    )

```
### Conditionals

    = is assignment  
    == is testing for equivalency
    === is testing for strict equivalency
    != not equal to

    || is or

    && is and


  **if statement**
```
    if(condition){
      // do something
    }
```

  **else statement**
```
    if(condition){
      // do something
    }
    else{
      // do something else
    }
```

  **else if statement**  
```
    if(condition){
      // do something
    }
    else if(another condition){
      // do something else
    }
    else{
      // do something if it is neither condition
    }
```

  **switch statement**
```
    var variable = 'something';

    switch(variable){
      case 'something':
        // do something
        break;
      case 'something else' :
        // do something else
        break;
      default:
        // do something here if variable is not something or something else
        break;
    }
```

### Objects

  #### Object literals

    var person = {
      firstName: 'Brad',
      LastName: "Bedlam",
      age: 30
    }

    // person.age == 30

  **Embedded Arrays in Objects**

    var person = {
      firstName: 'Brad',
      LastName: "Bedlam",
      age: 30,
      children: ['Buford', 'Maynard']
    }

    // person.children[0] = 'Buford'

  **Embedded Objects in Objects**

    var person = {
      firstName: 'Brad',
      LastName: "Bedlam",
      age: 30,
      address: {
        street: '100 Main St',
        city: 'Springfield',
        state: 'someState'
      }
    }

  **Embedded Functions in Objects**  

    var person = {
      firstName: 'Brad',
      LastName: "Bedlam",
      age: 30,
      address: {
        street: '100 Main St',
        city: 'Springfield',
        state: 'someState'
      }
      fullName: function(){
        return this.firstName+''+this.LastName;
      }
    }

  #### Object Constructors

  **Constructors**  

    var apple = new Object();
    apple.color = 'red';
    apple.shape = 'round';

    apple.describe = function(){
      return 'An apple is ' + this.shape + ' and ' + this.color;
    }

    apple.describe() // 'An apple is round and red'

  **Constructor Patterns**

    function Fruit(name, color, shape) = {
      this.name: name,
      this.color: color;
      this.shape: shape;
      this.describe = function(){
        return 'An ' + this.name + ' is ' + this.shape + ' and ' + this.color;
      };
    }

    var orange = new Fruit('orange', 'orange', 'round');

    orange.describe(); // 'An orange is orange and round'

  **Arrays of Objects**

    var users = [
      {
        name: 'Craig',
        age: 50
      },
      {
        name: 'Nancy',
        age: 44
      },
      {
        name: 'Eddie',
        age: 13
      }
    ];

    users[0].name // 'Craig'

  ### Events




  ### Built in JS Functions

  alert();

  console.log();

  **Scope**

  this.
