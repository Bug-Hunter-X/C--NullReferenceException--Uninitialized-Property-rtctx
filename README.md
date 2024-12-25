# C# NullReferenceException: Uninitialized Property

This repository demonstrates a common C# coding error: a `NullReferenceException` caused by accessing an uninitialized property.  The `bug.cs` file contains code that throws this exception, while `bugSolution.cs` offers a solution.

**Problem:** In `MyClass`, the `MyProperty` is not initialized before being accessed in `MyMethod()`.  If the program executes `MyMethod()` before assigning a value to `MyProperty`, it leads to a runtime `NullReferenceException`.

**Solution:** Initialize the property either in the constructor or when declaring the variable, thus preventing the null reference error.  The correct way is demonstrated in `bugSolution.cs`.