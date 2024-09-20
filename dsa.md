# JavaScript Accelerator Assessment

You should be able to do something in real time that reflects some level of competence with JavaScript.

## The bar for an accelerator fellow:

1. Write functions that accept parameters
2. Read problems and understand their inputs and outputs
3. Be decently familiar with JS's library of constructor methods (Math, String, Array, Object)
4. Be decently familiar with JS keywords (while, for, typeof, return)

The following problems do not need to be solved completely to show someone is ready for the accelerator class. The first and possibly second variations of a problem should be enough to indicate someone is ready.

## Problems for accelerator assessment:

### 1. Find the nth largest number of an array of integers

There can be duplicates in the array, and those duplicates do not count towards nth largest number.

**Constraints:**

- Arr.length >= 0
- n >= 0 <= arr.length

**Example 1:**

- **Input**: [], 1
- **Output**: null

**Example 2:**

- **Input**: [5,4,1], 1
- **Output**: 5

**Example 3:**

- **Input**: [5,4,1], 2
- **Output**: 4

**Example 4:**

- **Input**: [2,5,5], 2
- **Output**: 2

### 2. Vowel Remover

[Codewars: Vowel Remover](https://www.codewars.com/kata/5547929140907378f9000039)

### 3. Merge Two Objects

Write a function that takes in two objects and returns a new object that has all of the properties of both objects. Both objects have non-overlapping properties.

**Example 1:**

- **Input**: {}, {}
- **Output**: {}

**Example 2:**

- **Input**: {a: true}, {}
- **Output**: {a: true}

**Example 3:**

- **Input**: {a:true}, {a: false}
- **Output**: {a:false}

**Example 4:**

- **Input**: {a: {}, c: '!'}, {g: 2}
- **Output**: {a: {}, c: '!', g: 2}

### 4. Length of Last Word

[LeetCode: Length of Last Word](https://leetcode.com/problems/length-of-last-word/)

### 5. Palindrome Check

Write a function that accepts a string as a parameter and returns whether or not that string is a palindrome. The string only contains lowercase letters.

**Constraints:**

- Str.length >= 0

**Example 1:**

- **Input**: 'a'
- **Output**: true

**Example 2:**

- **Input**: 'ab'
- **Output**: false

**Example 3:**

- **Input**: 'bb'
- **Output**: true

**Example 4:**

- **Input**: 'ceec'
- **Output**: true

**Example 5:**

- **Input**: ''
- **Output**: true

### 6. Object Key Search

Write a function that looks through a provided object that has an unknown level of nesting in it (its values could have objects that have values that contain objects). Return a boolean whether or not the key "pursuit" exists in any object inside of the provided object.

**Example 1:**

- **Input**: {block: 'scope'}
- **Output**: false

**Example 2:**

- **Input**: {block: 'scope', pursuit: 'austell'}
- **Output**: true

**Example 3:**

- **Input**: {block: 'scope', other: {pursuit: 'place'}}
- **Output**: true

**Example 4:**

- **Input**: {block: 'scope', other: {pursu: {hello: 'hi', nest: {} }, }}
- **Output**: false

**Example 5:**

- **Input**: {}
- **Output**: false

### 7. (Hard) Mathematical Operations

Write a function that takes 3 parameters, two numbers and a string representing an operation symbol('+', '-', '\*', '/') and returns the output of running the given operation on the two numbers. All decimals should be rounded down to the nearest whole number. None of the test cases will have division by zero. All of the numbers will be integers.

**Example 1:**

- **Input**: 3, 2, '+'
- **Output**: 5

**Example 2:**

- **Input**: 2, 3, '-'
- **Output**: -1

**Example 3:**

- **Input**: 2, 3, '/'
- **Output**: 0

#### 7b) String of Operations

Write a function that takes a string of space-separated numbers and operations and returns the result of running all of the operations from left to right. All decimals should be rounded down to the nearest whole number. None of the test cases will have division by zero. All of the numbers will be integers in the test cases.

**Note**: All strings will be valid (number + space + operation + number).

**Example 1:**

- **Input**: '2 + 4 \* 3'
- **Output**: 18 (not 14 in this case because 2 + 4 = 6 and 6 \* 3 = 18)

**Example 2:**

- **Input**: '10 \* 5 / 3'
- **Output**: 16

**Example 3:**

- **Input**: '5 - 5 \* 10'
- **Output**: 0

**Example 4:**

- **Input**: '1 - 3 + 15 - 6 \* 2'
- **Output**: 14
