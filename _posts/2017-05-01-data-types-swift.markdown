---
layout: post
title:  "Data Types in Swift!"
date:   2017-05-01 08:00:00 +0530
categories: swift
---

Swift offers the programmer a rich assortment of built-in as well as user-defined data types.

# Primitive Data Types

The following types of basic data types are most frequently used when declaring variables −

## Integers
### Int
- On a 32-bit platform, Int is the same size as Int32.
- On a 64-bit platform, Int is the same size as Int64.

### UInt
- On a 32-bit platform, UInt is the same size as UInt32.
- On a 64-bit platform, UInt is the same size as UInt64.

For the naming conventions different specific kind of data types used. Swift provides the same naming convetions as C: 
- **8-bit unsigned integer** : **UInt8**
- **32-bit signed integer** : **Int32**

UInt8, Int32, Int6, UInt32, UInt64

#### NOTE
* UInt8 cannot store negative numbers. i.e.: 
``` swift
    let negativeInteger : UInt = -1 //will throw the error
```
* A varibale going out of capacity will be notified. If compiler is able to calculate the value it will notify:
``` swift
    let outofCapacityNumber : Int8 = Int8.max + 1 //will throw the error
```
* Adding two different types of data not allowed in Swift:
``` swift
    let outofCapacityNumber : Int8 = Int8.max + 1 //will throw the error
    let thousandAndOneHundered = thousand + UInt16(oneHundered) // Need typecasting
```
 
## Floating-Point Numbers
### Float
This is used to represent a 32-bit floating-point number and numbers with smaller decimal points. For example, 3.14159, 0.1, and -273.158.

### Double 
This is used to represent a 64-bit floating-point number and used when floating-point values must be very large. For example, 3.14159, 0.1, and -273.158.

### Bool
This represents a Boolean value which is either true or false.
``` swift
    let iamRight = true
    if iamRight {
        print("Yes, but for this time 😃");
    }
```
Because of type safety we can not treat integer as boolean:
``` swift
    let iamAlwaysRight = 1
    if iamAlwaysRight {
        print("You seems lost! Ask Siri for Help.");
    }
```

### String
This is an ordered collection of characters. For example, "Hello, World!"

### Character
This is a single-character string literal. For example, "C"

I'll explore string in next discussions.
