# Sorting-Algorithms-of-Cpp
# Name: Rajeev Ramesh Reddy E
#PRN: 24070123081

Aim:

To implement and understand various sorting algorithms using C++, analyze their time and space complexities, and compare their performance based on different input sizes.

Software Used: Vs Code

Theory:

Sorting algorithms in C++ are techniques used to arrange data in a specific order, typically ascending or descending. Common algorithms include Bubble Sort, Selection Sort, Insertion Sort, Merge Sort, and Quick Sort. Each has different time and space complexities, making them suitable for various scenarios. Sorting improves data organization, search efficiency, and overall program performance. In C++, sorting can be implemented manually using loops and conditions or via built-in functions like `sort()` from the STL. Understanding sorting logic enhances algorithmic thinking and prepares programmers for advanced topics like searching, optimization, and data structure manipulation.


Algorithm:

i) Algorithm: Quick Sort in C++

 1. Choose a Pivot
- In the `partition()` function, select the last element of the array (`arr[high]`) as the pivot.

 2. Rearrange Elements
- Traverse the array from `low` to `high - 1`.
- If an element is less than the pivot, increment `i` and swap `arr[i]` with `arr[j]`.

 3. Final Pivot Placement
- After the loop, swap `arr[i + 1]` with the pivot to place it in its correct sorted position.
- Return the pivot index `i + 1`.

 4. Recursive Sorting
- In `quickSort()`, recursively sort the subarrays:
  - Left: `low` to `pi - 1`
  - Right: `pi + 1` to `high`

 5. Display Result
- In `main()`, call `quickSort()` on the full array.
- Print the sorted array using a loop.

ii) Algorithm: Selection Sort in C++

 1. Traverse the Array
- Use a loop from index `0` to `size - 2` to iterate through each element.

 2. Find Minimum Element
- For each position `i`, find the index `minIdx` of the smallest element in the unsorted portion (`i+1` to `size - 1`).

 3. Swap Elements
- Swap the element at index `i` with the element at `minIdx` to place the minimum at its correct position.

 4. Repeat for All Positions
- Continue the process for all positions until the array is sorted.

 5. Display Sorted Array
- In `main()`, call `selectionSort()` and print the sorted array using a loop.

iii)  Algorithm: Bubble Sort in C++

 1. Traverse the Array
- Use an outer loop from `i = 0` to `size - 2` to control the number of passes.

 2. Compare Adjacent Elements
- Use an inner loop from `j = 0` to `size - i - 2` to compare each pair of adjacent elements.

 3. Swap if Out of Order
- If `arr[j] > arr[j + 1]`, swap the two elements to move the larger one toward the end.

 4. Repeat Passes
- Continue the process for all passes until the array is sorted.

 5. Display Sorted Array
- In `main()`, call `bubbleSort()` and print the sorted array using a loop.

Conclusion: 

Sorting algorithms in C++ are vital for organizing data efficiently. Techniques like Bubble, Selection, and Quick Sort enhance understanding of control flow, comparisons, and optimization. Mastering these builds a strong foundation for advanced programming, enabling faster data access, better performance, and cleaner logic in real-world applications and competitive coding.
