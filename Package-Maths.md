# Scope: maths

The `maths` scope contains mathematical functions and constants.
```js
import maths
```
OR
```js
import Maths
```

## Constants

### `PI`

The mathematical constant π (pi).

| Name | Description             |
| ---- | ----------------------- |
| PI   | The value of π (pi).    |

### `E`

The mathematical constant e.

| Name | Description         |
| ---- | ------------------- |
| E    | The value of e.     |

## Functions

### `add(first, second)`

Adds two numbers together.

#### Parameters

| Name   | Description                 |
| ------ | --------------------------- |
| first  | The first number to add.    |
| second | The second number to add.   |

#### Returns

The result of adding `first` and `second`.

#### Example

```python
result = maths.add(5, 3)
# Result: 8
```

### `sub(first, second)`

Subtracts one number from another.

#### Parameters

| Name   | Description                 |
| ------ | --------------------------- |
| first  | The number to subtract from.|
| second | The number to subtract.     |

#### Returns

The result of subtracting `second` from `first`.

#### Example

```python
result = maths.sub(10, 4)
# Result: 6
```

### `mul(first, second)`

Multiplies two numbers together.

#### Parameters

| Name   | Description                  |
| ------ | ---------------------------- |
| first  | The first number to multiply. |
| second | The second number to multiply.|

#### Returns

The result of multiplying `first` and `second`.

#### Example

```python
result = maths.mul(7, 3)
# Result: 21
```

### `div(first, second)`

Divides one number by another.

#### Parameters

| Name   | Description                |
| ------ | -------------------------- |
| first  | The number to be divided.  |
| second | The divisor.               |

#### Returns

The result of dividing `first` by `second`.

#### Example

```python
result = maths.div(15, 3)
# Result: 5
```

### `pow(base, exponent)`

Raises a base number to a given exponent.

#### Parameters

| Name     | Description               |
| -------- | ------------------------- |
| base     | The base number.          |
| exponent | The exponent to raise to. |

#### Returns

The result of raising `base` to the power of `exponent`.

#### Example

```python
result = maths.pow(2, 3)
# Result: 8
```

### `sqrt(number)`

Calculates the square root of a number.

#### Parameters

| Name   | Description                 |
| ------ | --------------------------- |
| number | The number to calculate the square root of. |

#### Returns

The square root of `number`.

#### Example

```python
result = maths.sqrt(25)
# Result: 5
```

### `mod(number)`

Calculates the modulus (remainder) of a number.

#### Parameters

| Name   | Description                 |
| ------ | --------------------------- |
| number | The number to find the modulus of. |

#### Returns

The modulus of `number`.

#### Example

```python
result = maths.mod(10, 3)
# Result: 1
```

### `ln(value)`

Calculates the natural logarithm of a value.

#### Parameters

| Name   | Description                 |
| ------ | --------------------------- |
| value  | The value to calculate the natural logarithm of. |

#### Returns

The natural logarithm of `value`.

#### Example

```python
result = maths.ln(2.71828)
# Result: 1.0
```

### `log10(value)`

Calculates the base 10 logarithm of a value.

#### Parameters

| Name   | Description                 |
| ------ | --------------------------- |
| value  | The value to calculate the base 10 logarithm of. |

#### Returns

The base 10 logarithm of `value`.

#### Example

```python
result = maths.log10(100)
# Result: 2.0
```

### `exp(exponent)`

Calculates the exponential value of a given exponent.

#### Parameters

| Name     | Description                   |
| -------- | ----------------------------- |
| exponent | The exponent to calculate the exponential value of. |

#### Returns

The exponential value of `exponent`.

#### Example

```python
result = maths.exp(2)
# Result: 7.38905609893
```

### `abs(number)`

Calculates the absolute value of a number.

#### Parameters

| Name   | Description                 |
| ------ | --------------------------- |
| number | The number to calculate the absolute value of. |

#### Returns

The absolute value of `number`.

#### Example

```python
result = maths.abs(-5)
# Result: 5
```

### `round(number)`

Rounds a number to the nearest integer.

#### Parameters

| Name   | Description               |
| ------ | ------------------------- |
| number | The number to be rounded. |

#### Returns

The rounded integer value of `number`.

#### Example

```python
result = maths.round(3.7)
# Result: 4
```

### `sin(angle)`

Calculates the sine of an angle.

#### Parameters

| Name   | Description               |
| ------ | ------------------------- |
| angle  | The angle in radians for which to calculate the sine. |

#### Returns

The sine of `angle`.

#### Example

```python
result = maths.sin(0.5)
# Result: 0.4794255386
```

### `cos(angle)`

Calculates the cosine of an angle.

#### Parameters

| Name   | Description               |
| ------ | ------------------------- |
| angle  | The angle in radians for which to calculate the cosine. |

#### Returns

The cosine of `angle`.

#### Example

```python
result = maths.cos(0.5)
# Result: 0.87758256189
```

### `tan(angle)`

Calculates the tangent of an angle.

#### Parameters

| Name   | Description               |
| ------ | ------------------------- |
| angle  | The angle in radians for which to calculate the tangent. |

#### Returns

The tangent of `angle`.

#### Example

```python
result = maths.tan(0.5)
# Result: 0.54630248984
```

### `asin(value)`

Calculates the arcsine of a value.

#### Parameters

| Name   | Description               |
| ------ | ------------------------- |
| value  | The value for which to calculate the arcsine. |

#### Returns

The arcsine of `value`.

#### Example

```python
result = maths.asin(0.5)
# Result: 0.52359877559
```

### `acos(value)`

Calculates the arccosine of a value.

#### Parameters

| Name   | Description               |
| ------ | ------------------------- |
| value  | The value for which to calculate the arccosine. |

#### Returns

The arccosine of `value`.

#### Example

```python


result = maths.acos(0.5)
# Result: 1.0471975512
```

### `atan(value)`

Calculates the arctangent of a value.

#### Parameters

| Name   | Description               |
| ------ | ------------------------- |
| value  | The value for which to calculate the arctangent. |

#### Returns

The arctangent of `value`.

#### Example

```python
result = maths.atan(0.5)
# Result: 0.463647609
```

### `sec(angle)`

Calculates the secant of an angle.

#### Parameters

| Name   | Description               |
| ------ | ------------------------- |
| angle  | The angle in radians for which to calculate the secant. |

#### Returns

The secant of `angle`.

#### Example

```python
result = maths.sec(0.5)
# Result: 1.13949392732
```

### `csc(angle)`

Calculates the cosecant of an angle.

#### Parameters

| Name   | Description               |
| ------ | ------------------------- |
| angle  | The angle in radians for which to calculate the cosecant. |

#### Returns

The cosecant of `angle`.

#### Example

```python
result = maths.csc(0.5)
# Result: 2.08582964293
```

### `cot(angle)`

Calculates the cotangent of an angle.

#### Parameters

| Name   | Description               |
| ------ | ------------------------- |
| angle  | The angle in radians for which to calculate the cotangent. |

#### Returns

The cotangent of `angle`.

#### Example

```python
result = maths.cot(0.5)
# Result: 1.83048772171
```

### `sinh(angle)`

Calculates the hyperbolic sine of an angle.

#### Parameters

| Name   | Description               |
| ------ | ------------------------- |
| angle  | The angle in radians for which to calculate the hyperbolic sine. |

#### Returns

The hyperbolic sine of `angle`.

#### Example

```python
result = maths.sinh(0.5)
# Result: 0.52109530549
```

### `cosh(angle)`

Calculates the hyperbolic cosine of an angle.

#### Parameters

| Name   | Description               |
| ------ | ------------------------- |
| angle  | The angle in radians for which to calculate the hyperbolic cosine. |

#### Returns

The hyperbolic cosine of `angle`.

#### Example

```python
result = maths.cosh(0.5)
# Result: 1.12762596521
```

### `tanh(angle)`

Calculates the hyperbolic tangent of an angle.

#### Parameters

| Name   | Description               |
| ------ | ------------------------- |
| angle  | The angle in radians for which to calculate the hyperbolic tangent. |

#### Returns

The hyperbolic tangent of `angle`.

#### Example

```python
result = maths.tanh(0.5)
# Result: 0.46211715726
```
