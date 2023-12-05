
```markdown
# QuickSort2 Implementation

Welcome to the QuickSort2 program! This Java program demonstrates the implementation of the QuickSort algorithm with a modification using the median of three as the pivot. The program includes counting the total number of copy and comparison operations performed during the sorting process.

## Usage

1. **Initialize Array**: Modify the `ab` array in the `QuickSort2` class with your desired set of integers.

2. **Run the Program**: Execute the `main` method in the `QuickSort2` class.

3. **View Results**: The program will print the original array, perform the QuickSort algorithm, and print the sorted array along with the total counts of copy and comparison operations.

## Modifications

- The QuickSort algorithm has been modified to use the median of three as the pivot for improved efficiency.
- The program prints the original and sorted arrays, along with the total counts of copy and comparison operations.

## Difference from Normal QuickSort

The primary difference lies in the choice of the pivot during the partitioning step. Instead of always choosing the last element as the pivot (as in normal QuickSort), QuickSort2 uses the median of three elements (left, middle, and right) to reduce the likelihood of choosing a poor pivot.

### Key Differences:

1. **Pivot Choice**: QuickSort2 uses the median of three values (left, middle, and right) as the pivot, aiming to improve pivot selection.

2. **Efficiency**: The modification aims to enhance the overall efficiency of the QuickSort algorithm, particularly for certain edge cases.

## Example

```java
public class QuickSort2Main {

    public static void main(String[] args) {
        QuickSort2.printArray();
        QuickSort2.quickSort(0, QuickSort2.ab.length - 1);
        QuickSort2.printArray();
        System.out.println("Total Copies: " + QuickSort2.copyCount);
        System.out.println("Total Comparisons: " + QuickSort2.comparisonCount);
        int totalCount = QuickSort2.comparisonCount + QuickSort2.copyCount;
        System.out.println("Total Operations: " + totalCount);
    }
}
```

## Contributing

Feel free to contribute by forking the repository, making changes, and submitting a pull request. Your feedback and improvements are welcome!

## License

This project is licensed under the [MIT License](LICENSE). Use it, modify it, and share it as needed.
```

Feel free to adjust the content based on your preferences or additional details you'd like to include.
