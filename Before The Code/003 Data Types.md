# Basic and Composites
Golang is a statically types language, this means that the type of all variables is known at compile time. What this does not mean is that we must specifically declare the type of each variable. Unlike Java, C and C++ go works more similar to Scala and Haskell in which it has the ability to figure out the type we want by the value we are assigning to it. 

## The basic types.

### Integers
*Default Value: 0*
Golang is made of 5 signed and unsigned integer types :

| Data Type      | Size in Bytes | Size in Bits | 
| -------------- |:-------------:|:------------:| 
| int / uint     |    4 or 8     |   32 or 64   |  
| int8 / uint8   |       1       |      8       |    
| int16 / uint16 |       2       |      16      |  
| int32 / uint32 |       4       |      32      |   
| int64 / uint64 |       8       |      64      |    

**signed** integers can hold either a positive or negative number
**unsigned** integers can hold positive numbers only. 

### Floats
*Default Value: 0.0*
There are 2 float types:

| Data Type | Size in Bytes | Size in Bits |
| --------- |:-------------:|:------------:|
| float32   |       4       |      32      |
| float64   |       8       |      64      |

### Runes
This is a type that represents characters through the use of int32 values. The rune is an alias type used in UTF-8 encoding. Unicode uses a system called [code points](https://en.wikipedia.org/wiki/Code_point), which are numbers assigned to represent abrstract characters. 

### Booleans
*Default Value: false*
A logical true or false value, unlike some other languages booleans in Go store the value as actually being "true" or "false" and not 1 or 0

### Strings
*Default Value: ""*
A string is an slice of characters(runes) that are variable in width, each character is represented by it's byte amount using UTF-8 encoding. These are a read only value, meaning they are immutable.

Each byte in a string is accessible.

### Bytes

Similar to how runes are an alias of the int32 a byte in go is an alias to a uint8. Unlike most commonly used languages Golang does not have a datatype that directly represents `char` so bytes are used to represent ASCII characters. 

*Runes vs Bytes: While runes represent every character in the UTF-8 encoding library, bytes only represent ASCII characters.* 

### Complex Numbers

| Data Type | Size in Bytes | Size in Bits |
| --------- |:-------------:|:------------:|
| complex64   |       8       |      64      |
| complex128  |       16       |      128      |

The actual mathematical reasonings behind the use of complex numbers are well beyond the scope of this documentation and as I find myself being someone who has yet to have any use whatsoever for them I do not thing I am in a position to explain their uses. 

Essentially complex numbers are represented in the form of both real and imaginary numbers, with the imaginary number being refered to as an `iota`. 

If you are someone who is seeking the use of complex numbers you are someone who probably already know their uses and implementations. 

complex64's are represented by 2 float32s, while complex128's are represented by 2 float64's

## The Composite Types
### Arrays


### Structs
### Slices
### Maps
### Channels
### Pointers
### Functions 
### Interfaces 






