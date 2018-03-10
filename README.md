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

## Whiteboard Problem 02:

* Write a function called isSorted that accepts a linked list as
a parameter and returns true if the linked list is sorted in
ascending order

an empty or single item list should be considered sorted.
because it’s not not sorted.

## Whiteboard Problem 02 picture:
![alt text](Whiteboard-02.JPG)

## Whiteboard Problem 02 solution:

* function isSorted(linkedList) {
    let current = list.root
    if(current === null || current.next === null) {
        return true;
    } while (current) {
        if (current.data >= current.next.data) {
            return false;
        }
        current = current.next;
    }
    return true;
}