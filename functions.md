## This is a more elaborated example of what functions look like in Jewel

### End Keyword
	The end keyword is the equivalent of a return statement in most programming languages when used in a function. It is meant to tell the function that it is to stop executing and pop itself of the call stack. Any value in the parentheses will be passed to the next function below and if it is main then the program ends.

```rust
// Functions are blocks that are defined outside the main function, the can either return a value or not
// Format of a function == name::argument1:argument2.. -> return types
// Function that returns a value

add::Int:Int->Int
add a b {
    end (a + b);
}

printSomething->Void
printSomething {
    print("Hi I'm a different function");
    end;
}

main::[String]->Int
main args {
    let mut num1 = 10;
    let mut num2 = 10;
    let sum = add(num1, num2);
    printSomething();
    print(sum);
	end (0);
}
```
