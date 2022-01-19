# Strings
String manipulation is a very important part of programming. From text parsing, formatting, splitting, and more, Asylum has you covered.

## String Operations
There are many operations you can apply to strings to manipulate them. Below is a list of common operations.

### String Addition
It is common to want to join strings together. In Asylum, you simply add strings together with `+`.

```rust
string a = "Hello ";
string b = "World!";
println(a + b);
```
Output:
```
Hello World!
```

### String Subtraction
You can also remove parts of strings in Asylum. Using `-` will remove any instance of the second string.

```rust
string a = "Hello World!";
println(a - "l");
```
Output:
```
Heo Word!
```

### String Multiplication
Want to repeat a string multiple times? Multiply it using `*` and an integer to repeat it.

```rust
println("Hello " * 3);
```
Output:
```
Hello Hello Hello 
```

### String Division
In Asylum, you can also split strings by using the `/` operator followed by what characters you wish to split by.

```rust
string[] a = "cat, dog, fox" / ", ";
for string s in a
    println(s);
```
Output:
```
cat
dog
fox
```

### String Comparison
In other programming languages, you may have to use methods such as `Equals(object other)` to make sure to compare the values of the strings rather than the references. Since Asylum is not reference-based, you can compare them with `==` just fine even if one of the items is a reference!

```rust
string a = "Hello World!";
string b = "Hello " + "World!";
string@ c -> b; // c is now a reference to b. For now just pretend c is a shortcut to b, and using c would use b instead.
string d = "Hellm";
println(c == a); // The same as b == a which is true.
println(a != b);
println(d <=> b); // Compares d and b. d has Hellm and m is two less than o, so the result is -2.
println(c <= a);
```
Output:
```
true
false
-2
true
```

## String Functions
For greater control over strings, you can use some of the buildin functions to manipulate them. TODO!!! toString, replace, substring, length, etc.

## F-Strings
Format strings, or f-strings for short, are a quick way of printing and reading data.