### [16,21,11,8,12,22] -> Merge Sort

#### 1. Write the stages of the above sequence according to the sort type.
###### Initially, we divide our series into two. We divide the dividing sequences again. We continue the process until only one element remains.

|                                                       |  |  |  |  |  |  |  |  |  |  |  |  |
|-------------------------------------------------------|- |- |- |- |- |- |- |- |- |- |- |- |
|We rewrite the series by dividing it in half.          |  |  |  |16|21|11|8 |12|22|  |  |  |
|                                                       |  |  |  |  |  |  |  |  |  |  |  |  |
|We divide the left and right rows into two again.      |  |  |16|21|11|  |  |8 |12|22|  |  |
|                                                       |  |  |  |  |  |  |  |  |  |  |  |  |
|We divide it once more until only one element remains. |  |16|21|  |11|  |  |8 |  |12|22|  |
|                                                       |  |  |  |  |  |  |  |  |  |  |  |  |
|                                                       |16|  |21|  |11|  |  |8 |  |12|  |22|


######  After the splitting process is finished, we combine our single-element arrays into binary binary. We continue this process until we get an ordered array.

|                                                       |  |  |  |  |  |  |  |  |  |  |  |  |
|-------------------------------------------------------|- |- |- |- |- |- |- |- |- |- |- |- |
|                                                       |16|  |21|  |11|  |  |8 |  |12|  |22|
|                                                       |  |  |  |  |  |  |  |  |  |  |  |  |
|We combine binary binary binary by sorting.            |  |16|21|  |11|  |  |8 |  |12|22|  |
|                                                       |  |  |  |  |  |  |  |  |  |  |  |  |
|We combine it again by sorting binary-binary.          |  |  |11|16|21|  |  |8 |12|22|  |  |
|                                                       |  |  |  |  |  |  |  |  |  |  |  |  |
|At the last combine, we get our sequence.              |  |  |  |8 |11|12|16|21|22|  |  |  |
    

#### 2. Write the Big-O notation.
Since it is a recursive function, it always divides the array into two by constantly calling itself. For the Merge operation of each split array, it will be O(n*(log n)) --> O(6*(log6)), since n operations are performed, which is the length of the array.
