# Metadata

## Examples

### Class Definition


```

.class Person
    .field i8 Age
    .field string Name
    
    .method Greet (class Person other)
        push static 0 // push "Hello "
        push argument 1 // push other ?
        load field 2    // other.Name
        call String.Concat // "Hello " + other.Name
        call println 1 // println("Hello " + other.Name)
```
