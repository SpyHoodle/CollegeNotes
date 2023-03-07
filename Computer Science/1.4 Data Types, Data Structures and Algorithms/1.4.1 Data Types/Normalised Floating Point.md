# Normalised Floating Point
2022-10-04 | [1.4.1 Data Types](1.4.1%20Data%20Types.md)

## Efficiency
- Exponent -> effects range
- Mantissa -> effects precision

## Normalised
- **Normalised** -> The optimised form for floating point, maximised range and maximised precision
- More precise numbers can be represented by a bigger mantissa and a smaller exponent
- Most significant bit and second significant bit of the mantissa must be different
  - e.g. $0.1010$ and $1.0110$ are valid but $1.1101$ is not valid
