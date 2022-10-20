# Array Methods

* [for (i, i++)](#for)
* [for (of)](#for-of)
* [forEach](#foreach)
* [Map](#map)
* [Filter](#filter)
* [Reduce](#reduce)
* [Find](#find)
* [FindIndex](#findindex)

> [CASE - Array methods combination](#case)

## FOR

```
for (let i=0; i < [].length; i++) {
    console.log()
}
```
## FOR-of

```
for (let item of items) {
    console.log(item)
}
```

## ForEach

* calls a function for each element in an array

```
items.forEach(function(item) {
    console.log(item)
})
```

```
items.forEach(item => console.log(item))
```

## Map

* creates a new array from calling a function for every array element
* calls a function once for each element in an array
* dose not execute the function for empty elements
* does not change the original array

> Output every person's name
```
const newArray = items.map(item => {
    return item[0]
})
```

> Output every person's name and age
```
const newPeople = people.map(person => `${person.name} (${person.age})`)
```

## Filter

* creates a new array filled with elements that pass a test provided by a function
* dose not execute the function for empty elements
* does not change the original array

> Output all adults (over 18 years old)
```
const adults = people.filter(person => person.age >= 18)
```

## Reduce

* executes a reducer function for array element
* returns a single value: the function's accumulated results
* does not execute the function for empty array elements
* dose not change the original array

> Output the sum of all budgets from the array
```
const amount = people.reduce((total, person) =>  total + person.budget, 0)
```

## Find

* returns the value of the first element that passes a test
* executes a function for each array element
* returns **undefined** if no elements are found
* does not execute the function for empty array elements
* dose not change the original array

> Output the object with name 'Игорь'
```
const igor = people.find(person => person.name === 'Игорь')
```

## FindIndex

* returns the index (position) of the first element that passes a test
* executes a function for each array element
* returns **-1** if no match is found
* does not execute the function for empty array elements
* dose not change the original array

> Output the index of object with name 'Игорь'
```
const igorIndex = people.findIndex(person => person.name === 'Игорь')
```

## CASE 

1. Iterate persons whose budget is more than 3000
2. Create a new array containing objects with info and budget values
3. Output the sum of their budgets

```
const amount = people
.filter(person => person.budget > 3000)
.map(person => {
    return {
        info: `${person.name} (${person.age})`,
        budget: person.budget
    }
})
.reduce((total, person) => total + person.budget, 0)
```