# JS30 #4: array-methods-day-1
This is the fourth practice of JS30 projects by Wes Bos.<br>
This project intends to show how to use some fundamental array methods like filter,map,sort and reduce.<br><br>
### The filter() method
It creates a new array filled with elements that pass a test provided by a function and when performing that,<br> it does not change the original array.<br>
In this step, it is showed how to filter the list of inventors for those who were born in the 1500's.<br>
```
 const fifteen = inventors.filter(inventor => inventor.year >= 1500 && inventor.year < 1600);
```
### The map() method
It creates a new array calling a function for every array element and does not change the original array like the filter method.<br>
In this step, it is showed how to make a new array including the inventors' first and last names applying to map method.
```
const fullNames = inventors.map(inventor => `${inventor.first} ${inventor.last}`);
```
### The sort() method
It sorts the elements of an array and that means it returns to an array with the items sorted.
Here, in this step, it is created an array<br> by sorting the inventors by their birthdates, oldest to youngest.
```
inventors.sort((a, b) => {
      return a.year - b.year;
    });
```
### The reduce() method
This method is used to return a single value which is the function's accumulated result.
In this challenge, the total years that all the inventors lived are calculated by using the reduce method.
```
 const totalYears = inventors.reduce((total, inventor) => {
      return total + (inventor.passed - inventor.year);
    }, 0);
```

