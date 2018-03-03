# Brandon Buchholz Code Fellows whiteboard problems:

## Whiteboard Problem 01:

* Write a function called `contains()` that accepts a
linked list and a value. Return true if the value is 
in the linked list.

## Whiteboard Problem 01 picture:
![alt text](Whiteboard-01.JPG)

## Whiteboard Problem 01 solution:

* function contains(list, value) {
    let current = list.root
    while(current !== null) {
        if current = (value) {
            return true
        }
        current = current.next
    }
    return false
};