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

```
items.forEach(function(item) {
    console.log(item)
})
```

```
items.forEach(item => console.log(item))
```

## Map

* method creates a new array populated with the results of calling a provided function on every element in the calling array

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

* method creates a shallow copy of a portion of a given array, filtered down to just the elements from the given array that pass the test implemented by the provided function

> Iterate array and give out all adults (over 18 years old)
```
const adults = people.filter(person => person.age >= 18)
```

## Reduce

## Find

## FindIndex
