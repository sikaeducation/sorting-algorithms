# Sorting Algorithms

## List four common sorting algorithms

Identifies at least four sorting algorithms from the following list: bubble, merge, quick, insertion, selection, heap, shell, or radix

>Common sorting algorithms include Bubble, Merge, Quick, Insertion, and Selection sort.

## Discuss code implementation for bubble sort

Correctly highlights key operations in bubble sort:

* Looping through the list
* For each item, compare the current value with the in the list
* Swap values if needed

>Bubble sort repeatedly steps through the list to be sorted, compares each pair of adjacent items and swaps them if they are in the wrong order.

## Discuss the time complexity of bubble sort

Correctly identifies the complexity of O(n^2):

* The complexity is directly related to the size of the input 
* Describes bubble sort going through the list twice

>Bubble sort has a time complexity of O(n^2). `n` represents the length of the input. For each item on the list (n), worst case scenario, Bubble sort will step through the whole list again (n * n).

## Identify the following sorting algorithm

![Sorting algorithm visualization](assets/sorting.gif)

* Identifies the sorting algorithm as insertion sort

>The gif displays a graphical example of insertion sort.

## Describe the difference between insertion and selection sort

Describes key differences between insertion and selection sort:

* Insertion builds a new sorted list
* Selection sorts the array in place
* Insertion places the current value in the right order as it loops
* Selection loops to find the next value and swaps it to the correct location

>Insertion and Selection sort are similar but have a few key differences: Insertion builds a new sorted list, selection sorts the array in place. Insertion places the current value in the right order as it loops, selection loops to find the next value and swaps it to the correct location.

## Discuss the time complexity of selection sort

Correctly identifies the complexity of O(n^2):

* The complexity is directly related to the size of the input 
* Describes selection sort going through the list twice

>Selection sort has a time complexity of O(n^2). `n` represents the length of the input. For each item on the list (n), Selection sort will step through the list to find the lowest value and place it in the right order (n - 1 comparisons). As it loops through the list, the comparisons will be less (n - 2, n - 3...) but this gets simplified to n, making the complexity (n^2)

## Discuss common uses of sorting algorithms in programming

Correctly highlights two of the following uses of sorting algorithms in programming:

* **Presentation** - Data is commonly viewed in a sorted manner
* **Searching** - It is more efficient to search through a list when it is sorted
* **Element Uniqueness** - It is easier find duplicate data when a list is sorted
* **Data analysis** - Sorting is used to figure out frequency, median, etc. 

>Sorting is commonly done to change the presentation order of data. Sorted data is easier to search through as well, to find duplicates or unique elements, and to do data analysis.

## Describe Quick or Merge Sort

Quick Sort: Similar to Selection Sort, Quick Sort implements in-place sorting. 

* It picks a pivot from the list
* It partitions the values, placing lower values to one side and higher values on the other
* Repeats the process recursively for the sub lists left and right of the pivot

>Quick Sort will partition the list into two equal pieces repeatedly, each time called on a list half the size (log(n) complexity). The process of partitioning (moving items left or right of the pivot) at each level will require operations the size of the list `n` in the worst case scenario, making the sorting algorithm O(n * log(n))

Merge Sort: Similar to Quick Sort, Merge Sort is a divide and conquer algorithm.

* It divides the list into `n` sublists. `n` being the size of the input
* Merges two sublists together in a sorted manner
* Repeates the process recursively until there is one sorted sublist left

## Discuss the time complexity of Quick or Merge Sort

Correctly identifies the complexity of O(n log(n)) for Quick Sort or Merge Sort

*  Quick Sort will partition the list into two equal pieces repeatedly, each time called on a list half the size (log(n) complexity). The process of particioning (moving items left or right of the pivot) at each level will require operations the size of the list `n` in the worst case scenario, making the sorting algorithm O(n * log(n)).  
* Merge Sort will divide the list into sublists at a log(n) complexity since it is half-ing the list every iteration. The merging of `n` sublists items takes O(n) time, making the sorting complexity O(n * log(n)) 

## Which sorting algorithm is most efficient to sort a nearly sorted array in ascending order, such as `[1,2,8,3,4,5,6,7,9,10]`

Since most items are in the right order, Insertion sort will require fewer swaps and comparisons as it loops through the list.

Selects Bubble or Insertion sort as the most efficient algorithm for a nearly sorted array

* Since most items are in the right order, Insertion sort will require fewer swaps and comparisons as it loops through the list
* Since most items are in the right order, Bubble sort will require to swap only a few items and ignore the items already in place.
* Quick and merge sort will perform a similar operation regardless of how sorted the list is. 
