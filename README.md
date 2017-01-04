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

`_.filter()` accepts the set of data and a callback function that narrows down the list by defining a set of criteria that each object must pass in order to be included in the resulting list that is returned.

`_.where()` accepts a dataset and selects only those items that match the properties defined in the object passed to it. Example:

```js
var result = _.where(students, {"school" : "Thoreau", "grade" : 10});
```

`_.reject()` opposite of `_.filter()`. Rejects items that match a set of criteria.

`_.every()` ensure that **every** criteria has been met.

`_.size()` at least one item passes a criteria set.

`_.size()`

`_.size()`

`_.size()`

`_.size()`

`_.size()`

`_.size()`

`_.size()`

`_.size()`
