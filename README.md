# Luhn Algorithm Validator

## Overview
This project is a simple **Luhn Algorithm Validator** implemented in Python. The Luhn algorithm, also known as the **modulus 10 algorithm**, is a widely used checksum formula to validate credit card numbers and other identification numbers.

This project was developed as part of the **'Scientific Computing with Python' certification** on **freeCodeCamp**, where I learned **string manipulation techniques** and applied them to implement this algorithm.

## Features
- Implements the **Luhn Algorithm** to verify card numbers.
- Handles input with **hyphens (`-`) or spaces (` `)** by removing them before processing.
- Uses **string manipulation techniques**, including `str.maketrans()` and `.translate()`.
- Works with **any card number** input as a string.
- Provides **clear output** indicating whether the card number is valid or not.

## How It Works
1. The input card number is **cleaned** by removing `-` and spaces.
2. The number is **processed using the Luhn Algorithm**, where:
   - Digits in **odd positions** (from the right) are summed directly.
   - Digits in **even positions** are **doubled**, and if the result is greater than `9`, the digits of the product are summed.
   - The total sum is calculated, and if it is divisible by `10`, the card number is **valid**.
3. The program prints **VALID!** or **INVALID!** based on the result.

## Code Example
```python
card_number = '4111-1111-4555-1142'  # Example input
```

### Sample Output
```
VALID!
```
