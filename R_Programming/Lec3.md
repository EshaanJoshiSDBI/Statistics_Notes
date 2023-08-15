### Basic Data Types
- Basic data types in R can be divided into the following types
1. numeric - (10.5,55,787)
2. integer - (1L,55L,100L, where the letter 'L' declares this as an integer)
3. complex - (9+3i, where 'i' is the imaginary part)
4. character (aka string) - ('k','R is exciting','FALSE','11.5')
5. logical (aka boolean) - (TRUE or FALSE)

```
> x <- 10.5
> class(x)
[1] "numeric"
> x<-1000L
> class(x)
[1] "integer"
> x<-9i+3
> class(x)
[1] "complex"
> x<-"R is exciting"
> class(x)
[1] "character"
> x<-TRUE
> class(x)
[1] "logical"
```

```
> x<-10.5
> y<-55
> x
[1] 10.5
> y
[1] 55
> class(x)
[1] "numeric"
> class(y)
[1] "numeric"
```