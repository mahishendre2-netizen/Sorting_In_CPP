# Sorting_In_CPP
# Aim
To study and implement sorting methods in C++.

# Theory
Sorting in C++ involves arranging elements within a data structure, such as an array or vector, in a specific order (e.g., ascending or descending). C++ provides various methods for sorting, including built-in functions and custom implementations of sorting algorithms.

# Selection Sort
It is a comparison-based sorting algorithm. It sorts an array by repeatedly selecting the smallest (or largest) element from the unsorted portion and swapping it with the first unsorted element. This process continues until the entire array is sorted.

First we find the smallest element and swap it with the first element. This way we get the smallest element at its correct position.

Then we find the smallest among remaining elements (or second smallest) and swap it with the second element.

We keep doing this until we get all elements moved to correct position.

# Bubble Sort
It is the simplest sorting algorithm that works by repeatedly swapping the adjacent elements if they are in the wrong order. This algorithm is not suitable for large data sets as its average and worst-case time complexity are quite high.

We sort the array using multiple passes. After the first pass, the maximum element goes to end (its correct position). Same way, after second pass, the second largest element goes to second last position and so on.

In every pass, we process only those elements that have already not moved to correct position. After k passes, the largest k elements must have been moved to the last k positions.

In a pass, we consider remaining elements and compare all adjacent and swap if larger element is before a smaller element. If we keep doing this, we get the largest (among the remaining elements) at its correct position.

# Insertion sort
It is a simple sorting algorithm that works by iteratively inserting each element of an unsorted list into its correct position in a sorted portion of the list. It is like sorting playing cards in your hands. You split the cards into two groups: the sorted cards and the unsorted cards. Then, you pick a card from the unsorted group and put it in the right place in the sorted group.

We start with the second element of the array as the first element is assumed to be sorted.

Compare the second element with the first element if the second element is smaller then swap them.

Move to the third element, compare it with the first two elements, and put it in its correct position

Repeat until the entire array is sorted.

Algorithms
# Selection Sort
Start.

Input n (size of array).

Input n elements into the array.

For i = 0 to n-2:

Set minIndex = i.

For j = i+1 to n-1: If arr[j] < arr[minIndex], update minIndex = j.

Swap arr[i] and arr[minIndex].

Display the sorted array.

End.

# Insertion Sort
Start.

Input n (size of array).

Input n elements into the array.

For i = 1 to n-1:

Set key = arr[i].

Set j = i - 1. While j >= 0 and arr[j] > key: Shift arr[j] to arr[j+1]. Decrement j.

Place key at arr[j+1].

Display the sorted array.

End.

Bubble Sort
Start.

Input n (size of array).

Input n elements into the array.

For i = 0 to n-2:

Set swapped = false.

For j = 0 to n-i-2:

If arr[j] > arr[j+1]:

Swap arr[j] and arr[j+1].

Set swapped = true.

If swapped = false, break (array already sorted).

Display the sorted array.

End.

# Conclusion
We learnt to implememnt different sorting methods in C++.
