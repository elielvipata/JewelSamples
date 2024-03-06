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
