# Using Our Packages

## Imports

Since we are aware that our packages at their core are just file and directory containers for code we, or someone else has written that fufills a specific purpose, it would be important to know how we make use of that code. 

That's where the `import` keyword comes into play. Let's take a look at import in action using what is probably the most written program on the face of the earth. Hello, world!

```go 
package main

import "fmt"

func main(){
	fmt.Println("Hello, world!")
}
```

We all know what this program outputs. Go uses something called the Standard Library (more on that later) to call the Println function and output our "Hello, world!" text. 

[`"fmt"`](https://pkg.go.dev/fmt) is a package within the Go standard library that is used to implement C style I/O operations. Go lang also lets you import multiple packages from various libraries using a multi-line import syntax that looks like:

```go 
package main

import (
	"bufio"    // buffered I/O 
	"fmt"      // formated I/O 
	"os"       // operating system functionality
)
```

#### Note
You can also alias an import.

```go 
package main

import f "fmt"

func main(){
	f.Println("Hello, world!")
}
```


## Exports
Unlike languages that explicitly declare exports, Go uses capitalization of works to specify their use as exported names. In the above examples within the `fmt` package `Println(...)` is capitalized and thus is exported from the package. Any names within a package that are not capitalized are not accessible from outside the scope of that package. 

