# Tids og størrelses kompleksitet

## O thetha and omega notation

![image](https://media.geeksforgeeks.org/wp-content/cdn-uploads/mypic.png)

| S.No.| Big O                                                                                                                                                                | Big Omega&nbsp;(Ω)                                                                                                                                             | Big Theta&nbsp;(Θ)                                                                                                                            |
|---------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
| 1.      | It is like (&lt;=)&nbsp;rate of growth of an algorithm is less than or equal to a specific value.&nbsp;                                                              | It is like (&gt;=)&nbsp;rate of growth is greater than or equal to a specified value.                                                                          | It is like (==)&nbsp;meaning the rate of growth is equal to a specified value.                                                                |
| 2.      | The upper bound of algorithm is represented by Big O notation. Only the above function is bounded by Big O. Asymptotic upper bound is &nbsp;given by Big O notation. | The algorithm’s lower bound is represented by Omega notation. The asymptotic lower bound is given by Omega notation.                                           | The bounding of function from above and below is represented by theta notation. The exact asymptotic behavior is done by this theta notation. |
| 3.      | Big O – Upper Bound                                                                                                                                                  | Big Omega (Ω) – Lower Bound                                                                                                                                    | Big Theta (Θ) – Tight Bound                                                                                                                   |
| 4.      | It is define as upper bound and upper bound on an algorithm is the most amount of time required ( the worst case performance).                                       | It is define as lower bound and lower bound on an algorithm is the least amount of time required ( the most efficient way possible, in other words best case). | It is define as tightest bound and tightest bound is the best of all the worst case times that the algorithm can take.                        |
| 5.      | Mathematically: Big Oh is 0 &lt;= f(n) &lt;= Cg(n) for all n &gt;= n0                                                                                                | Mathematically: Big Omega is 0 &lt;= Cg(n) &lt;= f(n) for all n &gt;= n0                                                                                       | Mathematically – Big Theta is 0 &lt;= C2g(n) &lt;= f(n) &lt;= C1g(n) for n &gt;= n0                                                           |

## rekursive funktioner
rekursive funtioner er funktioner der indeholder sig selv. fx:
t(n) = 1+t(2/n)

## Master Theorem
![Master Theorem](https://i.imgur.com/coKFB7D.png)

## algoritme cheat sheet

| Algorithm      | Best Case | Average Case | Worst Case |
|----------------|-----------|--------------|------------|
| Selection Sort | O(n^2)    | O(n^2)       | O(n^2)     |
| Bubble Sort    | O(n)      | O(n^2)       | O(n^2)     |
| Insertion Sort | O(n)      | O(n^2)       | O(n^2)     |
| Tree Sort      | O(nlogn)  | O(nlogn)     | O(n^2)     |
| Radix Sort     | O(dn)     | O(dn)        | O(dn)      |
| Merge Sort     | O(nlogn)  | O(nlogn)     | O(nlogn)   |
| Heap Sort      | O(nlogn)  | O(nlogn)     | O(nlogn)   |
| Quick Sort     | O(nlogn)  | O(nlogn)     | O(n^2)     |
| Bucket Sort    | O(n+k)    | O(n+k)       | O(n^2)     |
| Counting Sort  | O(n+k)    | O(n+k)       | O(n+k)     |

