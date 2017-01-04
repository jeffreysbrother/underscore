###Underscore.js

*functions for filtering data; derives smaller result sets from a large initial set of data.*

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

*Sorting and grouping*

`_.sortBy()` returns a list sorted according to some criteria.

`_.groupBy()` returns an **object** (associative array) where the keys represent the metric by which the grouping occurs.

`_.countBy()` returns an associative array arranged by the number of counts in each group.

*Manipulation*

`_.shuffle()` randomizes contents of the list. Uses the Fisher-Yates shuffle.

`_.map()` takes a data set and produces a new array based upon each item in the list. Can map a numerical grade to a letter grade, for example.

*Arrays and Objects*

`_.first()` and `_.last()` First or last element of the array (returns one value).

`_.initial()` and `_.rest()` Returns arrays that are subsets of the initial array: initial elements minus **x** number of elements ... and ... the last elements minus **x** number of elements off the front of the array.

*Array operations*

`_.without()` remove unwanted values from an array.

`_.union()` join two arrays together.

`_.intersection()` opposite of union. Returns common values from two arrays.

`_.difference()` returns values not present in the *other* array.

*Object operations*

`_.keys()` retrieve the keys of an object.

`_.values()` retrieve the values of an object.

`_.pick()` can request multiple properties by passing in desired keys.

`_.omit()` filter out multiple properties we don't need.

`_.extend()` add new properties to existing objects.

`_.defaults()` assign default values to an object.

`_.clone()` make a shallow copy of an object (values of objects that are arrays or objects themselves are copied by reference ... not duplicated)

`_.uniqueId()` generate a unique id and supply an optional prefix.

`_.random()` generate a random number (not between 0 and 1, like JavaScript's built-in function). Can provide one argument *x* for a value between zero and *x* (inclusive), or two arguments for a value between that range (also inclusive).

`_.times()` short-hand way of executing a counter loop (like a for loop).

`_.mixin()` use this to extend Underscore. Accepts an object where the keys are names of functions, and the value of each key is the function that carries out whatever the hell you want it to do. Example of creating a new `_.capitalize()` function:

```js
_.mixin({
      capitalize: function(string) {
          return string.charAt(0).toUpperCase() + string.substring(1).toLowerCase();
      }
});
```

`_.size()`

`_.extend()`

`_.size()`
