# Functions

## Example

```
func add(i32 a, i32 b) -> i32 {
  ret a + b
}
```

## Returning
Values can be returned (ret) from any location inside the function. In languages like JavaScript, if the return is in an if-statement, then it is the same as a break. However, all returns are the same regardless of location.

```
func add(i32 a, i32 b) -> i32 {
  ret a + b
}
```
Same as:
```
func add(i32 a, i32 b) -> i32 {
    if (a && b) ret a + b
}
```