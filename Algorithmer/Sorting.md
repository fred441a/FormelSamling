# Sorterings algorithmer

## Heapsort
Max-Heapify sort
seudo kode
A er arrayet vores Heap er gemt i
i er vores index i heap
```
Max-Heapify (A, i)

l = LEFT(i) 
r = RIGHT(i)

if l <= A.heap-size and A[l] > A[i]
    largest = l
else largest = i
if r <= A.heap-size and A[r] > A[largest]
    largest = r
if largest != i
    exchange A[largest] and A[i]
    Max-Heapify(A,largest)
```

Min-Heapify sort
seudo kode
```
Min-Heapify (A, i)

l = LEFT(i) 
r = RIGHT(i)

if l <= A.heap-size and A[l] < A[i]
    smallest = l
else smallest = i
if r <= A.heap-size and A[r] < A[largest]
    smallest = r
if smallest != i
    exchange A[smallest] and A[i]
    Min-Heapify(A,smallest)
```

## Quick sort
Quick sort is a divide and conquor algoritme

seudo kode:
A er det array der skal sorteres
p er vores første indgang i arrayet
r er den sidste indgang i arrayet
```
Quicksort(A,p,r)
if p < r
    q = Partition(A,p,r)
    Quicksort(A,p,q-1)
    Quicksort(A,q+1,r)

Partition(A,p,r)
x=A[r]
i=p-1
for j = p to r-1
    if A[j] <= x
        i = i+1 
        exchange A[i] with A[j]
exchange A[i+1] with A[r]
return i+1
```
## Count sort

```
Counting sort(A,n,k)
let B[1:n] and C[0:k]
for i = 0 to k
    C[i] = i
for j = 1 to n
    C[A[j]] = C[A[j]] + 1


```

## Radix sort
in radix sort you sort the numbers by the smallest digit first.

hvis alle tal i arrayet har lige mange digits er radix sort O(n)

## Bucket sort
O(n²)
MEN!
Big Theta på (n)
**SHITTY SUDO CODE **

!(shitty code)[https://i.imgur.com/1U8EpXe.png]
Legit den her kode er så dårligt skrevet at den legit ikke giver mening. så her er den lige i C++ \/

```
// Function to sort arr[] of
// size n using bucket sort
void bucketSort(float arr[], int n)
{
 
    // 1) Create n empty buckets
    vector<float> b[n];
 
    // 2) Put array elements
    // in different buckets
    for (int i = 0; i < n; i++) {
 
        // Index in bucket
        int bi = n * arr[i];
        b[bi].push_back(arr[i]);
    }
 
    // 3) Sort individual buckets
    for (int i = 0; i < n; i++)
        sort(b[i].begin(), b[i].end());
 
    // 4) Concatenate all buckets into arr[]
    int index = 0;
    for (int i = 0; i < n; i++)
        for (int j = 0; j < b[i].size(); j++)
            arr[index++] = b[i][j];
}
```
