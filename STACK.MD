```jsx
stack is a linear DS that follow LIFO last in first out the element inserted is the first to be pop out 
```

```jsx
class Stack {
    constructor() {
        this.array = [];
    }
    append(data) {
        this.array.push(data);
    }
    display() {
        console.log(this.array);
    }
    peek() {  // Fixed the method name
        return this.array.length > 0 ? this.array[this.array.length - 1] : undefined;
    }
    remove() {
        return this.array.pop();  // Return the removed element
    }
}

const myStack = new Stack();
myStack.append(5);
myStack.append(6);
myStack.display(); // Output: [5, 6]
console.log(myStack.peek()); // Output: 6
myStack.remove();
myStack.display(); // Output: [5]
```
```jsx
complexity same time & space push() o(1)
pop() o(1)
top() o(1)
empty() o(1)
```
