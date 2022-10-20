# Array Methods

* [for (i, i++)](#for)
* [for (of)](#for-of)
* [forEach](#foreach)
* [Map](#map)
* [Filter](#filter)
* [Reduce](#reduce)

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
console.log(newArray)
```

> Output every person's name and age
```
const newPeople = people.map(person => `${person.name} (${person.age})`)
console.log(newPeople)
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

## Find

## FindIndex
