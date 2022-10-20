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

```
const newArray = items.map(item => {
    return item[0]
})
console.log(newArray)
```

```
const newPeople = people.map(person => `${person.name} (${person.age})`)
console.log(newPeople)
```

## Filter

## Reduce

## Find

## FindIndex
