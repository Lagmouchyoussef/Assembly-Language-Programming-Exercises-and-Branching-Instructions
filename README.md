**Exercise 1:**

Write an assembly program to calculate the sum of an array.

**Exercise 2:**

Write an assembly program to find the maximum value in a given array.

**Exercise 3:**

Write an assembly program to find the minimum value in a given array.

**Exercise 4:**

Write an assembly program to calculate the sum of even numbers.

**Exercise 5:**

Write a program to find the position of a given number in an array.

**Exercise 6:**

Write a program to transfer positive or zero elements from array T to array TPositif and negative elements from T to array TNegatif.

**Exercise 7:**

Write a program to reverse an array.

### 4.5 Branching Instructions

Three types of branching are possible:

- Unconditional branches
- Conditional branches
- Function calls or interrupts

#### 4.5.1 Unconditional Branching

`JMP xyz` Causes an unconditional jump to the line labeled xyz.

`CALL xyz` Calls a procedure (subroutine) starting at the line xyz. The position of the instruction following the CALL is pushed onto the stack to ensure correct continuation after the subroutine execution.

#### 4.5.2 Conditional Branching

Conditional branches depend on the state of the flags (indicators) which are set by previous instructions.
In the following, we will use the terminology:
- **greater than** or **less than** for unsigned numbers
- **smaller than** or **larger than** for signed numbers
- `+` for the logical OR operator

`JE/JZ xyz` (Jump if Equal or Zero) Jump to line xyz if result is zero or if equal. That is, if Z=1.

`JNE/JNZ xyz` (Jump if Not Equal or Not Zero) Jump to line xyz if result is non-zero or if different. That is, if Z=0.

`JA xyz` (Jump if Above) Jump to line xyz if greater than (unsigned). That is, if C + Z = 0.

`JAE xyz` (Jump if Above or Equal) Jump to line xyz if greater than or equal (unsigned). That is, if C = 0.

`JB xyz` (Jump if Below) Jump if less than (unsigned). That is, if C = 1.

`JBE xyz` (Jump if Below or Equal) Jump to line xyz if less than or equal (unsigned). That is, if C + Z = 1.
