# Go Learning

## Chapter 01 - Tutorial

- Go has a lot of standard libraries and that's incredible
- I could read and make some rich examples, as an web server, client http with a methods
- Some aspects are confuse for me:
  - Pointers, of course
  - Method returns with more than one variable: resp, err := someMethod
  - Package declaration for different programs in the exercises (vs code show some warnings)

## Chapter 02 - Program Structure

## Names
Go has just 25 keywords like if, for, const, var, etc;

There is no limit on name length, but convention and style in Go programs lean toward short names, especially for local variables with small scopes; you are much more likely to see variables named i than theLoopIndex. **Generally, the larger the scope of a name, the longer and more meaningful it should be.**

The zero-value mechanism ensures that a variable always holds a well deﬁned value of its type;
**in Go there is no such thing as an uninitialized variable.** This simpliﬁes code and often ensures sensible behavior of boundary conditions without extra work. For example,

```go
var s string
fmt.Println(s) // ""
```