# Polygon-3

## Circuit Description

This is a simple digital circuit designed using the `circom` language. The circuit implements logical operations such as AND, OR, and NOT gates to compute the output based on input signals `a` and `b`.

## Components:

### AND Gate
- Input: `x`, `y`
- Output: `out`
- Truth Table:
  - 0 AND 0 = 0
  - 0 AND 1 = 0
  - 1 AND 0 = 0
  - 1 AND 1 = 1

### NOT Gate
- Input: `in`
- Output: `out`
- Truth Table:
  - NOT 0 = 1
  - NOT 1 = 0

### OR Gate
- Input: `x`, `y`
- Output: `out`
- Truth Table:
  - 0 OR 0 = 0
  - 0 OR 1 = 1
  - 1 OR 0 = 1
  - 1 OR 1 = 1

## Circuit Template

The circuit template consists of interconnecting these gates to perform logical operations.

- Input Signals: `a`, `b`
- Intermediate Signals: `x`, `y`
- Output Signal: `q`

The circuit follows this logical sequence:
1. `AND` gate computes the conjunction of input signals `a` and `b`, resulting in signal `x`.
2. `NOT` gate negates input signal `b`, resulting in signal `y`.
3. `OR` gate computes the disjunction of signals `x` and `y`, resulting in the output signal `q`.

## How to Use

To use this circuit, follow these steps:
1. Define your input signals `a` and `b`.
2. Connect the input signals to the `main` component.
3. Execute the circuit using a compatible compiler or interpreter for `circom`.

---

Make sure to include any additional instructions or details specific to your application or environment.
