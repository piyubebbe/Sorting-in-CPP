# Implementation of Sorting in C++

**Aim:** To study and implement sorting in C++  
**Software:** Mingw C/C++ compiler, VS Code, online C++ compiler  

---

## Program 1: Bubble Sort Using Pointer

### Theory with Explanation

- Bubble Sort compares adjacent elements and swaps them if they’re out of order.
- The array is traversed using pointer arithmetic, incrementing pointer addresses instead of indices.
- The outer loop controls the number of passes; the inner loop compares `*ptr` and `*(ptr+1)`.
- Swapping is performed via dereferencing: `*a`, `*b`.
- Using pointers provides low-level control and replaces array indexing.
- Sorting is in-place with space complexity O(1).
- Time complexity is O(n²) for worst and average cases.
- Efficient for embedded systems or memory-constrained environments.

#### Algorithm

1. Start
2. Repeat the sorting process for (n - 1) passes, where n is the array size.
3. In each pass, set a second pointer to the element next to the current one.
4. Compare the values pointed to by the two pointers.
5. If the first value is greater than the second, swap them using a temporary variable.
6. Move both pointers one step forward.
7. Continue comparing and swapping until the end of the unsorted portion.
8. After each pass, reduce the range of comparison by one.
9. Repeat steps until all elements are sorted.
10. End

---

## Program 2: Insertion Sort

### Theory with Explanation

- Insertion Sort builds the final sorted array one element at a time.
- It assumes the first element is already sorted.
- Each new element (key) is compared with the sorted portion to find its correct position.
- Larger elements are shifted right to make space for the key.
- Sorting is done in-place with space complexity O(1).
- Time complexity is O(n²) in worst and average cases, best case is O(n).
- Stable and preserves the relative order of equal elements.
- Efficient for small or nearly sorted datasets, easy to implement and understand.

#### Algorithm

1. Start
2. Store the current element as the key.
3. Compare the key with elements before it.
4. Shift all larger elements one position to the right.
5. Insert the key at its correct position.
6. Repeat for all elements.
7. End

---

## Program 3: Bubble Sort (Array-based)

### Theory with Explanation

- Bubble Sort compares adjacent elements and swaps them if they are out of order.
- Performs multiple passes until the array is sorted.
- Elements accessed and swapped via pointer dereferencing.
- swap() function exchanges values using pointers.
- Outer loop tracks number of passes; inner loop compares array[i] and array[i+1] using pointers.
- After each pass, the largest unsorted element bubbles to its correct position.
- Sorting is done in-place, space complexity O(1).
- Time complexity is O(n²) for worst and average cases.
- Simple, stable, and ideal for learning pointer manipulation.

#### Algorithm

1. Start
2. Input the number of elements and store in an array.
3. Initialize a counter to track completed passes.
4. Repeat the sorting process until all passes are done.
5. In each pass, compare adjacent elements using pointers.
6. If the first element is greater than the second, swap them.
7. Continue comparisons till the end of the unsorted portion.
8. Increment pass counter.
9. Repeat steps until the array is sorted.
10. Display the sorted array.
11. End

---

## Conclusion

The three sorting implementations—Bubble Sort with pointers, Bubble Sort with arrays, and Insertion Sort—demonstrate foundational techniques in algorithm design and memory manipulation. Bubble Sort with pointers emphasizes low-level control and pointer arithmetic, while the array-based version offers clarity and simplicity for beginners. Insertion Sort efficiently places elements and is ideal for nearly sorted data. All three are in-place and stable, making them memory-efficient and predictable. Though not optimal for large datasets, these algorithms are excellent for learning core sorting logic, control flow, and data movement. Together, they build strong intuition for algorithmic thinking and further exploration of more advanced methods.
