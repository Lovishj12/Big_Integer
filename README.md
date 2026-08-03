# BigInt: Arbitrary-Precision Integer Library for C++

A lightweight, robust C++ library designed to handle exceptionally large integers that exceed the 64-bit limits of standard data types like `long long`. By storing numbers internally as strings, `BigInt` allows for limitless scaling in mathematical operations and algorithmic computations.

## Key Features

- **Multiple Constructors:** Instantiate `BigInt` objects from `std::string`, `const char*`, or `unsigned long long`.
- **Operator Overloading:** Full support for standard C++ operators (`+`, `-`, `*`, `/`, `%`, `^`, `==`, `<`, `>`, etc.).
- **Seamless I/O:** Works flawlessly with standard input/output streams (`std::cin` and `std::cout`).
- **Mathematical Sequences:** Built-in functions to generate large Factorials, Fibonacci numbers, and Catalan numbers.
- **Modular Design:** Clean separation of headers (`BigInt.h`), implementation (`BigInt.cpp`), and testing (`main.cpp`).

## Compilation & Execution

Clone the repository and compile the source files using a standard C++ compiler (like `g++`). Remember that header files (`.h`) are not compiled directly.

**1. Clone the repository:**
```bash
git clone [https://github.com/Lovishj12/Big_Integer.git](https://github.com/Lovishj12/Big_Integer.git)
cd Big_Integer
```

**2. Compile the project:**
```bash
g++ main.cpp BigInt.cpp -o BigIntProgram
```

**3. Run the executable:**
- **Windows:** `.\BigIntProgram`
- **Linux/Mac:** `./BigIntProgram`

## Quick Start Example

```cpp
#include <iostream>
#include "BigInt.h"

int main() {
    // Create large integers
    BigInt base("150000000000000000000");
    BigInt multiplier(2);

    // Standard arithmetic operations
    BigInt result = base * multiplier;
    std::cout << "Product: " << result << '\n';

    // Advanced math: 100th Fibonacci number
    std::cout << "Fibonacci(100): " << NthFibonacci(100) << '\n';

    // Calculate massive factorials
    std::cout << "Factorial(50): " << Factorial(50) << '\n';

    return 0;
}
```

## API / Operator Reference

| Category | Operators / Functions |
| :--- | :--- |
| **Basic Arithmetic** | `+`, `-`, `*`, `/`, `%` |
| **Assignment Math** | `=`, `+=`, `-=`, `*=`, `/=`, `%=`, `^=` |
| **Relational** | `==`, `!=`, `>`, `<`, `>=`, `<=` |
| **Increment/Decrement** | `++` (pre & post), `--` (pre & post) |
| **Advanced Math** | `^` (Power), `sqrt()` (Square Root) |
| **Algorithms** | `Factorial(n)`, `NthFibonacci(n)`, `NthCatalan(n)` |
| **Helper Functions** | `Length()`, `Null()` |
