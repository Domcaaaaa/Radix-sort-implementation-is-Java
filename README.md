# RadixSort Implementation in Java

## Description
This repository contains a Java implementation of the **Radix Sort** algorithm, a non-comparative sorting algorithm that sorts numbers by processing individual digits.

## Features
- Implements **Radix Sort** using **Counting Sort** as a subroutine.
- Sorts an array of integers in ascending order.
- Demonstrates the sorting process with a sample array.

## How It Works
Radix Sort works by sorting numbers digit by digit, from the least significant digit to the most significant. The algorithm uses Counting Sort as a stable sorting technique at each digit level.

## Usage
### Prerequisites
- Java Development Kit (JDK) installed.

### Running the Script
1. Clone this repository or download the `RadixSort.java` file.
2. Open a terminal or command prompt in the directory where `RadixSort.java` is located.
3. Compile the Java file using:
   ```sh
   javac RadixSort.java
   ```
4. Run the program using:
   ```sh
   java RadixSort
   ```

## Example Output
```
Before sorting
[122, 431, 565, 22, 1, 47, 787]
After sorting
[1, 22, 47, 122, 431, 565, 787]
```

## Code Structure
- `radixsort(int[], int)`: Main function that sorts the array using Radix Sort.
- `countingsort(int[], int, int)`: Helper function that sorts numbers based on a specific digit using Counting Sort.

## Complexity Analysis
- **Time Complexity**: O(d * (n + k)) where:
  - `d` is the number of digits in the largest number,
  - `n` is the number of elements in the array,
  - `k` is the range of digits (0-9).
- **Space Complexity**: O(n) due to the temporary arrays used in Counting Sort.
