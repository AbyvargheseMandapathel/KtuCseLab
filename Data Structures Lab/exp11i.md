**S3 Datastructures Lab\
Experiment 11**
-----------------------------------------------------------------

Question:
Implementation of bubble sort

Solution:
How it's done?
Bubble sort algorithm starts by comparing the first two elements of an array and swapping if necessary, i.e., if you want to sort the elements of array in ascending order and if the first element is greater than second then, you need to swap the elements but, if the first element is smaller than second, you mustn't swap the element. Then, again second and third elements are compared and swapped if it is necessary and this process go on until last and second last element is compared and swapped. This completes the first step of bubble sort.

If there are n elements to be sorted then, the process mentioned above should be repeated n-1 times to get required result. But, for better performance, in second step, last and second last elements are not compared becuase, the proper element is automatically placed at last after first step. Similarly, in third step, last and second last and second last and third last elements are not compared and so on

Refer to the program!


Input and Output
----------------
Enter the number of elements to be sorted: 6
1. Enter element: 12
2. Enter element: 3
3. Enter element: 0
4. Enter element: -3
5. Enter element: 1
6. Enter element: -9
In ascending order: -9 -3 0 1 3 13

--------------------------------------------------------------------

