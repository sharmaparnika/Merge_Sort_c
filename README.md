# Merge Sort in C

Merge sort is similar to the quick sort algorithm as it uses the divide and conquer approach to sort the elements. It is one of the most popular and efficient sorting algorithm. It divides the given list into two equal halves, calls itself for the two halves and then merges the two sorted halves. We have to define the merge() function to perform the merging.

The sub-lists are divided again and again into halves until the list cannot be divided further. Then we combine the pair of one element lists into two-element lists, sorting them in the process. The sorted two-element pairs is merged into the four-element lists, and so on until we get the sorted list.

### Algorithm for Merge Sort:


*    **Step 1:**  Find the middle index of the array.

        **Middle** = 1 + (last – first)/2

*    **Step 2:** Divide the array from the middle.

*    **Step 3:** Call merge sort for the first half of the array

       MergeSort(array, first, middle)

*    **Step 4:** Call merge sort for the second half of the array.

       MergeSort(array, middle+1, last)

*    **Step 5:** Merge the two sorted halves into a single sorted array.


### Merge Sort Complexity
Now, let's see the time complexity of merge sort in best case, average case, and in worst case. We will also see the space complexity of the merge sort.

1. **Time Complexity**

 | Case | Time Complexity |
 | --- | --- |
 | `Best Case` | **O(n(logn))** |
 | `Average Case` | **O(n(logn))** |
 | `Worst Case` | **O(n(logn))** |

**Quick Glimpse:**

*     Best Case Complexity - It occurs when there is no sorting required, i.e. the array is already sorted. The best-case time complexity of merge sort is O(n(logn)).

*     Average Case Complexity - It occurs when the array elements are in jumbled order that is not properly ascending and not properly descending. The average case time complexity of merge sort is O(n(logn)).

*     Worst Case Complexity - It occurs when the array elements are required to be sorted in reverse order. That means suppose you have to sort the array elements in ascending order, but its elements are in descending order. The worst-case time complexity of merge sort is O(n(logn)).

2. **Space Complexity**

      | Space Complexity | O(n) |
      | --- | --- |
      | `Stable` | **YES** |
      
 **Please Note** - The space complexity of merge sort is O(n). It is because, in merge sort, an extra variable is required for swapping.
 
 **Output:**
 
 ![image](https://user-images.githubusercontent.com/73773202/151399518-3e76efd4-8b09-40d1-87da-aaa8496f8e48.png)


---
