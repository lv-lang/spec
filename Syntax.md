## Numbers
```
3.14
843020
```
## Strings
```
"double quotes"
'single quotes'
`backtick quotes`
```
## Booleans
```
true
false
```
## Functions
```
func myFunc(arg1, arg2) {
    
}
myFunc(1,2)
// ES6-Like functions? (Great for callback readablility)
const myFunc = (arg1, arg2) => {

}
```
## If/else
```
mut isAirplane = true
mut isBiplane = false
if (isAirplane && isBiplane) {

} else if (isAirplane && !isBiplane) {

} else {

}
```
## Operators

**Addition**

`+`

**Subtraction**

`-`

**Multiplication**

`*`

**Division**

`/`

**Modulo**

`%`

**Greater than**

`<`

**Less than**

`>`

**Plus-equals**

`+=`

**Minus-equals**

`-=`

**Multiply-equals**

`*=`

**Divide-equals**

`/=`

**Modulo-equals**

`%=`

**Increment**

`++`

**Decrement**

`--`

**And**

`&&`

**Or**

`||`

**Not**

`!`

**Assign**

`=`

**Relative Equality**

`==`

**Exact Equality**

`==`

**Bracket access**

`[]`

**Dot access**

`.`

**Bitshift right**

`>>`

**Bitshift left**

`<<`

## Comments
```
// Single Line Comment
/*
Multi Line Comment
*/
```
## Variables
**Inmutable**
```
const foo = "bar"
```
**Mutable**
```
mut foo: string = "bar"
```
**Edit Mutable**
```
mut foo: string = "bar"
foo = "moo"
```
## Unknown
Maybe?
## Objects
```
mut foo = {
    moo: "bar"
}
```
## Array
```
mut foo: Array<string> = ["foo", "moo", "bar"]
foo[0]
```
## Template Literals
```
mut name = "Jairus"
"Welcome, {name}"
```
**Name exists**
```
mut name = "Jairus"
"Welcome, {name}"
converts to:
"Welcome, " + name
```
**Name doesn't exist**
```
mut name = "Jairus"
"Welcome, {name}"
converts to:
"Welcome, {name}"
```
## Loops
```
while (condition) {
    
}
```
## Import
```
const foo = import('./')
const { foo, bar } = import('./')
const [ foo, bar ] = import('./')
```
## Import functions
```
import func myFunc(arg1, arg2): void
```
## Export
```
const foo = "Foo!"
const bar = "Bar!"

Option 1
export foo
export bar

Option 2
export {
    foo: foo,
    bar: bar
}

Option 3
export const foo = "Foo!"
export const bar = "Bar!"
```
## Classes
```
class myClass {
 constructor(arg1, arg2) {}
 func normalFunction(arg1): void {

 }
 get func getFunction(): string {
    return "hahaha!"
 }
 set func setFunction(data: string): void {
    this.getFunction = data
 }
}

const theClass = myClass("arg1", "arg2")
theClass.normalFunction("arg1")
theClass.getFunction
theClass.setFunction = "haha!"
```