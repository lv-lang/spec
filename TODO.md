# Core
1. Finalize Syntax
are we doing the `mut foo: string = "bar"` or `string* foo = "bar"`?
So I'm not really sure. I think that mutability should be a type thing if that makes sense.
Do
es it?

Myabe

Perhaps we should have:
//Constant
var myVar:string ="2"
//Mutable
var myVar:string* = "2";
// Its quxite long tho.
maybe:
string myVar = "2"
is shorter
Yeah that seems good
my main worry is mainting ts/js idioms
but we can move past them
as they are kind primitive

So, are we making a whole new syntax here, or knocking it off of js/ts?

I think we are addapting some js/ts features, except with our own custom syntax
Yeah, that's what I was thinking
Kind of a mix-mash of different langs. 
Yeah that seems good
however what about auto?
I dont like the syntax: ?
auto myVar = "2"; 

I have an idea:

//MAnual type
<string> myVar = "hhello"
//Auto

<> myVar = "hello"

Hmm. 
Should we change the return type on functions?
b/c it might be confusing to have ts-style return types
func myFunc(a: string, b: string): void {

}

funct myFunc(a <string>, b: string): <string> {}
Actually nvm
I think types should be like ts
TS-types look really nice on functions
But I think we should stick to one type-style
<> isn't type style, its variable  style
I just want to remove the annoying auto/var/const/let
^ I agree for sure
statements



It might get ugly if you have rlly long types

<string[[[[[[[[[]]]]]]]]]> foo = [[[[[[[[[[["hah!"]]]]]]]]]]]
^ would be rare tho
perhaps just |?
|myvar:string="2";

maybe auto-detect vars?

string foo = "haha"
// If foo isn't declared before, its a var.
// else, its a assign
// ^ would be compiled at runtime. A bit like 
python's vars
hm. let me think for a second ok
Maybe look for ways other langs do it?

https://gobyexample.com/variables
https://doc.rust-lang.org/book/ch03-01-variables-and-mutability.html
https://www.tutorialspoint.com/cprogramming/c_variables.htm
https://nim-by-example.github.io/variables/
https://www.w3schools.com/python/python_variables.asp
https://dart.dev/guides/language/type-system
https://www.w3schools.com/cpp/cpp_variables.asp

c++ vars are my fav
yeah, we should go with that
cool
wbt c++ funcs?
They look nice ig
the problem ig is how we deal with higher level constructs 
but idk
yeah
what about parameter syntax
hmm.. What's your opinion first?

however var declarations are signified
by <>'s

2. Add types
3. Create AST
4. Add compiler (binaryen + wasm-opt?)
6. Add syntax
 <br>
 a. Strings
 <br>
 b. Numbers
 <br>
 c. Booleans
 <br>
 d. Functions
 <br>
 e. If/else
7. Add closures
8. Add transforms
9. Add standard library
 <br>
 a. String
 <br>
 b. Number
 <br>
 c. Boolean
 <br>
 d. Array
 <br>
 e. Object
 <br>
 f. Math
 <br>
 g. In-built
10. Add union types

# Ideas
1. Code formatter