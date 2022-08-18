# Garbage collection

I always heard this term get thrown around but I never really looked into what it was until now (August 17th, 2022).

## What is the garbage collector and what does it do?

The gargabe collector in Javascript is a form of automatic memory management. Any objects that are no longer in use
by the program, the garbage collector will free up that bit of memory.

This bit is straight from [MDN Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Memory_Management):

### Memory life cycle

1.) Allocate the memory you need
2.) Use the allocated memory (read, write)
3.) Release the allocated memory when it is not needed anymore

## Wrapping up

Memory management could be a post of its own but this is garbage collection in a nutshell. We create a value or object and JavaScript will automatically allocate memory for us and will also take it back. 