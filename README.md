# Brandon Buchholz Code Fellows whiteboard problems:

## Whiteboard Problem 01:

* Write a function called `contains()` that accepts a
linked list and a value. Return true if the value is 
in the linked list.

## Whiteboard Problem 01 picture:
![alt text](assets/Whiteboard-01.JPG)

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
![alt text](assets/Whiteboard-02.JPG)

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
## Whiteboard Problem 03:

* Write a function called `isBalanced` that accepts a
string of left and right brackets and returns true if
the brackets are balanced.

Use a stack!
Push whenever you see an opening curly brace.
Pop whenever you see a closing curly brace.
If you see a closing curly brace when the stack is empty,
that's an error.

## Whiteboard Problem 03 picture:
![alt text](assets/Whiteboard-03.JPG)

## Whiteboard Problem 03 solution:

* function isBalanced(str) {
    let stack = [];
    let open = { '{': '}' };
    let closed = { '}': true };
    for (var i = 0; i < str.length; i++) {
        let char = str[i];
        if (open[char]) {
            stack.push[char]
        } else if (closed[char]) {
            if (open[stack.pop()] !== char)
             return false;
        }
    }
    return stack.length === 0;
};
## Whiteboard Problem 04:

* Write a function called tally that accepts a string and returns the most frequently used word in the string.

Assume the string your given is all lowercase, contains no punctuation and each word is seperated by exactly one space.

If you were given good input for the last verse of The Twelve Days of Christmas your function should return "a" because "a" is the word that appears the most in this verse:


## Whiteboard Problem 03 picture:
![alt text](assets/Whiteboard-04.JPG)

## Whiteboard Problem 03 solution:

* let tally = function (str {
    let mw = {};
    let hv = 0;
    let hk = null;
    if (str.length === 0 ) return false
    let arr = str.split(" ");
    for (let i = 0; i < app.length; i++){
        if (mw[i] === undefined) {
            mw[i] = 0;
        }
            mw[i]++
    }
    for( key in mw) {
        if( mw[key]> hv) {
            hv = mw[key];
            hk = key;
        }
    } 
    return hk;
});