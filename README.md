# evaluation-javascript-iterator
Please consider any code you write for this task to be production quality, meaning that it should follow your normal development process as much as possible. Please submit as many files as necessary.

Please use vanilla javascript.

## Question 1

We are going to implement a simple iterator for JavaScript. Please implement a class that has the following interface.

A constructor that takes an array.

`hasNext()`

If the class can iterate the array further, it will return true. If a call to next() will fail, it will return false.

`next()`

This moves the iterator one spot and returns the new value.

`current()`

This will return the current value pointed to by the iterator.

`tag()`

This function will return a function, this function when invoked will return the current value when the tag function was invoked.

`reverse()`

This function will reverse the loaded array. After this function is invoked a call to current will return the same value it would have before the call. For example

1 2 3

current -> 2

reverse -> (internal state is now 3 2 1)

current -> 2


## Question 2

You are given the following html page.

```

<html>
<head></head>
<body>

<div class="section">
    1 2 3 4 5 6
</div>

<div class="section">
    6 5 4 3 2 1
</div>

</body>
</html>
```
 

Write a script that will load from the first div with the class section into the iterator class you just created.
