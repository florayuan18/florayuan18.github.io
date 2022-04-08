---
layout: page
title: Week 3 - Sorts
subtitle: Flora Yuan
---
## Challenges
**Week 3 - Sorts**

Challenges:
* Sort and Analysis and see which one is most efficient
* Run each sort 12 times on 5000+ elements
* Throw out high and low

## Code Snippets
```javascript
for (int i = 0; i < arr.length - 1; i++)
{
    int index = i;
    for (int j = i + 1; j < arr.length; j++){
    if (arr[j] < arr[index]){
        index = j;//searching for lowest index
    }
}
    int smallerNumber = arr[index];
    arr[index] = arr[i];
    arr[i] = smallerNumber;
}
```

* Selection Sort --> This is the actual sorting function, which searches for the lowest index in order to figure out where the next element should go in the order.

```javascript
int[] arr = new int[myArray.size()];
for (int m = 0; m < myArray.size(); m++)
{
    arr[m] = myArray.get(m);
}

//2. insertion sorting
int n = arr.length;
for (int j = 1; j < n; j++)
{
    int key = arr[j];
    int i = j-1;
    while ( (i > -1) && ( arr [i] > key ) )
    {
        arr [i+1] = arr [i];
        i--; // decrement
    }
    arr [i+1] = key;
}
```

* Insertion Sort --> This part of the code is assigning myArray elements to the array int[] arr.  The second part is the actual sorting function that figures out where the element belongs.

```javascript
void merge(int a[], int beg, int mid, int end)
    {
        int i, j, k;
        int n1 = mid - beg + 1;
        int n2 = end - mid;

        // temporary Arrays
        int LeftArray[] = new int[n1];
        int RightArray[] = new int[n2];

        // copy data to temp arrays
        for (i = 0; i < n1; i++)
            LeftArray[i] = a[beg + i];
        for (j = 0; j < n2; j++)
            RightArray[j] = a[mid + 1 + j];

        i = 0; // initial index of first sub-array
        j = 0; // initial index of second sub-array
        k = beg;  // initial index of merged sub-array
```

* Merge Sort --> For this, I referenced temporary arrays and copied data into those temporary arrays that would then be merged to sort.

```javascript
        int n = arr.length;
        int temp = 0;
        for(int i=0; i < n; i++)
        {
            for(int j=1; j < (n-i); j++)
            {
                if(arr[j-1] > arr[j])
                {
                    //swap elements
                    temp = arr[j-1];
                    arr[j-1] = arr[j];
                    arr[j] = temp;
                }
            }
        }
```

* Bubble Sort --> This sort simply repeatedly swaps the adjacent elements if they are in the wrong order.  This function figures out the order of the elements and does just this.

* I think what I learned most about this was the idea of using tester data.  Since the requirement was to use 5000+ elements, it looked very clustered and hard to read.  So, I often changed it to use 10 variables before I committed in order to make sure that the function I wrote worked.  I also opted to print the array before the sort and after the sort, just to make sure that it worked.  I think this helped me check my work, and it is definitely something I will employ in the future.

![sortssheet.png](/assets/img/sortssheet.png)

## GitHub
[Selection Sort](https://github.com/florayuan18/just-to-suffer/commit/e0d12f57f7421fadfd713953d2ad0fbe84752462)
[Insertion Sort](https://github.com/florayuan18/just-to-suffer/commit/ea1176bd9058e83559e38613565e136559d4a2c6)
[Merge Sort](https://github.com/florayuan18/just-to-suffer/commit/a1fdb50ed6f373c81bb2a403f2118c45d2c0de33)
[Bubble Sort](https://github.com/florayuan18/just-to-suffer/commit/9ab77f45347949ab95f7d309b7f4e38c17ba1c3d)

## Replit
[Replit](https://replit.com/@florayuan18/DataStructures#Main.java)