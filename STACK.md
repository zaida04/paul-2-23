## Explanation for stack

Say we have the trace tool. We want to keep track of every change someone makes to their trace, and allow them to use the undo button to undo the last change they made.

The best way we can do this, is by using a Stack. A stack will always return the last thing added (FILO, first-in last-out) to the stack.

### Visualization

Create stack frame -> Create variable -> Name variable -> Cross out variable

It'll look a lot like this on the stack:
```
---
Cross out variable <-- this is the top
Name variable
Create variable
Create stack frame
---
```

And we can just use the pop() method off the stack, and get "Cross out variable". I now know what the last thing created was.
