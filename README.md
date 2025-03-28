# Decimal
Decimal is an educational project by School 21, aimed at implementing the decimal type in the C programming language. The standard C library does not provide a built-in decimal type, making this implementation particularly useful for financial calculations, where the rounding errors typical of floating-point arithmetic are unacceptable.
## Key Features of Decimal Type
Precision & Range: Represents decimal numbers from ±79,228,162,514,264,337,593,543,950,335 with a default value of 0.

**Structure**:

* A sign bit (1 bit).

* A 96-bit integer for numerical value.

* A scaling factor (power of 10 from 0 to 28) that determines the position of the decimal point.

**Accurate Rounding**: Multiplication and division operations minimize precision loss when passed to rounding methods.

**Trailing Zeros Preservation:** Retains trailing zeros, which do not affect arithmetic or comparison operations but maintain numerical integrity.

This format is ideal for high-precision financial calculations requiring both integer and fractional digits while minimizing rounding errors.

## Usage
1. Clone this repository via
   - SSH `git@github.com:Zayfed/decimal.git` or
   - HTTPS `https://github.com/Zayfed/decimal.git`
2. Run make to build project
3. Run make test to build project and run aux tests
4. Run make gcov_report to create a test report

