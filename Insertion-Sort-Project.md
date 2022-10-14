### [22,27,16,2,18,6] -> Insertion Sort

##### 1. Write the stages of the given array according to the sort type.

The algorithm moves forward over the array each time, takes one element of the array and sorts it one by one with the backward elements, and in each order, if it is smaller than the element it has sorted, it replaces it with that element and throws it back one by one.
   
since we are talking about the first number ( 22 ), it is ordered by itself. It continues without any action.
    
22 data and 27 data are compared. the first two data are completed when 22, 27 are small. Any changes are made.
    
it compares the number 16 with the one behind it, 16 is smaller than 27. he changes places from 16 to 27, that is, he swaps. Then he compares 16 and 22 again, 16 is also smaller than 22. it changes places from 16 to 22.
       
it compares 2 with a number behind 2, which is smaller than 27. he changes places from 2 to 27, that is, he swaps. Then he compares 2 with 22 again, 2 is also smaller than 22. it changes places from 2 to 22. Then again, 2 compares with 16, 2 is also smaller than 16. it changes places from 2 to 16.

it compares the number 18 with the one behind it, 18 is smaller than 27. he changes places from 18 to 27, that is, he swaps. Then again, 18 and 22 are compared, 18 is also smaller than 22. it changes places from 18 to 22. Then again, 18 compares with 16, 18 is also greater than 16. Any changes are made.
   
it compares the number 6 with the one behind 6, which is smaller than 27. it changes places from 6 to 27, so it makes a swap. Then again, 6 compares with 22, 6 is also smaller than 22. it changes places from 6 to 22. Then again, 6 compares with 18, 6 is also smaller than 18. it changes places from 6 to 18. Then again, 6 compares with 16, 6 is also smaller than 16. replaces 6 with 16
##### 2. Big-O gösterimini yazınız.

   O(n^2)

##### 3. Time Complexity: 
###### - Worst case: The number we are looking for is at the end.
An array given exactly the opposite, in which case each element of the array will be smaller than the one behind it. So the inner loop for the 1st element is 0, backward for the 2nd element is 1, 3. two for the element will then make the move back as far as 3 4 5 6...n. So 0+1+2+3+4…..+n-1 = [n*(n-1)]/2   :  n^2

###### - Average case: The number we are looking for is in the middle,
When we take the average of the worst case and the best case, we find "n^2".

###### - Best case: The number we are looking for is at the beginning of the series.
A fully ordered sequence passes through n numbers once, and remains with this single pass, since there is no need to move any of them backward. So n

##### 4. Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? 
since it is in the middle of the data set, it is covered by the average case.
    
#### 2. [7,3,5,8,2,9,4,15,6] write the first 4 steps of the sequence according to the Insertion Sort.
 |1.Step|7|3|5|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |2.Step|3|7|5|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |3.Step|3|5|7|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
 
 |4.Step|3|5|7|8|2|9|4|15|6|      
 |------|-|-|-|-|-|-|-|- |-|
