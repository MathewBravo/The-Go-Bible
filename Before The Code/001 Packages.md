# The Building Blocks of Golang

## What are Packages?

As with most popular programming languages, go is made up of a multitude of files and directories. 

Just like every C++, C and Rust program, Go uses a "main" to act as an entry point to the rest of the program. When the program is created it links the main package to all the packages that your main package imports and following this process it invokes your `main` function. When your `main` function finishes its execution regardless of any incomplete co-routines (Go-routines) the program will exit. 

Does this mean that every time I write anything in Go, I must have a `package main`. Not necessarily, there may be many times when you create packages that are designed to be extensible or used by other Go programs to complete tasks. Most commonly, this type of implementation is called a "shared library". 

Remember, packages are just a containment method, they are nothing more than files and directories that are used by your `package main` to complete the tasks they were designed and written to do. 

### Common File Structure Conventions

```
go-project
  |
  |--go.mod
  |--go.sum
  |
  +-- cmd
  |    |
  |    +-- main
  |          L main.go 
  +-- pkg
       |
       +-- doctor
       |     L meetpatient.go
   	   |	 L givemedicine.go
       |
       +-- reception
            L bookpatient.go
   	  		L answercall.go
```


### Naming Conventions for Packages

The convention for naming packages in go is to have the name of the package be the same as the last name in the import path. 

```go
	// goprogram/pkg/doctor/meetpatient.go

	package meetpatient
```


*Continue 
[Imports and Exports](obsidian://open?vault=The%20Go%20Bible&file=Before%20The%20Code%2F002%20Imports%20and%20Exports)




