###Underscore.js

`_.size()` gets the size of an array, for example.

`_.each()` accepts an object and a callback function that runs every time it encounters an element in that object.

`_.find()` finds the **first** instance of an element that matches a set of criteria (via a callback). For example:

```js
function searchStudents(item) {
  if (item.school === "Franklin")
    return true;
}

var elem = _.find(students, searchStudents);
```

`_.findWhere()` accepts an object with properties/values we wish to match. Example:

```js
elem = _.findWhere(students, {school : "Thoreau", grade: 11});
```

`_.contains()` searches a list of values for a particular value.

`_.pluck()` retrieves all of the values for a given property.

`_.size()`

`_.size()`

`_.size()`

`_.size()`
