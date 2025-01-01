# Uninitialized Property Access in C#

This repository demonstrates a common C# error: accessing a class property before it has been assigned a value.  Uninitialized properties can lead to unexpected behavior, such as exceptions or incorrect calculations.  The `bug.cs` file shows the problematic code, while `bugSolution.cs` offers a corrected version.

## Bug Description

The `MyClass` class has a property `MyProperty`. The `MyMethod` attempts to access `MyProperty` without first assigning it a value. This can result in the program obtaining an unexpected value (0 for an integer, or null for a reference type) leading to unpredictable behavior or runtime errors.

## Solution

The solution involves initializing `MyProperty` either in the constructor or before accessing it in the method. This ensures a predictable and well-defined state for the object.